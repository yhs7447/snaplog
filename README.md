📸 SNAPLOG – AI 기반 사진 일기 웹 서비스

사진 한 장으로 하루를 기록하는 AI 일기 서비스

SNAPLOG는 사용자가 업로드한 사진을 기반으로
이미지 분석과 LLM(OpenAI API)을 활용해 자동으로 감성적인 일기를 생성하는
사진 기반 자동 일기 생성 웹 서비스입니다.

글을 직접 작성해야 하는 부담을 줄이고,
사진 속 정보(EXIF, 위치, 분위기)를 바탕으로
하루의 경험을 자연스럽게 기록할 수 있도록 설계되었습니다.
---

🔗 서비스 링크

🌐 배포 URL: https://snaplog-app-water.azurewebsites.net

※ 현재 외부 API 키 제거로 일부 기능(로그인/생성) 제한
---

👩‍💻 프로젝트 정보

유형: 팀 프로젝트 (Microsoft AI 엔지니어 양성과정)

기간: 2025.10.23 ~ 2025.11.14(1개월 120H)

인원: 3명

주제: AI 기반 사진 일기 자동 생성 서비스
---

🙋‍♀️ 담당 역할 (개인 기여)

UI/UX · 이미지 처리 · AI 일기 생성 전담

UI/UX 전체 설계

사진 업로드 기능 구현

업로드된 이미지 분석 로직 구현

LLM(OpenAI API)을 활용한 자동 일기 생성 기능 구현

GPT-4o-mini / GPT-4o 기반
3단계 AI 생성 파이프라인 설계 (분석 → 초안 → 보정)
---

✨ 주요 기능
1️⃣ 사진 업로드 및 분석

이미지 업로드

EXIF 데이터 추출 (촬영 시간, GPS)

이미지 주요 요소 및 분위기 분석

2️⃣ AI 자동 일기 생성

OpenAI API 활용

사진 기반 사실 정보 추출 후 감성 문장 생성

사용자 경험을 고려한 자연스러운 말투 적용

3️⃣ 지도 기반 추억 시각화

EXIF 위치 정보 기반 지도 표시

Leaflet.js를 활용한 지도 시각화

방문 장소 클러스터링 및 경로 표시
---

🧠 AI 생성 구조 (핵심)

3단계 교차 검증 파이프라인

분석 단계

이미지에서 사실 정보 추출 (객체, 배경, 분위기)

안전성 필터 적용

초안 생성

GPT-4o-mini / GPT-4o 활용

비용 효율성과 품질을 고려한 모델 분리

보정 단계

초안을 자연스러운 일기 문장으로 개선

감정 과장 최소화, 현실성 강화
---

🛠 기술 스택
🖥 Frontend

HTML / CSS / JavaScript

IndexedDB (브라우저 로컬 DB)

exifr (이미지 EXIF 데이터 파싱)

Leaflet.js (지도 시각화, 클러스터링)

⚙️ Backend

Python

Flask (API 엔드포인트, 라우팅, CORS 처리)

Azure Cosmos DB (NoSQL, CRUD)

🤖 AI / External API

OpenAI API (자동 일기 생성)

OpenStreetMap API (지도 시각화)

🧰 Development & Collaboration

Git / GitHub

VS Code

Cursor

🧠 AI Assist Tools

Copilot

Gemini Code Assist

ChatGPT

Claude

🚀 배포

Azure Web Service: 웹 서비스 배포

GitHub Pages: 정적 웹 리소스 배포


🔐 테스트 계정
ID: estt8758@gmail.com
PW: estt8758
---

📈 확장 가능성

사용자 문체/감정 기반 개인화 일기

멀티모달 입력 (음성, 영상)

날씨 API 연동

프리미엄 구독 모델

여행 로그 / 포토북 제작 서비스
---

📝 회고

“문제를 명확히 정의하면 해결 속도가 빨라진다”

이번 프로젝트를 통해
AI 기반 서비스 설계, 이미지 처리, LLM 파이프라인 구성,
그리고 실제 서비스 배포까지 웹 서비스의 전체 흐름을 경험할 수 있었습니다.

앞으로도 이러한 경험을 바탕으로
사용자에게 실질적인 가치를 제공하는 백엔드 개발자로 성장하고자 합니다.