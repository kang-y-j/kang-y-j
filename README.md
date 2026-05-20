# 강영재 | AI Service Engineer Portfolio

> LLM · RAG · LangChain · Python 기반 AI 서비스 개발을 목표로 학습하고 있습니다.
> 데이터를 분석하고, 모델을 실제 서비스 흐름에 연결하여 실질적인 가치를 만드는 것을 목표로 합니다.

---

## About Me

AI 기능을 활용한 서비스 개발에 흥미를 가지고 있으며 LangChain과 Python 중심으로 LLM 기반 서비스 흐름을 설계하고 구현해본 경험이 있습니다.
이 GitHub는 제가 학습한 내용과 성장 과정을 기록하는 공간으로, AI 서비스 엔지니어로 성장하기 위한 다양한 실험과 프로젝트를 포함합니다.

---

## Career Interest

- AI Service Engineer
- LLM / RAG 기반 서비스 개발
- Machine Learning Developer (초기 단계)

---

## Tech Stack

### Currently Available Skills
> 프로젝트에서 실제로 사용한 기술 중심

| 분야 | 기술 |
|------|------|
| 언어 | Python |
| ML / 데이터 | NumPy, Pandas, Scikit-learn(기초), 데이터 전처리 및 EDA |
| LLM 파이프라인 | LangChain 기반 LLM 파이프라인 구성, OpenAI API |
| RAG 구성 | 문서 임베딩 생성(OpenAI), 검색 기반 RAG 구조 설계 |
| 개발 환경 | Git, GitHub, Colab, Jupyter |

### Learning & Upcoming Skills
> 학습 및 실습을 통해 확장 중인 기술 영역

| 분야 | 기술 |
|------|------|
| Backend (REST API) | FastAPI, Spring Boot (모델 추론 API 구성 및 연동 경험) |
| LLM Orchestration | LangGraph |
| Vector Store | FAISS, Chroma |
| 멀티모달 | 이미지 + 텍스트 입력 처리 |
| Speech | TTS 활용 |
| 딥러닝 | PyTorch |
| 배포 / 환경 | Docker, 간단한 클라우드 배포 |
| MLOps | 모델 서빙, 파이프라인 자동화 |
| DB | 기초 SQL |

---

## Key Strengths

- LangChain/LangGraph 기반 파이프라인 설계 경험
- 전처리, 임베딩, 검색 기반 RAG 구성 경험
- 멀티모달/Agent 기반 서비스 구조 설계 경험 (학습 및 실습 중심)

---

## Education & Certifications (Preparing)

- KT Aivle School 8기 수료(AI Track)
- AICE Associate(2025.02)
- TOEIC Speaking: IM2 (2025.03)
- 정보처리기사 — 2026 상반기 예정

---

> 본 프로젝트들은 팀 실습 및 개인 학습을 통해 구현한 결과물이며, 각 Repository는 제가 담당하거나 학습 과정에서 직접 설계·구현한 부분을 중심으로 정리했습니다.

---

## Projects

> 아래 프로젝트들은 학습 및 실습 목적의 프로젝트로, 각각 특정 기능이나 구조에 초점을 두고 구현했습니다.
> 모든 기능을 완전 자동화하거나 상용 수준으로 구현한 것은 아닙니다. 각 Repository는 단계적으로 업데이트될 예정입니다.

---

### 1) LangChain 기반 PPT → 강의 자동 생성 Agent

PPT 파일을 입력하면 슬라이드 분석부터 설명 스크립트 및 음성 강의까지 자동 생성하는 AI Agent

- **Category**: LLM Agent / Multimodal
- **Tech**: LangChain, LangGraph(OpenAI API), Python, TTS
- **Highlights**
  - 슬라이드 단위 상태(State) 관리
  - 텍스트 + 이미지 멀티모달 입력 처리
  - LangChain/LangGraph 기반 Agent 구조

👉 [프로젝트 상세: AI Lecture Agent Repository](https://github.com/kang-y-j/kt20250924-1)

---

### 2) LLM 기반 AI 면접관 Agent

이력서를 기반으로 질문을 생성하고 답변을 평가하여 후속 질문을 결정하는 인터뷰 Agent

- **Category**: LLM Agent / RAG
- **Tech**: LangChain, LangGraph, ChromaDB, OpenAI API, Python
- **Highlights**
  - 질문 전략(question strategy) 설계
  - 답변 점수 기반 인터뷰 분기 로직
  - RAG를 활용한 맥락 유지 질문 생성

👉 [프로젝트 상세: AI Interview Agent Repository](https://github.com/kang-y-j/ai-interview-agent)

---

### 3) EV Charger Ops Platform — 전기차 충전소 통합 관제 시스템

센서 데이터와 이미지를 AI로 분석해 충전기 이상을 감지하고, 운영자에게 자동 알림을 발송하는 충전소 관리 플랫폼

- **Category**: AI Integration / Backend / Monitoring
- **Tech**: Spring Boot, FastAPI, LangChain, LightGBM, WebClient, AWS S3, JPA
- **Team**: 8명
- **담당**: Backend(세션 기반 로그인/인증 구현), LightGBM 이상 예측 모델 개발, FastAPI 연동, 멀티모달 AI 분석 파이프라인 설계
- **Highlights**
  - 세션 기반 로그인 / 인증 필터 구현 (Spring Security)
  - 센서 로그 + 충전기 이미지 결합 멀티모달 AI 분석 파이프라인 설계
  - LightGBM 기반 충전기 이상 예측 모델 학습 및 FastAPI 연동
  - 화재 / 파손 / 오염 여부 자동 판별 → 실시간 모니터링 API 구현
  - 이상 감지 시 운영사 이메일 자동 발송 기능 연동

👉 [프로젝트 상세: EV Charger Ops Platform Repository](https://github.com/kang-y-j/ev-charger-ops-platform)


### 4) 전주시 생활 편의시설 지도 시각화

전주시 공공데이터를 활용해 버스정류장·도시공원·공영주차장을 한 화면에서 탐색할 수 있는 인터랙티브 지도 웹 애플리케이션

- **Category**: GIS / 공공데이터 / Web
- - **Tech**: Python, FastAPI, Pandas, Leaflet.js, HTML/CSS/JS
  - - **Highlights**
    -   - 전주시 공공데이터 전처리 및 인코딩 변환 파이프라인 구축
        -   - Geolocation API 기반 내 위치 감지 및 반경 필터링 (1/5/10km)
            -   - OSM Nominatim API 활용 주소 지오코딩
                -   - Railway 클라우드 배포
                    -
                    👉 [프로젝트 상세: jeonju_map Repository](https://github.com/kang-y-j/jeonju_map) | [배포 URL](https://web-production-de371.up.railway.app/)

                    ---
                    ---

## Contact

- **Email**: kfccckyj@naver.com
- **GitHub**: [https://github.com/kang-y-j](https://github.com/kang-y-j)

---

*Thanks for visiting my Portfolio!*
