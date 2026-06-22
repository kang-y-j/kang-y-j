# 강영재 | AI Service Engineer Portfolio

> LLM · RAG · LangChain · Python 기반 AI 서비스를 설계하고 구현합니다.
> 데이터를 분석하고 모델을 실제 서비스 흐름에 연결해, 실질적인 가치를 만드는 것을 목표로 합니다.

---

## About Me

AI 기능을 활용한 서비스 개발에 흥미를 가지고 있으며, LangChain과 Python을 중심으로 LLM 기반 서비스 흐름을 직접 설계하고 구현해왔습니다.
이 GitHub는 제가 학습한 내용과 성장 과정을 기록하는 공간으로, AI 서비스 엔지니어로 성장하기 위한 다양한 실험과 프로젝트를 담고 있습니다.

---

## Career Interest

- AI Service Engineer
- LLM / RAG 기반 서비스 개발
- LLM Agent 설계 및 운영

---

## Tech Stack

### Currently Available Skills
> 프로젝트에서 실제로 사용한 기술 중심

| 분야 | 기술 |
| --- | --- |
| 언어 | Python |
| ML / 데이터 | NumPy, Pandas, Scikit-learn(기초), LightGBM, 데이터 전처리 및 EDA |
| LLM 파이프라인 | LangChain · LangGraph 기반 파이프라인 구성, OpenAI API |
| LLM Agent | CrewAI 기반 멀티 에이전트 구조 설계 |
| RAG 구성 | 문서 임베딩 생성(OpenAI), FAISS / ChromaDB 기반 검색 RAG 설계 |
| Backend | FastAPI 기반 모델 서빙 API 구성 및 배포 경험 |
| 개발 환경 | Git, GitHub, Colab, Jupyter, Hugging Face Spaces |

### Learning & Upcoming Skills
> 학습 및 실습을 통해 확장 중인 기술 영역

| 분야 | 기술 |
| --- | --- |
| 멀티모달 | 이미지 + 텍스트 입력 처리 |
| Speech | TTS 활용 |
| 딥러닝 | PyTorch |
| 배포 / 환경 | Docker, 클라우드 배포 |
| MLOps | 모델 서빙, 파이프라인 자동화 |
| DB | 기초 SQL |

---

## Key Strengths

- LangChain / LangGraph / CrewAI 기반 LLM Agent 파이프라인 설계 경험
- 전처리, 임베딩, 검색 기반 RAG 구성 및 할루시네이션 개선 경험
- LightGBM 기반 이상 예측 모델 개발 및 성능 최적화 경험

---

## Education & Certifications

- 정보처리기사 (2026.06)
- TOEIC Speaking: IM2 (2026.04)
- KT AIVLE School AI개발자 트랙 수료 (2026.03)
- KT AIVLE School BIG Project 우수상 (2026.03)
- AICE Associate (2026.02)


---

> 아래 프로젝트는 팀 실습 및 개인 학습을 통해 구현한 결과물이며,
> 각 Repository는 제가 직접 담당하거나 설계·구현한 부분을 중심으로 정리했습니다.

---

## Projects

> 학습 및 실습 목적의 프로젝트로, 각각 특정 기능과 구조에 초점을 두고 구현했습니다.
> 일부는 상용 수준이 아닌 실험 단계이며, 각 Repository는 단계적으로 업데이트됩니다.

---

### 1) LLM 기반 AI 면접관 Agent

이력서를 기반으로 질문을 생성하고 답변을 평가하여 후속 질문을 결정하는 인터뷰 Agent.
초기 단일 파이프라인(v1)에서 멀티 에이전트 구조(v2)로 발전시키며 질문 품질과 답변 해석 정확도를 개선했습니다.

- **Category**: LLM Agent / RAG
- **Tech**: LangChain, CrewAI, FAISS, OpenAI API, FastAPI, Python
- **Highlights**
  * 질문 생성 에이전트와 답변 평가 에이전트를 CrewAI로 분리해 질문 품질 안정화
  * 이력서 PDF를 FAISS로 벡터화해 질문 근거를 확보, 할루시네이션 개선
  * FastAPI 백엔드로 분리해 Hugging Face Spaces에 배포, 현재도 운영 중

👉 [프로젝트 상세: AI Interview Agent Repository](https://github.com/kang-y-j/ai-interview-agent)

---

### 2) LangChain 기반 PPT → 강의 자동 생성 Agent

PPT 파일을 입력하면 슬라이드 분석부터 설명 스크립트 및 음성 강의까지 자동 생성하는 AI Agent.

- **Category**: LLM Agent / Multimodal
- **Tech**: LangChain, LangGraph, OpenAI API, Python, TTS
- **Highlights**
  * 슬라이드 단위 상태(State) 관리
  * 텍스트 + 이미지 멀티모달 입력 처리
  * LangGraph 기반 Agent 흐름 제어

👉 [프로젝트 상세: AI Lecture Agent Repository](https://github.com/kang-y-j/kt20250924-1)

---

### 3) EV Charger Ops Platform — 전기차 충전소 통합 관제 시스템

센서 데이터와 이미지를 AI로 분석해 충전기 이상을 감지하고, 운영자에게 자동 알림을 발송하는 충전소 관리 플랫폼. (KT AIVLE School BIG Project, 우수상 수상 / 8인 팀 프로젝트)

- **Category**: AI / Machine Learning / Monitoring
- **Team**: 8명
- **담당**: LightGBM 이상 예측 모델 개발 및 성능 최적화
- **Highlights**
  * 정상 데이터가 많은 불균형 상황에서 단계적 피처 엔지니어링 적용
  * Optuna 기반 하이퍼파라미터 최적화 및 Early Stopping 적용
  * 불균형 데이터 환경에서 Macro F1 0.93 달성
  * 학습한 모델을 충전기 이상(화재/파손/오염) 자동 판별에 활용

👉 [프로젝트 상세: EV Charger Ops Platform Repository](https://github.com/kang-y-j/ev-charger-ops-platform)

---

## Contact

- **Email**: kfccckyj@naver.com
- **GitHub**: https://github.com/kang-y-j

---

*Thanks for visiting my Portfolio!*
