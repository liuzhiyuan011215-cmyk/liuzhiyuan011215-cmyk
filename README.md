# 안녕하세요, LIU ZHIYUAN(유지원)입니다 👋

**AI 응용 개발자**를 목표로 하는 한국교통대학교 소프트웨어전공 학생입니다.
대규모 언어 모델(LLM)·음성 인식·OCR을 **실제로 매일 쓰는 도구**로 만드는 일을 합니다.
유학생으로서 직접 겪은 불편(수업 언어, 단어 암기, 게임 속 의사소통)에서 문제를 찾고, 끝까지 배포해서 씁니다.

> 🇨🇳 中国留学生 · 한국어 / 中文 / English · 目标岗位：AI 应用开发

---

## 🎯 희망 직무: AI 응용 개발 (AI Application Engineer)

| 직무에서 필요한 역량 | 이를 보여주는 프로젝트 |
|---|---|
| LLM을 서비스에 붙이고 **환각을 검증**하는 설계 | [CardMaker](https://github.com/liuzhiyuan011215-cmyk/CardMaker) (사전 대조 검증), [report2excel](https://github.com/liuzhiyuan011215-cmyk/report2excel) (금액 재계산·단가 이상 탐지) |
| **실시간 음성** AI (스트리밍, 재연결) | [valorant-translator](https://github.com/liuzhiyuan011215-cmyk/valorant-translator), [translator-ultimate](https://github.com/liuzhiyuan011215-cmyk/translator-ultimate), [live-translate](https://github.com/liuzhiyuan011215-cmyk/live-translate) |
| 데이터 정제·정규화 | [knut-campus-guide](https://github.com/liuzhiyuan011215-cmyk/knut-campus-guide) (250건 → 178곳, 합계 검증) |
| 협업·오픈소스 기여 | DouDuo [PR #3](https://github.com/81199000/DouDuo/pull/3)·[PR #5](https://github.com/81199000/DouDuo/pull/5) 원작자 병합, [campuse_place PR #2](https://github.com/skyhy0228/campuse_place/pull/2) 팀 프로젝트 기여 |
| 자동화·배포 (GitHub Actions / Pages) | [ai-briefing](https://github.com/liuzhiyuan011215-cmyk/ai-briefing), 웹 프로젝트·과제 5건 Pages 배포 |
| 테스트로 품질 보증 | CardMaker **pytest 238개** (API Key 없이 실행 가능) |

## 🛠 기술 스택

- **언어**: Python · JavaScript · HTML/CSS · (Swift 일부)
- **AI / API**: Google Gemini (Live API 포함) · 알리바바 DashScope(Qwen) · Groq Whisper · 멀티모달 LLM OCR
- **데스크톱 / 데이터**: PySide6 · SQLite · PyMuPDF · RapidOCR · openpyxl · AnkiConnect
- **품질 / 배포**: pytest · Git · GitHub Actions · GitHub Pages
- **AI 협업 개발**: Claude Code 등 AI 코딩 도구로 구현하고, **설계·테스트·실사용 검증은 직접** 합니다. 대표작 CardMaker는 심사 면담 이후 수정부터 AI가 도운 커밋을 `(AI)`로 표시해 구분했습니다.

---

## ⭐ 대표 프로젝트 — CardMaker (졸업작품 · 캡스톤디자인)

**PDF·스캔본 단어장 → 사전으로 검증된 Anki 학습 카드 자동 생성 데스크톱 앱**

- **문제**: LLM으로 단어 뜻을 뽑으면 그럴듯한 오답(환각)이 섞여 그대로 암기하게 됨
- **해결**: OCR → LLM 추출 → **국립국어원 krdict · ECDICT · 위키낱말사전 · PanLex로 대조 검증** → 통과한 카드만 자동 선택
- **규모**: 커밋 30여 개 · 테스트 238개 · Windows/macOS · 한/중/영 UI · CLI와 MCP 서버도 제공
- **본인 역할**: 개인 프로젝트(기획·설계·구현·테스트·문서 전부). 심사 면담 후 Windows 호환·오프라인 사전 3종·오탐 방지 수정을 직접 진행

👉 [저장소 보기](https://github.com/liuzhiyuan011215-cmyk/CardMaker)

---

## 📂 프로젝트 목록 (총 13개 · 프로필 저장소 제외)

### 1. 캡스톤디자인
| 프로젝트 | 내용 | 기술 |
|---|---|---|
| [CardMaker](https://github.com/liuzhiyuan011215-cmyk/CardMaker) | PDF 단어장 → 검증된 Anki 카드 | Python, PySide6, OCR, LLM, SQLite, pytest |

### 2. 팀 프로젝트
| 프로젝트 | 내용 | 본인 역할과 기여 |
|---|---|---|
| [campuse_place](https://github.com/liuzhiyuan011215-cmyk/campuse_place) (원본: [skyhy0228/campuse_place](https://github.com/skyhy0228/campuse_place)) | 교통대 맛집·숨은 장소·강의실 검색 통합 사이트 (팀원 4명 작업 통합) | **중국어(유학생) 모드 데이터 제공**: 장소 173곳 번역, 유학생 생활 꿀팁 5개, 유학생 추천 표시 (내 [knut-campus-guide](https://github.com/liuzhiyuan011215-cmyk/knut-campus-guide)에서 통합됨)<br>**추가 기능 PR** [#2](https://github.com/skyhy0228/campuse_place/pull/2) (검토 중): 중국어 번역 100%, 혼밥 가능 필터·배지, 오늘의 랜덤 추천 + 테스트<br>React/TS 통합 코드는 팀원(skyhy0228)이 작성 |

### 3. 개인 프로젝트
| 프로젝트 | 내용 | 기술 |
|---|---|---|
| [valorant-translator](https://github.com/liuzhiyuan011215-cmyk/valorant-translator) | 게임 중 팀원 음성 → 실시간 중국어 이중 자막, F8 누르고 말하면 영어/한국어로 번역 | Python, Gemini Live API, VB-Cable, 오버레이 UI |
| [translator-ultimate](https://github.com/liuzhiyuan011215-cmyk/translator-ultimate) | 유학생 수업 동시통역 (강의 PDF에서 전문용어 추출해 번역 정확도 향상) | Groq Whisper, DashScope, HTML/JS |
| [live-translate](https://github.com/liuzhiyuan011215-cmyk/live-translate) | 휴대폰 브라우저용 동시통역, 녹음·전사본을 내 구글 드라이브에 저장 | Gemini Live API, Google Drive API, GitHub Pages |
| [report2excel](https://github.com/liuzhiyuan011215-cmyk/report2excel) | 가게 영업 보고서(사진/PDF) → 수식·자동 검증이 들어간 Excel | Python, 멀티모달 LLM, SQLite, openpyxl, PySide6 |
| [ai-briefing](https://github.com/liuzhiyuan011215-cmyk/ai-briefing) | 매일 아침 AI 뉴스 3개를 골라 요약해서 카카오톡으로 전송 | Python, Gemini, GitHub Actions, Kakao API |
| [hacktoberfest-pomodoro](https://github.com/liuzhiyuan011215-cmyk/hacktoberfest-pomodoro) | 뽀모도로 + 할 일 관리 (MLH Global Hack Week 참가작) | HTML, CSS, JavaScript |

### 4. 수업 과제 결과물
| 프로젝트 | 과제 | 배포 |
|---|---|---|
| [knut-campus-guide](https://github.com/liuzhiyuan011215-cmyk/knut-campus-guide) | AI 데이터 서사 및 Vibe Coding — 250건 정규화 → 178곳, 한/중 전환 | [사이트](https://liuzhiyuan011215-cmyk.github.io/knut-campus-guide/) |
| [library-loan](https://github.com/liuzhiyuan011215-cmyk/library-loan) | 바이브코딩 실기 — 도서관 대출 시스템 | [사이트](https://liuzhiyuan011215-cmyk.github.io/library-loan/) |
| [room-booking](https://github.com/liuzhiyuan011215-cmyk/room-booking) | 바이브코딩 실기 — 강의실 예약 시스템 | [사이트](https://liuzhiyuan011215-cmyk.github.io/room-booking/) |
| [dino-game](https://github.com/liuzhiyuan011215-cmyk/dino-game) | GitHub 배포 실습 — 달리기 웹 게임 | [사이트](https://liuzhiyuan011215-cmyk.github.io/dino-game/) |

### 5. 오픈소스 수정 (타인의 원본 + 내 수정)
> 원본 코드는 원작자의 것이며, 아래 표에는 **내가 수정한 부분만** 적었습니다.

| 저장소 | 원본 | 내가 한 일 |
|---|---|---|
| [DouDuo](https://github.com/liuzhiyuan011215-cmyk/DouDuo) | [81199000/DouDuo](https://github.com/81199000/DouDuo) (iOS 동영상 클라이언트) | **원작자 저장소에 PR 2건 병합** (릴리스 노트에 기여자로 기재)<br>[#3](https://github.com/81199000/DouDuo/pull/3) v1.3.10: 배속 고정, 백그라운드 재생·잠금화면 컨트롤, 라이브 방송 선택 목록<br>[#5](https://github.com/81199000/DouDuo/pull/5) v1.3.13: 배속 전환 시 소리가 끊기지 않는 **독립 오디오 엔진**(약 850줄). 처음(v1.3.11)엔 위험 지적으로 보류 → 지적된 문제를 고쳐 다시 제출 → 병합, 현재도 원작자의 메인 코드에서 사용 중 |

---

## 📫 연락처
- Email: [liuzhiyuan011215@gmail.com](mailto:liuzhiyuan011215@gmail.com)
- GitHub: [@liuzhiyuan011215-cmyk](https://github.com/liuzhiyuan011215-cmyk)
