# 📄 [웹 애플리케이션 프로젝트 기획 및 기술 명세서]

---

## 1. 프로젝트 개요

| 항목 | 내용 |
|:---|:---|
| 프로젝트명 | 예: 쇼핑몰 주문 관리 시스템 (ShoppingMall Order System) |
| 개발 기간 | 예: 2025.05.01 ~ 2025.06.15 (약 6주) |
| 개발 인원 | 3명 (프론트엔드 1, 백엔드 1, 풀스택 1) |
| 주요 기술 | Java (Spring Boot), MySQL, React.js, AWS EC2 (배포) |

---

## 2. 기획 배경 및 목적

- **기획 배경**:  
  사용자 친화적인 웹 기반 쇼핑몰 주문/결제 시스템이 필요함.
- **목적**:  
  상품 조회, 장바구니, 주문, 결제까지 가능한 **풀스택 웹 시스템** 구현.  
  RESTful API를 통한 **백엔드와 프론트엔드 완전 분리 개발**.

---

## 3. 주요 기능

| 구분 | 기능 설명 |
|:---|:---|
| 사용자 | 회원가입, 로그인, 상품 검색, 장바구니, 주문 및 결제 |
| 관리자 | 상품 등록/수정/삭제, 주문 관리, 회원 관리 |
| 기타 | 반응형 웹 구현 (모바일/PC 대응) |

---

## 4. 기술 스택

| 구분 | 기술 |
|:---|:---|
| Frontend | React.js (Vite, Axios, Redux 사용 예정) |
| Backend | Java 17, Spring Boot 3, Spring Security, JWT 인증 |
| Database | MySQL 8.x, JPA (Hibernate ORM) |
| Server | AWS EC2 (Ubuntu), Nginx (Reverse Proxy) |
| Version Control | Git, GitHub |
| Build/Deploy | Docker, Jenkins (CI/CD 예정) |

---

## 5. 시스템 아키텍처

```
[React Frontend]  <--->  [Spring Boot Backend API]  <--->  [MySQL Database]
         ↓
     (AWS EC2 서버 배포)
```
- React는 Axios를 통해 Spring Boot 서버와 HTTP 통신 (REST API 호출)
- Spring Boot는 JPA로 DB (MySQL)와 통신
- EC2 서버에 프론트/백엔드 통합 배포

---

## 6. 데이터베이스 설계 (ERD 요약)

| 테이블 | 설명 |
|:---|:---|
| USERS | 사용자 정보 저장 (회원/관리자 구분) |
| PRODUCTS | 상품 정보 저장 |
| ORDERS | 주문 기록 저장 |
| ORDER_ITEMS | 주문 상세 (구매한 상품 목록) |
| CART | 장바구니 저장 |

---

## 7. API 명세 (간단 예시)

| Method | Endpoint | 설명 |
|:---|:---|:---|
| POST | /api/users/register | 회원가입 |
| POST | /api/users/login | 로그인 (JWT 발급) |
| GET | /api/products | 상품 목록 조회 |
| POST | /api/orders | 주문 생성 |
| GET | /api/orders/{id} | 주문 상세 조회 |

---

## 8. 개발 일정 (간단 예시)

| 주차 | 목표 |
|:---|:---|
| 1주차 | 환경 세팅 (Spring Boot + MySQL + React 초기 세팅) |
| 2~3주차 | 회원가입/로그인/상품 조회 기능 구현 |
| 4주차 | 장바구니/주문/결제 구현 |
| 5주차 | 관리자 기능 (상품 등록/삭제 등) |
| 6주차 | 최종 배포, 테스트, 발표 준비 |

---

## 9. 보안 및 성능 고려사항

- JWT를 이용한 사용자 인증 및 권한 관리
- Spring Security를 통한 API 보호
- Docker 컨테이너화로 빠른 배포 및 서버 관리
- Axios 인터셉터를 통한 토큰 자동 처리
- XSS/CSRF 등 보안 위협 대응

---

## 10. 기대 효과

- 실제 서비스를 설계하고 배포하는 경험 습득
- 프론트엔드-백엔드 완전 분리형 개발 경험
- AWS 배포 및 DevOps(CI/CD) 경험
- React + Spring Boot 실전 프로젝트 역량 강화

---

# ✅ 핵심 요약
> "Spring Boot + MySQL + React 조합으로  
> 회원가입, 로그인, 상품 조회/주문/결제 기능을 가진  
> **실전형 풀스택 웹 애플리케이션**을 만든다."

---

# 📌 추가
필요하면  
- **ERD(데이터베이스 테이블 관계도)** 샘플  
- **API 상세 명세서** (POST/GET 요청 body 샘플)  
- **프로젝트 폴더 구조 예시 (React + Spring Boot 통합)**  

**이것들도 만들어줄 수 있어!** 🔥

