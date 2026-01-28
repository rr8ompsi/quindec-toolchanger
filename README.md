## Overview

**Project Quindecum – A 15-Tool Toolchanger 3D Printer**

Project Quindecum is an open-source toolchanger project built around the  
**Quindec Toolchanger**, a high-density multi-tool system originally developed
for a **Voron 2.4 (350mm)** printer.

The name **Quindec** is derived from the Latin word for *fifteen*.  
On a 350mm Voron 2.4 platform, this toolchanger is designed to support  
**up to 15 independent tools**, prioritizing tool count while maintaining
mechanical feasibility.

Although the current implementation targets the Voron 2.4 (350mm),
the overall architecture is **not inherently limited to a single printer model**.

The toolchanger can be adapted to other CoreXY-style printers by modifying
the **Tool Carriage Holder** to match the target printer’s A/B idler geometry.
No fundamental changes to the tool or dock architecture are required.

The current Voron-based design should be understood as a **reference platform**,
not a hard limitation.

This project focuses on two primary design goals:

1. **Accessibility and cost efficiency**
   - Use commonly available and inexpensive components
   - Avoid specialized or hard-to-source parts where possible

2. **Maximum tool density**
   - Treat tool count as a primary design constraint
   - Optimize layout and geometry to support as many tools as possible
  
While the mounting interface may change between printers,
the architectural boundaries and control responsibilities of the system
remain intentionally consistent.

See: [DESIGN_SCOPE_AND_INTENT.md](DESIGN_SCOPE_AND_INTENT.md)

## 개요

**Project Quindecum – A 15-Tool Toolchanger 3D Printer**

Project Quindecum은  
**Quindec Toolchanger**를 중심으로 설계된 오픈소스 툴체인저 프로젝트입니다.  
현재 구현은 **Voron 2.4 (350mm)** 프린터를 기준으로 개발되었습니다.

**Quindec**라는 이름은 라틴어로 *15*를 의미하며,  
350mm 규격의 Voron 2.4 프린터에서  
**최대 15개의 툴을 수용할 수 있도록 설계된 툴체인저**라는 점에서  
이 이름을 사용했습니다.

현재 설계는 Voron 2.4 (350mm)를 기준으로 하지만,  
이 툴체인저의 구조는 **특정 프린터에 고정된 설계가 아닙니다**.

다른 CoreXY 계열 프린터에서도  
**Tool Carriage Holder 구조물만 해당 프린터의 A/B Idler 구조에 맞게 수정하면**,  
툴과 툴 거치대 구조를 그대로 유지한 채 적용이 가능합니다.

즉, Voron 2.4 기반 설계는  
**현재 시점의 기준 플랫폼(reference platform)**일 뿐,  
확장 가능성을 제한하기 위한 선택은 아닙니다.

이 프로젝트의 설계에서 가장 중요하게 고려한 키포인트는 다음 두 가지입니다.

1. **부품 수급의 용이성과 비용**
   - 구하기 쉬운 범용 부품 위주의 설계
   - 가능한 한 저렴한 구성 유지

2. **툴 개수의 극대화**
   - 툴 개수를 설계의 핵심 제약 조건으로 설정
   - 구조와 배치를 최적화하여 최대한 많은 툴 배치

프린터에 따라 장착 인터페이스는 달라질 수 있지만,  
시스템의 구조적 경계와 제어 책임은 의도적으로 동일하게 유지됩니다.

자세한 내용은 아래 문서를 참고해 주세요.  
➡ [DESIGN_SCOPE_AND_INTENT.md](DESIGN_SCOPE_AND_INTENT.md)

