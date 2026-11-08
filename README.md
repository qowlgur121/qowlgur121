## 배지혁 · 신입 백엔드 개발자

AI를 실제 업무에 붙이고, 돈이 걸린 처리는 권한과 검증으로 막습니다.
혼자 운영한 온라인 판매의 주문 처리 서버를 설계해 하루 최대 1,378건을 처리했습니다. 결과를 모르는 주문은 재실행하지 않고 대조 후 확정하게 했고, AI 점검 에이전트에는 허용한 조치만 주었습니다.

[포트폴리오](https://qowlgur121.github.io) · [포트폴리오 PDF](https://qowlgur121.github.io/portfolio.pdf) · [이력서 PDF](https://qowlgur121.github.io/resume.pdf) · qowlgur121@gmail.com

### 주요 프로젝트

**판매 운영 자동화, AI 운영** &nbsp;개인 · 2026.09 ~ 10
- 결제 확인 → 공급처 발주 → 고객 발송 → 매시간 대사가 정해진 코드로 이어지는 주문 파이프라인. 하루 최대 **1,378건** 실거래 처리
- 공급처 응답이 끊겨 결과를 모르는 주문은 재구매하지 않고 보류한 뒤 거래 이력과 정확히 1건이 맞을 때만 확정. 중복 처리는 UNIQUE 제약과 조건부 UPDATE로 DB가 마지막에 차단
- AI 점검 에이전트는 상태를 읽고 보고하며 허용 목록의 조치만 실행. 재구매·코드 할당·고객 발송처럼 되돌릴 수 없는 조치는 코드 규칙과 사람 결정으로만
- 핵심 로직을 일반화한 공개 예제(재현 테스트 포함) → [order-fulfillment-guard](https://github.com/qowlgur121/order-fulfillment-guard)
- `Python` `SQLite(WAL)` `systemd` `Oracle Cloud`

**공공기관 AI 상담 챗봇, RAG** &nbsp;3인 팀 팀장 · 2025.09 ~ 12 · 전북특별자치도사회서비스원 산학
- 재학습이 필요했던 파인튜닝 챗봇을 공개 게시판을 매일 새벽 수집해 임베딩하는 RAG로 바꿔 복지사업 **1,809건**·시설 **18,319곳**이 재학습 없이 반영
- LLM이 의도·지역·대상 조건을 뽑고 실패하면 규칙으로 처리(6가지 의도 경로). 기관 포털을 고칠 수 없어 스크립트 한 줄로 붙는 위젯으로 연결
- 내 담당: 요구사항 협의·설계·서버·검색·인증 / 팀원: 자료 조사·발표·문서. 기관 성과보고회 표창 · 캡스톤디자인 우수상
- `FastAPI` `LangChain` `PostgreSQL + pgvector` `bge-m3` `Docker`

**[OpenContext](https://github.com/OpenContextAI/open-context) · 사내 문서 AI 검색 MCP 서버** &nbsp;3인 팀 · 2025.08 ~ 12
- 회사 문서를 밖으로 보내지 않고 AI 코딩 도구가 검색해 쓰는 사내 설치형 서버. 제안·기획과 설계를 맡음
- 내 담당: 검색 엔진(BM25 + 로컬 임베딩 벡터 점수 결합, 0~1 정규화), AI가 목록을 먼저 보고 필요한 원문만 가져가는 2단계 조회 API, DB, 관리자 화면, 배포 — 커밋 [b227bb6](https://github.com/OpenContextAI/open-context/commit/b227bb6) · [26be0ea](https://github.com/OpenContextAI/open-context/commit/26be0ea). 문서 처리 파이프라인·MCP 어댑터는 팀원
- 2025 오픈소스 개발자대회 출품 · 학부 작품경진대회 은상
- `Java 21` `Spring Boot` `Elasticsearch` `Ollama` `PostgreSQL` `MCP`

**현장실습 · (주)텔로스** &nbsp;학교 현장실습 · 2025.07 ~ 08
- 사내 직원 로그인·권한·좌석 관리와 출입 기록으로 근무 상태를 판정하는 웹 서비스 백엔드. 고칠 수 없는 외부 출입 단말 DB는 읽기 전용으로 연동, Docker로 회사 서버 배포
- `Java` `Spring Boot` `JPA` `Spring Security` `JWT` `SQL Server` `Docker`

주문 서버와 복지 챗봇 원본은 운영 서비스·기관 과제라 비공개입니다. 구조·판단·사고 기록은 포트폴리오에 있고, 면접에서 화면으로 보여드릴 수 있습니다.

### 소개

- **기술** &nbsp;Java · Spring Boot · Python · FastAPI · PostgreSQL · SQLite · Elasticsearch · Docker · Linux
- **학력** &nbsp;전북대학교 컴퓨터공학부 졸업 (2026.02) · 전공 3.83 / 4.5
- **자격증** &nbsp;정보처리기사 · SQLD · ADsP
