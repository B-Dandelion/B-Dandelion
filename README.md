# 진민경 · Jin Minkyoung

### AI Service & Interactive Contents

**AI 기술을 실제 서비스와 콘텐츠 경험으로 연결하는 개발자**를 지향합니다.  
사용자 입력이 클라이언트의 상태 변화와 서버·데이터·AI 처리로 이어지고, 다시 사용자가 체감하는 결과로 돌아오는 전체 흐름을 구현하는 데 관심이 있습니다.

세종대학교 인공지능학과 · 2027.02 졸업 예정

---

## What I Build

- **Interactive / Game-side Software** — Unity/C# 기반 XR 인터랙션, 입력·상태·오디오·서버 연동
- **Mobile Services** — Flutter 앱, 역할별 사용자 흐름, 실제 서비스 출시·운영
- **Backend & Data** — Supabase/PostgreSQL, RLS, RPC, FastAPI, 권한과 도메인 규칙 설계
- **AI Integration** — LLM·STT·TTS·NLP 모델을 서비스 흐름에 연결하고 결과를 검증
- **Web Services** — Next.js 기반 웹 애플리케이션, 인증·스토리지·배포·실패 처리

---

## Selected Projects

| Project | What I built | Stack |
| --- | --- | --- |
| **[VR AI Interactive Experience](https://github.com/B-Dandelion/VR-AI-Interactive-Experience)** | Meta Quest에서 음성 질문을 **STT → LLM → TTS**로 처리해 VR 안에서 재생하는 인터랙션 흐름. Unity/C# 입력·오디오·HTTP 통신과 FastAPI AI 서버 통합 | Unity, C#, XR Interaction Toolkit, FastAPI, faster-whisper, Gemini, Edge TTS |
| **[포레스트링 Teacher](https://github.com/B-Dandelion/Forestring_teach)** · **[Student](https://github.com/B-Dandelion/forestring_stu)** | 바이올린 학원에서 실제 운영 중인 수업 일정 관리 서비스. **1인 개발**로 앱·DB·백엔드·스토어 배포·운영을 담당하고 Firebase 구조를 Supabase/PostgreSQL 기반으로 재설계 | Flutter, Dart, Supabase, PostgreSQL, RLS, RPC |
| **[INC Website](https://github.com/B-Dandelion/INC_Website)** · **[Live](https://inc-kings.vercel.app/)** | 콘텐츠 아카이브 웹사이트 **1인 개발**. 역할별 공개 범위, 관리자 업로드, PostgreSQL 메타데이터와 R2 파일 저장소 분리, 업로드 실패 rollback 구현 | Next.js, TypeScript, Supabase, Cloudflare R2, Vercel |
| **[Porter — Autonomous Delivery App](https://github.com/B-Dandelion/capstone-frontend)** | 자율배송 캡스톤의 Flutter 앱과 **mission/control interface** 담당. 기사·입주민 UI, OCR 기반 목적지 입력, 배송 상태 및 장비 통신 흐름 구현 | Flutter, Dart, Google ML Kit, HTTP, Wi-Fi |
| **[COURTIFY](https://github.com/B-Dandelion/COURTIFY)** · **[Server](https://github.com/B-Dandelion/courtify_server)** | 민사 판결문을 기사형 요약으로 변환하는 **수업 프로젝트 프로토타입**. 생성 결과의 금액·이자율·결론 보존 여부를 별도 기준으로 검증 | Flutter, FastAPI, KoBART, PyTorch, Transformers |

---

## Engineering Focus

### System Integration
서로 다른 런타임과 서비스를 단순히 연결하는 데서 끝내지 않고, **입력 → 상태 → 통신 → 데이터/AI 처리 → 사용자 피드백**의 경계를 명확히 설계하는 것을 중요하게 생각합니다.

### Live-service Engineering
포레스트링을 실제 운영하면서 일정 생성 오류와 누락 데이터를 직접 추적·복구했고, 이후 반복적인 사후 수정 대신 **데이터 구조와 권한·도메인 규칙을 재설계**했습니다.

### AI with Verification
생성형 AI와 모델 출력을 그대로 사용하는 것보다 **목적과 제약을 먼저 정의하고, 실제 데이터·예외 상황·평가 기준으로 다시 검증**하는 방식으로 활용합니다.

---

## Tech Stack

| Area | Technologies |
| --- | --- |
| **Client / Interactive** | Unity, C#, Flutter, Dart, XR Interaction Toolkit |
| **Backend / Data** | Supabase, PostgreSQL, SQL, PL/pgSQL, RLS, RPC, FastAPI |
| **Web** | Next.js, TypeScript, Cloudflare R2, Vercel |
| **AI / ML** | Gemini API, faster-whisper, Edge TTS, KoBART, PyTorch, Transformers |
| **Tools** | Git, GitHub, Figma |

---

## Current Direction

현재는 **게임·인터랙티브 콘텐츠 개발, AI 서비스 개발, LLM/AI Agent, Human-AI Interaction** 영역을 중심으로 프로젝트와 취업 준비를 이어가고 있습니다.

프로젝트를 볼 때는 결과 화면뿐 아니라 각 저장소의 README에 정리한 **구조, 역할, 기술적 판단, 운영 과정**도 함께 확인해 주세요.
