# 진민경 · Jin Minkyoung

### AI Service & Interactive Contents

**AI 기술을 실제 사용자가 체감하는 서비스와 인터랙티브 경험으로 구현하는 개발자**를 지향합니다.

모델이나 API 자체보다, 사용자의 입력이 **클라이언트 상태 → 서버·데이터 처리 → AI 추론 → 사용자 피드백**으로 이어지는 전체 흐름을 설계하고 구현하는 데 관심이 있습니다.  
Flutter/Next.js 기반 서비스 개발, Supabase/PostgreSQL 백엔드, Unity/XR 인터랙션, AI 모델·API 연동을 프로젝트 안에서 함께 다뤄왔습니다.

세종대학교 인공지능학과 · 2027.02 졸업 예정

---

## What I Build

### AI-powered Products
LLM·STT·TTS·NLP 모델을 단순 호출하는 데서 끝내지 않고, **사용자 입력과 서비스 흐름 안에 연결하고 결과를 검증**합니다.

### Service Engineering
Flutter와 Next.js 기반 앱·웹을 만들고, Supabase/PostgreSQL의 **인증·권한·도메인 규칙·데이터 정합성**까지 함께 설계합니다.

### Interactive Systems
Unity/XR, 모바일 입력, 장비 인터페이스처럼 사용자의 행동이 시스템 상태와 외부 처리로 이어지는 **인터랙티브 소프트웨어 경계**를 구현합니다.

---

## Featured Projects

### 🥽 [VR AI Interactive Experience](https://github.com/B-Dandelion/VR-AI-Interactive-Experience)
**Voice AI × Unity XR · 4인 팀 프로젝트**

Meta Quest에서 사용자의 음성 질문을 **STT → LLM → TTS**로 처리하고 다시 VR 안에서 음성으로 재생하는 인터랙티브 콘텐츠입니다.

- Unity/C# 음성 입력, 오디오 데이터 처리, XR 상태 및 인터랙션 구현
- `UnityWebRequest` 기반 Unity ↔ FastAPI 통신
- faster-whisper → Gemini → Edge TTS AI voice pipeline 구현
- 입력 장치부터 AI 응답 재생까지 클라이언트·서버 전체 흐름 통합

`Unity` · `C#` · `XR Interaction Toolkit` · `FastAPI` · `faster-whisper` · `Gemini` · `Edge TTS`

---

### 🎻 [포레스트링 Teacher](https://github.com/B-Dandelion/forestring-teacher) · [Student](https://github.com/B-Dandelion/forestring-student)
**Production Mobile Service · 1인 개발**

실제 바이올린 학원에서 운영 중인 수업 일정 관리 서비스입니다. 요구사항 정리부터 앱·데이터 구조·백엔드 로직·스토어 배포·운영 및 유지보수까지 담당했습니다.

- Flutter 기반 Teacher / Manager / Master / Student 사용자 흐름
- Firebase 구조를 Supabase/PostgreSQL 기반으로 재설계
- RLS·RPC·Edge Functions를 이용한 역할별 권한 및 서버 검증
- 수업 취소 → 수업권 반환 → 보강 사용의 도메인 lifecycle 설계
- 운영 중 발생한 일정 누락·정합성 문제를 추적하고 데이터 구조와 규칙으로 개선

`Flutter` · `Dart` · `Supabase` · `PostgreSQL` · `RLS` · `RPC` · `Edge Functions`

---

### 🗂️ [INC Website](https://github.com/B-Dandelion/INC_Website) · [Live](https://inc-kings.vercel.app/)
**Full-stack Content Service · 1인 개발**

기관의 발간물·세미나·보고서 등을 관리하는 권한 기반 콘텐츠 아카이브 웹사이트입니다.

- Next.js App Router 기반 프론트엔드·서버 API 구현
- `public / member / admin` 공개 범위 및 관리자 권한 설계
- PostgreSQL 메타데이터와 Cloudflare R2 파일 저장소 분리
- R2 업로드 후 DB 저장 실패 시 객체를 제거하는 rollback 처리
- 기존 자료 이관 스크립트와 Vercel 배포·운영

`Next.js` · `TypeScript` · `Supabase` · `PostgreSQL` · `Cloudflare R2` · `Vercel`

---

### ⚖️ [COURTIFY](https://github.com/B-Dandelion/COURTIFY) · [Server](https://github.com/B-Dandelion/courtify_server)
**NLP Service Prototype · 수업 프로젝트**

민사 판결문을 기사형 요약으로 변환하는 Flutter + FastAPI 기반 AI 서비스 프로토타입입니다.

- KoBART 기반 법률 문서 요약 inference pipeline
- 금액·이자율·판결 결론 보존 여부를 별도 평가 기준으로 정의
- 입력 구조와 decoding 설정을 조정해 생성 실패 유형을 검증
- AI 출력을 그대로 사용하는 대신 **사용 목적에 맞는 실패 기준을 먼저 정의하고 평가**

`Flutter` · `FastAPI` · `KoBART` · `PyTorch` · `Transformers`

---

## Additional Project

**[Porter — Autonomous Last-mile Delivery App](https://github.com/B-Dandelion/capstone-frontend)**  
캡스톤 팀 프로젝트에서 Flutter 앱과 **delivery mission / control interface**를 담당했습니다. 카메라 OCR → 목적지 파싱 → 배송 mission 생성 → 장비 통신 경계를 구현하며 사용자 작업을 로봇 실행 계층에 연결했습니다.

---

## Engineering Approach

**End-to-end Integration**  
서로 다른 기술을 나열하기보다 **입력 → 상태 → 통신 → 데이터/AI 처리 → 사용자 피드백**이 하나의 경험으로 동작하도록 연결합니다.

**Production-oriented Design**  
실제 운영 서비스에서 권한, 데이터 정합성, 실패 처리, migration과 유지보수까지 고려하며 문제를 사후 수정이 아닌 구조와 규칙으로 해결하려고 합니다.

**AI with Verification**  
AI 결과를 그대로 신뢰하기보다 목적과 제약을 정의하고, 실제 실패 유형과 평가 기준을 통해 결과를 다시 확인합니다.

---

## Tech Stack

| Area | Technologies |
| --- | --- |
| **Client / Interactive** | Flutter, Dart, Unity, C#, XR Interaction Toolkit |
| **Backend / Data** | Supabase, PostgreSQL, SQL, PL/pgSQL, RLS, RPC, FastAPI |
| **Web** | Next.js, TypeScript, Cloudflare R2, Vercel |
| **AI / ML** | Gemini API, faster-whisper, Edge TTS, KoBART, PyTorch, Transformers |
| **Tools** | Git, GitHub, Figma |

---

## Current Focus

현재는 **AI-powered products와 interactive systems의 접점**을 중심으로 역량을 확장하고 있습니다.  
특히 LLM/AI Agent 기술이 실제 앱·웹·XR의 사용자 인터랙션과 서비스 workflow 안에서 어떻게 동작할 수 있는지에 관심을 두고 있습니다.
