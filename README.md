# 📖  **StoryTeller**

### 아이맞춤형 AI 동화 생성 및 리딩 서비스

**StoryTeller**는 LLM과 생성형 AI를 활용하여 **아이 맞춤형 동화 생성·삽화·리딩 서비스**를 제공하는  플랫폼입니다.

 입력한 이름, 나이, 장르를 기반으로 동화를 자동으로 생성하고, LoRA 기반 Stable Diffusion으로 삽화를 만들며, ElevenLabs API를 통해 입력한 목소리로 동화를 읽어줍니다.

---

# 프로젝트 메인사진

### 📍 **StoryTeller-Backend**

StoryTeller-Backend는 FastAPI 기반으로 구축된 백엔드 시스템으로, **동화 생성, 품질 평가, 요약, 이미지 생성, 오디오 생성** 등 전체 AI 파이프라인을 관리합니다.

**주요 기능**:

- **동화 생성**: QLoRA Fine-Tuned LLM으로 맞춤형 동화 생성
- **스토리 평가**: LoRA Fine-Tuned LLM을 통해 품질 자동 평가
- **스토리 요약**: 페이지 단위 요약으로 삽화 생성 프롬프트 최적화
- **삽화 생성**: Stable Diffusion + LoRA로 동화 분위기에 맞는 이미지 생성
- **TTS 리딩**: ElevenLabs API로 부모 목소리 기반 오디오 스트리밍
- **DB 관리**: MySQL에 동화/이미지/오디오/로그 저장 및 이어듣기 지원

**추가 설명**:

- **데이터 관리**: 생성된 동화, 이미지, 오디오를 DB에 저장 및 검색 가능
- **모델 학습 및 추론**: QLoRA/LoRA를 활용해 모델 최적화 가능
- **스트리밍**: 오디오 파일을 페이지 단위로 실시간 제공

---

### 📍 **StoryTeller-FE**

StoryTeller-FE는 React + TypeScript 기반으로 개발된 프론트엔드로, **사용자 친화적인 동화 생성·시청각 경험**을 제공합니다.

**주요 기능**:

- **동화 생성 UI**: 이름·나이·장르 입력 기반 동화 생성 요청
- **실시간 시각화**: 생성된 동화, 삽화, 오디오를 직관적으로 확인 가능
- **API 연동**: ngrok을 통한 백엔드 연결 및 실시간 데이터 반영
- **데이터 관리**: 사용자별 생성 기록 조회 및 이어듣기 기능 제공

**추가 설명**:

- **반응형 UI**: 다양한 디바이스(모바일/PC)에서 최적화
- **UX 강화**: 페이지 단위 동화 읽기 및 이어듣기 지원

---

# **시스템 구성 및 아키텍처**
<img width="500" height="657" alt="스크린샷 2025-08-20 19 59 32" src="https://github.com/user-attachments/assets/f7f20d4b-339f-43bd-abfb-43660eb08c19" />



---

# **🛠️ 기술 스택**

| **Frontend**       |  **Backend**     | **AI**     | **Database**     | **TTS**     | **server**     |
|------------|--------------|--------------|--------------|--------------|--------------|
| [![My Skills](https://skillicons.dev/icons?i=react)](https://skillicons.dev) | [![My Skills](https://skillicons.dev/icons?i=fastapi)](https://skillicons.dev) | [![My Skills](https://skillicons.dev/icons?i=pytorch)](https://skillicons.dev) <img width="50" height="50" alt="스크린샷 2025-08-20 20 08 26" src="https://github.com/user-attachments/assets/e660b773-7cf3-484c-878b-afa4eb04356d" /> | [![My Skills](https://skillicons.dev/icons?i=mysql)](https://skillicons.dev) | <img width="70" height="50" alt="스크린샷 2025-08-20 20 11 41" src="https://github.com/user-attachments/assets/5e12cede-e606-40cb-84f5-60509bc6517f" />  | <img width="70" height="50" alt="스크린샷 2025-08-20 20 13 39" src="https://github.com/user-attachments/assets/a556b245-af0b-48eb-ae35-5d2feaeedc4e" /> | 
