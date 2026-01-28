## Overview

**Project Quindecum – A 15-Tool Toolchanger 3D Printer**

![image](./pics/preview.jpg)

Here are some videos demonstrating the Quindec Toolchanger in action:

[![6 Tools stress test with MGN rail](http://img.youtube.com/vi/-aM5X-14fe0/0.jpg)](https://www.youtube.com/watch?v=-aM5X-14fe0)
[![6 color test on my new toolchanger](http://img.youtube.com/vi/941lrKT-fIY/0.jpg)](https://www.youtube.com/watch?v=941lrKT-fIY)

**Join my Discord Server:**

[![Join Discord](https://img.shields.io/badge/Discord-Join%20Chat-5865F2?logo=discord&logoColor=white)](https://discord.gg/CxMwUS3zvY)

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

## Project Status & Upcoming Release

Project Quindecum is currently in a **closed beta testing phase**.

The project will be publicly released once all remaining legal and
intellectual-property related considerations have been carefully reviewed
and resolved.  
This is a precautionary step to ensure that the project can be shared openly
and responsibly.

A public release is planned in the near future.

---

## Closed Beta Test Participation

Closed beta testers are currently being recruited.

### Preferred configuration
You may apply for the closed beta if:
- You own a **Voron 2.4**
- Your printer uses the **stock Voron 2.4 A/B idler configuration**

This configuration requires no redesign of the Tool Carriage Holder
and is the primary reference platform for testing.

### Other configurations
You may also apply if:
- Your printer is **not a Voron 2.4**, or
- Your Voron uses **non-stock A/B idlers**

In this case, you are expected to **design and adapt your own Tool Carriage Holder**
to match your printer’s A/B idler geometry.

---

## Expectations for Beta Testers

Closed beta testers are expected to actively participate in the project by:

- Testing the toolchanger in real printing scenarios
- Providing feedback on mechanical, electrical, and usability aspects
- Reporting issues and edge cases
- Assisting with documentation, diagrams, or build notes when possible
- Contributing in any other helpful way as the project evolves

This is a collaborative testing effort rather than a one-way distribution.

If you are interested in participating, please be prepared to share
constructive feedback and practical insights during the testing phase.


## 개요

**Project Quindecum – A 15-Tool Toolchanger 3D Printer**

![image](./pics/preview.jpg)

Quindec Toolchanger의 동작을 보여주는 영상들입니다.

[![6 Tools stress test with MGN rail](http://img.youtube.com/vi/-aM5X-14fe0/0.jpg)](https://www.youtube.com/watch?v=-aM5X-14fe0)
[![6 color test on my new toolchanger](http://img.youtube.com/vi/941lrKT-fIY/0.jpg)](https://www.youtube.com/watch?v=941lrKT-fIY)

**디스코드 서버 링크:**

[![Join Discord](https://img.shields.io/badge/Discord-Join%20Chat-5865F2?logo=discord&logoColor=white)](https://discord.gg/CxMwUS3zvY)

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

## 프로젝트 상태 및 공개 예정

Project Quindecum은 현재 **클로즈드 베타 테스트 단계**에 있습니다.

본 프로젝트는 남아 있는 법적·지식재산권 관련 사항을 충분히 검토하고
문제가 없음을 명확히 한 이후에 공개될 예정입니다.  
이는 프로젝트를 보다 책임감 있고 안정적으로 공개하기 위한
사전 조치입니다.

정식 공개는 **빠른 시일 내**에 이루어질 예정입니다.

---

## 클로즈드 베타 테스트 참여 안내

현재 클로즈드 베타 테스트 참여자를 모집 중입니다.

### 우선 대상 구성
아래 조건에 해당하는 경우, 클로즈드 베타 테스트에 지원할 수 있습니다.

- **Voron 2.4** 프린터를 보유하고 있고
- **순정 Voron 2.4 A/B 아이들러 구조**를 사용하는 경우

이 구성은 Tool Carriage Holder의 추가 설계 없이 바로 테스트가 가능하며,
현재 프로젝트의 기준(reference) 플랫폼입니다.

### 기타 구성
아래 경우에도 지원은 가능합니다.

- Voron 2.4가 아닌 다른 프린터를 사용하는 경우
- Voron 2.4이지만 **A/B 아이들러가 순정이 아닌 경우**

이 경우, 해당 프린터에 맞는 **Tool Carriage Holder를 직접 설계해야 합니다.**

---

## 베타 테스터에게 기대하는 사항

클로즈드 베타 테스터는 단순 사용자가 아니라,
프로젝트에 함께 참여하는 협력자로서 다음과 같은 역할을 기대합니다.

- 실제 출력 환경에서 툴체인저 테스트
- 기구, 전기, 사용성 관련 피드백 제공
- 문제점 및 엣지 케이스 리포트
- 가능하다면 문서화, 다이어그램, 빌드 노트 작성 지원
- 기타 프로젝트에 도움이 되는 다양한 기여

본 베타 테스트는 일방적인 배포가 아닌,
**상호 피드백을 기반으로 한 협업 과정**입니다.

참여를 원하신다면, 테스트 과정에서
적극적인 피드백과 경험 공유가 가능하신 분을 환영합니다.
