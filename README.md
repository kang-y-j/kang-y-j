# 강영재 | AI Service Engineer Portfolio

> LLM · RAG · CrewAI · LangChain · Python 기반 AI 서비스 개발을 목표로 학습하고 있습니다.
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
| 배포 / 환경 | 간단한 클라우드 배포 |
| DB | 기초 SQL |

---

## Key Strengths

- LangChain/LangGraph 기반 파이프라인 설계 경험
- 전처리, 임베딩, 검색 기반 RAG 구성 경험
- CrewAI 멀티 에이전트 워크플로우 설계 및 구현 경험
- 멀티모달/Agent 기반 서비스 구조 설계 경험 (학습 및 실습 중심)

---

## Education & Certifications

- TOEIC Speaking: IM2 (2026.04)
- KT Aivle School 8기 수료(AI Track)
- AICE Associate(2026.02)
- 정보처리기사 — 필기 합격 (2025.06)

---

> 본 프로젝트들은 팀 실습 및 개인 학습을 통해 구현한 결과물이며, 각 Repository는 제가 담당하거나 학습 과정에서 직접 설계·구현한 부분을 중심으로 정리했습니다.

---

## Projects

> 아래 프로젝트들은 학습 및 실습 목적의 프로젝트로, 각각 특정 기능이나 구조에 초점을 두고 구현했습니다.

---

### 1) LangChain 기반 PPT → 강의 자동 생성 Agent

PPT 파일을 입력하면 슬라이드 분석부터 설명 스크립트 및 음성 강의까지 자동 생성하는 AI Agent

- **Category**: LLM Agent / Multimodal
- **Tech**: LangChain, LangGraph, OpenAI API, Python, TTS
- **Highlights**
  - 슬라이드 단위 상태(State) 관리
  - 텍스트 + 이미지 멀티모달 입력 처리
  - LangChain/LangGraph 기반 Agent 구조

👉 [프로젝트 상세: AI Lecture Agent Repository](https://github.com/kang-y-j/kt20250924-1)

---

### 2) LLM 기반 AI 면접관 Agent v1

이력서를 기반으로 질문을 생성하고 답변을 평가하여 후속 질문을 결정하는 인터뷰 Agent

- **Category**: LLM Agent / RAG
- **Tech**: LangChain, LangGraph, ChromaDB, OpenAI API, Python
- **Highlights**
  - 질문 전략(question strategy) 설계
  - 답변 점수 기반 인터뷰 분기 로직
  - RAG를 활용한 맥락 유지 질문 생성

👉 [프로젝트 상세: AI Interview Agent v1 Repository](https://github.com/kang-y-j/ai-interview-agent)

---

### 3) LLM 기반 AI 면접관 Agent v2 — CrewAI 멀티 에이전트로 고도화

v1의 단일 파이프라인을 CrewAI 멀티 에이전트로 고도화하고 Streamlit 웹 UI를 추가한 버전

- **Category**: Multi-Agent / RAG / Web UI
- **Tech**: CrewAI, LangChain, FAISS, OpenAI API, Streamlit, Python
- **v1 → v2 발전 포인트**

| | v1 | v2 |
|---|---|---|
| 아키텍처 | 단일 파이프라인 | 멀티 에이전트 |
| 이력서 분석 | 직접 입력 | RAG 자동 검색 |
| UI | 없음 (CLI) | Streamlit 웹 UI |
| 에이전트 수 | 1개 | 면접관 + 평가자 |

- **Highlights**
  - 이력서 PDF를 RAG로 벡터화하여 관련 내용 자동 검색
  - CrewAI 면접관 에이전트 → 질문 생성, 평가자 에이전트 → 답변 평가
  - Streamlit 웹 UI로 PDF 업로드부터 평가까지 한 화면에서 처리

👉 [프로젝트 상세: AI Interview Agent v2 Repository](https://github.com/kang-y-j/ai-interview-agent-v2)

---

### 4) EV Charger Ops Platform — 전기차 충전소 통합 관제 시스템

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

---

## Contact

- **Email**: kfccckyj@naver.com
- **GitHub**: https://github.com/kang-y-j

---

*Thanks for visiting my Portfolio!*
