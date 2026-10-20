# 진민경 · Jin Minkyoung

### Flutter App Developer

Flutter로 만든 앱을 **App Store·Google Play에 출시해 2년째 운영**하고 있습니다.
기능을 구현하는 데서 끝내지 않고, 운영 중 발견한 문제를 데이터 구조와 서버 규칙으로 해결합니다.

세종대학교 인공지능학과 · 2027.02 졸업 예정
[Portfolio](https://b-dandelion.github.io/portfolio/) · [Email](mailto:jinbabging@gmail.com)

---

## Featured Projects

### 🎻 포레스트링 Teacher · Student
**Production Mobile App · 1인 개발 · 2024.10 출시 ~ 운영 중**

[Teacher Repo](https://github.com/B-Dandelion/forestring-teacher) · [Student Repo](https://github.com/B-Dandelion/forestring-student) · [App Store](https://apps.apple.com/kr/app/id6736948353) · [Google Play](https://play.google.com/store/apps/details?id=forestring.student.app) · [Case Study](https://b-dandelion.github.io/portfolio/forestring.html)

바이올린 학원 지점 2곳에서 실제로 쓰는 수업 예약·운영 앱입니다. 요구사항 정리부터 앱, 데이터 구조, 백엔드 로직, 스토어 배포, 운영까지 혼자 맡고 있습니다.

| 누적 수강생 | 수업 기록 | DB 함수 | RLS 정책 |
| --- | --- | --- | --- |
| 96명 | 3,690건 | 174개 | 21개 |

<sub>2026-10-20 운영 DB 기준, 앱 심사용·QA 계정 제외</sub>

- Flutter 앱 2개로 Teacher / Manager / Master / Student 4개 역할의 흐름을 나눠 구현
- Firebase 기반 초기 구조를 Supabase/PostgreSQL 중심으로 재설계하고, 권한과 중요한 변경 규칙을 RLS·RPC로 서버에서 검증
- 수업 취소 → 수업권 반환 → 보강 예약으로 이어지는 수업권 상태 흐름을 DB 단에서 관리해 중복 사용과 잘못된 상태 변경을 차단
- 학기 자동 전환이 매일 밤 실패하던 원인을 강사 근무시간 버전 충돌로 추적해 수정하고, 예정 수업 961건이 규칙을 지키는지 쿼리로 재검증

`Flutter` · `Dart` · `Supabase` · `PostgreSQL` · `PL/pgSQL` · `RLS` · `RPC` · `Edge Functions`

---

### 🗂️ INC Website
**Full-stack Web Service · 1인 개발 · 2026.02 공개**

[Repository](https://github.com/B-Dandelion/INC_Website) · [Live](https://inc-kings.vercel.app/) · [Case Study](https://b-dandelion.github.io/portfolio/inc.html)

기관의 발간물·세미나·보고서를 공개 범위에 따라 제공하는 권한 기반 자료실입니다. 게시판 11개에서 자료 679건을 관리하고 있습니다(2026-10-20 기준).

- 자료 정보는 PostgreSQL에, 실제 파일은 Cloudflare R2에 나눠 저장
- R2 업로드 후 DB 저장이 실패하면 올린 파일을 지워, 목록에 없는 파일이 남지 않도록 처리
- `public / member / admin` 공개 범위와 관리자 권한을 서버 API에서 검증
- 기존 자료를 새 구조로 옮기는 이관 스크립트 작성

`Next.js` · `TypeScript` · `Supabase` · `PostgreSQL` · `Cloudflare R2` · `Vercel`

---

## Other Projects

| 프로젝트 | 내용 | 형태 |
| --- | --- | --- |
| [COURTIFY](https://github.com/B-Dandelion/COURTIFY) · [Server](https://github.com/B-Dandelion/courtify_server) | Flutter + FastAPI + KoBART 판결문 기사형 요약 앱. 금액·이자율·판결 결론이 보존되는지 별도 기준으로 검증 | 수업 프로젝트 |
| [Porter](https://github.com/B-Dandelion/capstone-frontend) | 자율배송 캡스톤의 Flutter 앱. 카메라 OCR로 목적지를 읽어 배송 mission을 만들고 장비 통신으로 연결 | 캡스톤 팀 |
| [VR AI Interactive Experience](https://github.com/B-Dandelion/VR-AI-Interactive-Experience) | Meta Quest에서 음성 질문을 STT → LLM → TTS로 처리해 답하는 VR 콘텐츠 (Unity · FastAPI) | 4인 팀 |
| 2024 데이터 크리에이터 캠프 | ResNet-18로 31종 패션 스타일 이미지 분류. 배경 제거 전처리와 클래스 불균형 대응 실험 | 4인 팀 · 장려상 |

---

## How I Work

**운영을 기준으로 설계합니다**
권한, 데이터 정합성, 실패 처리, 마이그레이션까지 고려해서, 문제를 사후 수정이 아니라 구조와 규칙으로 막으려고 합니다.

**흐름 전체를 연결합니다**
화면 입력부터 클라이언트 상태, 서버 검증, 데이터 저장, 사용자 피드백까지 하나의 흐름으로 동작하는지 확인합니다.

---

## Tech Stack

| Area | Technologies |
| --- | --- |
| **Mobile** | Flutter, Dart, Provider, Android / iOS 스토어 배포 |
| **Backend / Data** | Supabase, PostgreSQL, PL/pgSQL, RLS, RPC, Edge Functions |
| **Web** | Next.js, TypeScript, Cloudflare R2, Vercel |
| **Also used** | FastAPI, PyTorch, Unity / C# |
| **Tools** | Git, GitHub, Figma |
