# Design Scope and Architectural Intent  
(Project Quindecum)

This document defines the architectural boundaries and non-goals of Project Quindecum.
Its purpose is to prevent ambiguity regarding system behavior, component responsibility,
and control relationships.

---

## 1. Major Components

Project Quindecum consists of the following conceptual components:

### Tool
- A mechanically passive unit containing a nozzle and sensors.
- A tool has no active electrical functionality unless mechanically attached
  to the toolhead.

### Toolhead
- The only component that supplies electrical power, data, and control signals
  to a tool.
- A tool is electrically active only when attached to the toolhead.

### Tool Carriage
- A mechanically passive structure used to hold tools when not in use.
- Tool carriages have no electrical or data interface with tools.

---

## 2. Electrical and Control Boundaries

The following constraints are fundamental to the system architecture:

- No electrical power or data is supplied to a tool unless it is attached
  to the toolhead.
- Tool carriages do not initialize, control, communicate with, or power tools.
- Control responsibility for a tool never transitions between subsystems.

A tool is either:
- Attached to the toolhead and fully controlled, or
- Held by a tool carriage and electrically inert.

---

## 3. Tool Carriage Cooling System Intent

Some tool carriages may include cooling fans.

These cooling systems are intentionally constrained as follows:

- Tool-carriage-mounted cooling fans are powered directly by the system.
- Cooling fans are electrically and logically isolated from the tool.
- No electrical path exists between the cooling system and the tool.
- Cooling fans do not read, infer, or respond to tool temperature,
  tool state, or tool identity.

Cooling is treated as **tool-carriage-local environmental management**,  
not tool control.

---

## 4. Cooling Control Logic

Cooling fan behavior may be determined by:

- Tool carriage slot occupancy state
- Static job configuration information
- Recent tool carriage activity

Cooling fan behavior does not depend on:

- Tool electrical state
- Tool temperature
- Tool readiness
- Tool initialization or preconditioning

Cooling decisions are scoped to **tool carriage slots as physical locations**,  
not to tools as active devices.

---

## 5. Explicit Non-Goals

Project Quindecum explicitly does not implement:

- Any mechanism by which a tool carriage supplies power or data to a tool
- Tool initialization, sensing, heating, or control while held by a tool carriage
- Multi-source power or control architectures for tools
- Any form of tool operation outside of attachment to the toolhead

---

## 6. Design Philosophy

Project Quindecum enforces a strict single-point-of-control model.

This is a deliberate architectural decision and is considered a core
design constraint rather than an implementation detail.
