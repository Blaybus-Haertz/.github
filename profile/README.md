# ✂️ 헤어색Chill...
![image](https://github.com/user-attachments/assets/186cc07a-365c-4ee6-85f4-428b9c107113)


## 🏆 2025 블레이버스 MVP 해커톤 개발 대회 맞춤형 헤어 컨설팅 예약 서비스 

### 📜 Contents
 1. [Overview](#-overview)
 2. [서비스 화면](#-서비스-화면)
 3. [주요 기능](#-기능)
 4. [개발 환경](#%EF%B8%8F-개발-환경)
 5. [시스템 아키텍처](#-시스템-아키텍처)
 6. [데이터베이스 설계도](#-데이터베이스-설계도)
 7. [기술 특이점](#-기술-특이점)
 8. [팀원 소개](#-팀원-소개)
 
## ✨ Overview
##### 🏆 개발 기간: 25.02.09 ~ 25.02.19
- 나에게 어울리는 헤어스타일을 찾는 일은 어려우며, 어떤 스타일이 내 얼굴형과 어울릴지 어떤 디자이너가 내 취향에 맞을지 고민이 많습니다.
- 또한, 바쁜 일정 속에서 미용실 방문이 어려운 경우도 많습니다. 그래서 우린 언제 어디서든 전문가의 컨설팅을 쉽게 받을 수 있는 서비스가 필요합니다.
- 따라서 헤어색chill은 원하는 스타일과 전문가를 빠르게 매칭하여 **대면/비대면 헤어 컨설팅**을 편리하게 예약할 수 있는 서비스입니다.


## ✨ 헤어색Chill의 사이트
##### 🏆 [사이트](https://blaybus-haertz.netlify.app/)


## ✨ 헤어색Chill의 소통 플랫폼 
##### 🏆 [노션_API 명세서](https://honeysuckle-mars-c88.notion.site/Blaybus-API-19955892b35e8077a31dffad665754b5?pvs=4)
##### 🏆 디스코드


## 👀 서비스 화면
### ✨ `모바일(아이폰 12 Pro 기준 max-width:480px)` 지원O

### 📹 [시연 영상](https://www.youtube.com/watch?v=UwCR5-vFiCY)

### 📄 [PPT](https://drive.google.com/file/d/1ibmfdnB7W1p3U8yaASYXRdMP1xR9DHB4/view?usp=drive_link)


### 🚀 스타일 컨설팅, 바로 시작!
  - 헤어스타일이 고민된다면? 전문가와 상담하고 바로 해결하세요!
  - 대면/비대면 선택 후 나에게 맞는 디자이너를 추천해 드립니다.
  - 예약 신청, 조회, 변경, 취소까지 한 번에!
  <br>📌 쉽고 직관적인 예약 시스템!
  <br>📌 대면/비대면 선택에 따른 맞춤 디자이너 추천
  <br>📌 신뢰할 수 있는 전문가들과의 컨설팅
  <br>
  <img src="https://github.com/user-attachments/assets/cf0d1d5e-bf2c-4d72-a33d-e629d0f92f54" width="200">  
  <br>

### ⏰ 내가 원하는 시간, 원하는 방식으로 바로 예약!
  - 터치 몇 번으로 손쉽게 예약
  - 대면/비대면 중 원하는 방식 선택
  <br>
  <img src="https://github.com/user-attachments/assets/fbdbfa0f-cab2-4856-9373-56c0648e20c2" width="200">
  <br>

### ✅ 복잡한 것들을 All 바로 
  - 가능한 시간을 자동으로 체크합니다.
  <br>
  <img src="https://github.com/user-attachments/assets/823347be-61f2-411e-98d6-8e11196858de" width="200">
  <br>

### ✨ 내 스타일에 맞는 디자이너를 자동 추천!
  - 대면/비대면 선택에 따라 최적의 디자이너 리스트업
  - 프로필,  포트폴리오를 확인하고 내게 맞는 디자이너 선택
  <br>
  <img src="https://github.com/user-attachments/assets/80b92593-b08c-4044-a675-895ba30415ae" width="200">  
  <br>


### 💳 안전한 결제 & 예약 관리
  - 계좌이제/간편결제 지원 (페이앱 연동 가능)
  - 결제 후 예약 확정 및 변경 가능
  - 비대면 컨설팅 선택 시 구글 미트 링크 자동 생성
  <br>
  <img src="https://github.com/user-attachments/assets/8047f98f-8187-45b8-aa5d-7d6342a5dafa" width="200">
  <img src="https://github.com/user-attachments/assets/9dbba19e-3671-45c9-9d49-07e5d845c1f1" width="200">  
  <br>


  
## ✨  기능 

 - `Google OAuth`
	- Refresh Token을 활용하여 Redis에 저장한 뒤 사용자 인증을 효율적으로 관리했습니다.
 
 - `예약 시스템`
	- 사용자는 원하는 디자이너, 시간대, 비대면/대면 여부를 선택하고 결제를 통해 예약할 수 있습니다.
	- 예약 조회, 예약 취소, 예약 생성 기능을 제공하며, 생성된 예약 시간은 다른 사용자가 선택할 수 없도록 제한했습니다.
 
 - `결제 시스템`
 	- 계좌이체 및 카카오페이를 활용한 결제 시스템을 구현했습니다.
	- 계좌이체의 경우 딥링크(Deep Link)를 활용하여 앱에서 결제를 진행할 수 있도록 했습니다.
 
 - `구글 미트 링크 생성`
 	- 사용자가 비대면으로 예약을 신청할 경우, 시스템에서 자동으로 구글 미트 링크를 생성하여 사용자에게 제공합니다.
 
 - `GPS 기능`
 	- 디자이너를 조회할 때 사용자의 현재 위치를 기준으로 가장 가까운 디자이너 리스트를 조회할 수 있도록 구현했습니다.
 
 - `로드밸런싱`
 	- 서버를 3대 증설하여 트래픽을 분산하는 환경을 구축했습니다.


## 🖥️ 개발 환경
**Management Tool**
- 형상 관리 : Git
- 커뮤니케이션 : Discord, Notion
- 디자인 : Figma

**🐳 Backend**
- Java `17.0.6`
- Spring Framework `3.2.4`

**🦊 Frontend**
-  React, TypeScript, CSS

**🗝️ API**
- Google(OAuth, Meet, MAP) API
- KakaoPay API
   
**🗂️ DB**
- MySQL `8.0.30`
- Redis
  
**🌐 Server**
- AWS EC2 (Ubuntu `20.04`)
- Nginx `1.23` (Reverse Proxy)
- HTTPS (TLS `1.2`)
- RDS, S3, LoadBalancing

**🔨 IDE**
- IntellJ `2023.2`

## 💫 시스템 아키텍처
![image](https://github.com/user-attachments/assets/8ad18949-7da0-40cb-979c-87a312fe590c)


## ✨ 데이터베이스 설계도
![image](https://github.com/user-attachments/assets/845a739e-52a1-456d-8e0d-6f6582dec331)


## ✨ 기술 특이점
- Feign Client를 활용하여 카카오페이 및 구글 미트 기능을 개발하였으며, 이를 통해 외부 API와의 통신을 간결하게 처리하였습니다.
- 구글 미트 링크 생성 과정에서 클라이언트와의 통신 중 미팅 시작 시간을 넘겨주는 startTime 부분에서 오류가 발생했습니다. 트러블슈팅 결과 30분 단위로 분절된 타임 테이블 특성 상 밀리초 부분에 들어가는 00.000000값이 Hibernate상에서 null로 처리되어 발생하는 오류였고, 이를 해결하기 위해 클라이언트 측에서 요청 시 밀리초 부분에 임의의 값을 추가하는 방식으로 수정하여 문제를 해결하였습니다.
- 구글 맵의 GPS 기능을 활용하여 사용자의 현재 위치를 기반으로 가장 가까운 디자이너 리스트를 조회할 수 있도록 구현하였습니다.
- 로드 밸런싱 기법을 적용하여 서버를 3대로 확장함으로써 부하를 분산시키고 안정적인 서비스 운영이 가능하도록 개선하였습니다.

# ❤️‍🔥 헤어색Chill 팀원 소개

## 🎯 PM (2명) 및 🎨 Designer (1명)

| **[안시환](https://github.com/shwnahn)** | **[이건희](https://github.com/leegh1025)** | **송연우** |
|:----------------------------------------:|:-------------------------------------:|:----------------------------------------:|
| ![안시환](https://github.com/user-attachments/assets/d8700eef-f4fb-4df6-8083-eaf23dff4f26)| ![이건희](https://github.com/user-attachments/assets/56027870-cc6c-4947-ba84-c6b05fb07396)|![송연우](https://github.com/user-attachments/assets/9404ef3e-0e3d-4737-a14e-993333f94cd3)|
| **Leader & PM** | **PM** | **Designer** |

### 팀원 역할
- **안시환** : 팀장, 프로젝트 기획, 상담, 최종 발표 진행
- **이건희** : 프로젝트 기획, 상담
- **송연우** : UI/UX 디자인, PPT 제작

---

## 🎭 Frontend Developers (2명)

| **[이지현](https://github.com/ljh130334)** | **[장지요](https://github.com/wldy4627)** |
|:----------------------------------------:|:-------------------------------------:|
| ![이지현](https://github.com/user-attachments/assets/932ac1ec-514b-416a-8b2b-359c2b7d1b30)| ![장지요](https://github.com/user-attachments/assets/14ae8f27-93b9-44fe-8080-8a147ab89498)|
| **Leader & Frontend Developer** | **Frontend Developer** |

### 팀원 역할
- **이지현** : 프론트엔드 팀장, 페이지 설계, API 응답 처리
- **장지요** : 페이지 설계, API 응답 처리

---

## ⚙ Backend Developers (4명)

| **[김동욱](https://github.com/lian2945)** | **[김민수](https://github.com/devkev00)** | **[유승주](https://github.com/touhou09)** | **[최승호](https://github.com/chltmdgh522)** |
|:----------------------------------------:|:-------------------------------------:|:-------------------------------------:|:-------------------------------------:|
| ![김동욱](https://github.com/user-attachments/assets/325fc6e8-328e-41eb-810d-514a6e6b67e0)| ![김민수](https://github.com/user-attachments/assets/2497f24c-ee8d-40c1-af38-5bd930986c41)| ![유승주](https://github.com/user-attachments/assets/22f13960-2e74-412d-964a-7c5c53052a25)| ![최승호](https://github.com/user-attachments/assets/92d23704-bb2d-47ca-967e-6f3b6afebd95)|
| **Leader & Backend Developer** | **Backend Developer** | **Backend Developer** | **Backend Developer** |

### 팀원 역할
- **김동욱** : 백엔드 팀장, 서버 최적화, GPS 개발, Google OAuth 토큰 개발
- **김민수** : 구글 미트 API 개발, 예약 시스템 API 개발, 서버 최적화
- **유승주** : 예약 시스템 API 개발
- **최승호** : 예약 생성 및 타임 테이블 API 개발, 카카오페이 개발, 서버 최적화 
