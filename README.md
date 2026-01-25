<h1 align="center">강영재 | AI Service Engineer Portfolio</h1>

<p align="center">
  LLM · RAG · LangChain · Python 기반 AI 서비스 개발을 목표로 학습하고 있습니다.  
  데이터를 분석하고, 모델을 실제 서비스 흐름에 연결하여 실질적인 가치를 만드는 것을 목표로 합니다.
</p>

---

## About Me
AI 기능을 활용한 서비스 개발에 흥미를 가지고 있으며  
LangChain과 Python 중심으로 LLM 기반 시스템을 직접 설계·구현해왔습니다.  
이 GitHub는 제가 학습한 내용과 성장 과정을 기록하는 공간으로,  
AI 서비스 엔지니어로 성장하기 위한 다양한 실험과 프로젝트를 포함합니다.

---

## Career Interest
- AI Service Engineer  
- LLM / RAG 기반 서비스 개발  
- Machine Learning Developer (초기 단계)

---

## Tech Stack

<div style="display: flex; gap: 20px; width: 100%;">

  <div style="flex: 1;">
    <h3>Currently Available Skills</h3>
    <table>
      <tr><th>분야</th><th>기술</th></tr>
      <tr><td><b>언어</b></td><td>Python</td></tr>
      <tr><td><b>ML/데이터</b></td><td>Numpy, Pandas, Scikit-learn(기초), 데이터 전처리</td></tr>
      <tr><td><b>LLM 파이프라인</b></td><td>LangChain, LangGraph</td></tr>
      <tr><td><b>AI 기능</b></td><td>GPT-4o / GPT-mini API, Prompt Engineering</td></tr>
      <tr><td><b>RAG 구성</b></td><td>임베딩 생성(OpenAI), 간단한 RAG 구조 설계</td></tr>
      <tr><td><b>프로젝트 경험</b></td><td>AI 면접관 / RAG QA / 강의 자동 생성 Agent</td></tr>
      <tr><td><b>개발 환경</b></td><td>Git, GitHub, Colab, Jupyter</td></tr>
      <tr><td><b>멀티모달</b></td><td>이미지+텍스트 분석, TTS 활용</td></tr>
    </table>
  </div>

  <div style="flex: 1;">
    <h3>Learning & Upcoming Skills</h3>
    <table>
      <tr><th>분야</th><th>기술</th></tr>
      <tr><td><b>Vector Store</b></td><td>FAISS, Chroma</td></tr>
      <tr><td><b>Backend(API)</b></td><td>FastAPI, Flask</td></tr>
      <tr><td><b>딥러닝</b></td><td>PyTorch</td></tr>
      <tr><td><b>배포/환경</b></td><td>Docker, 간단한 클라우드 배포</td></tr>
      <tr><td><b>MLOps</b></td><td>모델 서빙, 파이프라인 자동화</td></tr>
      <tr><td><b>DB 기초</b></td><td>SQL</td></tr>
    </table>
  </div>

</div>

---

## Key Strengths
- LangChain/LangGraph 기반 파이프라인 설계  
- 전처리, 임베딩, 검색 기반 RAG 구성 경험  
- 멀티모달/Agent 기반 서비스 구현 역량

---

## Education & Certifications (Preparing)
- KT Aivle School 8기 (AI Track)  
- 빅데이터 분석기사 — 2026 상반기 예정  
- 정보처리기사 — 2026 상반기 예정

---

> 본 프로젝트들은 팀 실습 및 개인 학습을 통해 구현한 결과물이며,  
> 각 Repository는 제가 담당하거나 학습 과정에서 직접 설계·구현한 부분을 중심으로 정리했습니다.

# Projects  

아래 프로젝트들은 학습과 실습을 통해 단계적으로 구현한 작업들입니다.   
각 프로젝트는 기능 구현뿐 아니라, 구조 설계와 흐름 정리에 초점을 두고 정리했습니다.  
각 Repository는 단계적으로 업데이트될 예정입니다.

---

## 1) LangChain 기반 PPT → 강의 자동 생성 Agent
> PPT 파일을 입력하면 슬라이드 분석부터  
> 설명 스크립트 및 음성 강의까지 자동 생성하는 AI Agent

- **Category**: LLM Agent / Multimodal
- **Tech**: LangGraph, LangChain, OpenAI API, Python, TTS
- **Highlights**
  - 슬라이드 단위 상태(State) 관리
  - 텍스트 + 이미지 멀티모달 입력 처리
  - LangChain/LangGraph 기반 Agent 구조

👉 프로젝트 상세: [AI Lecture Agent Repository](https://github.com/kang-y-j/ai-lecture-agent)

---
## 2) LLM 기반 AI 면접관 Agent
> 이력서를 기반으로 질문을 생성하고  
> 답변을 평가하여 후속 질문을 결정하는 인터뷰 Agent

- **Category**: LLM Agent / RAG
- **Tech**: LangChain, LangGraph, ChromaDB, Python
- **Highlights**
  - 질문 전략(question strategy) 설계
  - 답변 점수 기반 인터뷰 분기 로직
  - RAG를 활용한 맥락 유지 질문 생성

👉 프로젝트 상세: 준비 중

---
## 3) AI 기반 도서 관리 & 표지 이미지 생성 웹 서비스
> 사용자가 도서를 등록하면  
> 책 설명을 기반으로 AI가 표지 이미지를 자동 생성하고  
> 개인 도서 정보를 관리할 수 있는 웹 서비스

- **Category**: AI Web Service / Backend 중심
- **Tech**
  - Backend: Spring Boot, Spring Data JPA, MySQL
  - Frontend: React
  - AI: OpenAI Image Generation API
  - Infra: AWS EC2, S3, CI/CD
- **Highlights**
  - 사용자–도서 간 연관관계 기반 REST API 설계
  - 도서 설명을 프롬프트로 활용한 AI 표지 이미지 생성
  - 생성된 이미지 메타데이터 DB 저장 및 재사용 구조 설계
  - 로컬(H2) → 운영(MySQL) 환경 마이그레이션 경험
  - AWS 기반 배포 및 CI/CD 파이프라인 구성 경험

👉 프로젝트 상세: 준비 중


## Contact
- Email: kfccckyj@naver.com  
- GitHub: https://github.com/kang-y-j

<br>

<p align="center"><b>Thanks for visiting my Portfolio!</b></p>
