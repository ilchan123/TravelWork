# 🌍 TravelWork App

> **원격 근무자를 위한 여행 및 업무 관리 애플리케이션**  
> 여행하면서 업무를 효율적으로 관리할 수 있도록 도와주는 웹 및 모바일 앱입니다.

[![GitHub Repo](https://img.shields.io/badge/GitHub-TravelWork-blue?style=flat&logo=github)](https://github.com/ilchan123/TravelWork)

---

## 📌 프로젝트 개요
**TravelWork**는 디지털 노마드와 원격 근무자를 위한 여행 및 업무 관리 도구입니다.  
사용자는 여행 일정을 관리하고, 업무를 정리하며, 협업 기능을 활용할 수 있습니다.

## 🚀 주요 기능
- **여행 일정 관리**: 여행 경로 및 계획 설정
- **업무 관리**: 할 일 목록, 일정, 미팅 관리
- **팀 협업 기능**: 공유 일정 및 채팅
- **지도 및 장소 추천**: 여행지 기반 추천 시스템
- **다크 모드 지원**: 사용자 경험 향상

---

## 🛠 기술 스택
- **Frontend**: React.js / React Native  
- **Backend**: Node.js (Express.js)  
- **Database**: PostgreSQL / MongoDB  
- **Authentication**: JWT (JSON Web Token)  
- **Cloud Storage**: Firebase / AWS S3  
- **API**: OpenAI API (추천 시스템), Google Maps API  

---

## 📂 폴더 구조
TravelWork/ 
│── frontend/ # 프론트엔드 React 코드 
│── backend/ # 백엔드 Express API
│── database/ # 데이터베이스 스키마 및 초기 데이터
│── config/ # 환경 설정 파일 
│── components/ # 재사용 가능한 UI 컴포넌트
│── routes/ # API 라우팅 설정 
│── middleware/ # 인증 및 보안 미들웨어 
│── assets/ # 이미지 및 정적 파일
│── README.md # 프로젝트 문서
│── package.json # 프로젝트 의존성 관리 파일
│── .env.example # 환경 변수 예시 파일

---

## 📦 설치 방법
### 1️⃣ 백엔드 실행
```bash
# 리포지토리 클론
git clone https://github.com/ilchan123/TravelWork.git
cd TravelWork/backend

# 패키지 설치
npm install

# 환경 변수 설정 (.env 파일 필요)
cp .env.example .env

# 서버 실행
npm start
2️⃣ 프론트엔드 실행

cd ../frontend

# 패키지 설치
npm install

# 개발 서버 실행
npm start
⚙️ API 엔드포인트
기능	메서드	엔드포인트	설명
회원가입	POST	/auth/signup	사용자 회원가입
로그인	POST	/auth/login	사용자 로그인
여행 일정 생성	POST	/trips	새로운 여행 일정 추가
여행 일정 조회	GET	/trips/:id	특정 여행 일정 조회
할 일 추가	POST	/tasks	업무 목록에 새로운 할 일 추가
할 일 조회	GET	/tasks/:id	특정 할 일 조회
채팅 메시지	POST	/chat/send	실시간 채팅 메시지 전송
