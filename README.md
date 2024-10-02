# 📦 TeamCostco SYSTEM README

<img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/%EB%AC%BC%EB%A5%98%20%ED%9A%8C%EC%82%AC_.jpg?raw=true" width="500" height="400"/> 

- 배포 URL : http://15.165.19.189
- Test ID : test  
- Test PW : 1234

## 프로젝트 소개

- Costco의 물류 프로세스를 혁신하고 효율성을 극대화하기 위한 종합적인 관리 시스템 개발 프로젝트
- 실시간 재고관리부터 주문 처리, 데이터 분석, 창고 관리, 간편 발주까지 가능한 시스템
- 운영 비용 절감과 주문 처리시간 단축, 재고 회전율 개선이 가능한 시스템

## 팀원 구성

| 강동윤 | 김동민 | 주형돈 | 김동우 |
|:------:|:------:|:------:|:------:|
| <img src="https://avatars.githubusercontent.com/u/173039221?v=4" width="50" height="50"/> <br> [@KangDY26](https://github.com/KangDY26) | <img src="https://avatars.githubusercontent.com/u/173039024?v=4" width="50" height="50"/> <br> [@uiwoowP](https://github.com/uiwoowP) | <img src="https://avatars.githubusercontent.com/u/173039030?v=4" width="50" height="50"/> <br> [@hdjoo0820](https://github.com/hdjoo0820) | <img src="https://avatars.githubusercontent.com/u/173039738?v=4" width="50" height="50"/> <br> [@DukkyRacoon](https://github.com/DukkyRacoon) |

| 전상민 | 이신비 | 오혜준 | 김민수 |
|:------:|:------:|:------:|:------:|
| <img src="https://avatars.githubusercontent.com/u/68059753?v=4" width="50" height="50"/> <br> [@jsm3794](https://github.com/jsm3794) | <img src="https://avatars.githubusercontent.com/u/173039141?v=4" width="50" height="50"/> <br> [@SHINBI116](https://github.com/SHINBI116) | <img src="https://avatars.githubusercontent.com/u/173116759?v=4" width="50" height="50"/> <br> [@Oh-hyejun](https://github.com/Oh-hyejun) | <img src="https://avatars.githubusercontent.com/u/131967955?v=4" width="50" height="50"/> <br> [@gopo543](https://github.com/gopo543) |

## 1. 개발 환경

- Front-end : HTML, CSS, JavaScript
- Back-end : Java, Spring Boot, Naver API, Google Pub/Sub API, Oracle SQL Developer
- 버전 및 이슈관리 : Github, Github Issues, Github Project
- 협업 툴 :  Slack, Notion, Figma
- 서비스 배포 환경 :

## 2. 채택한 개발 기술과 전략

### Front-end 기술

- **HTML, CSS, JavaScript**
  - 웹 페이지의 구조와 스타일을 정의하기 위해 사용되었습니다. 
  - 사용자 경험을 향상시키기 위해 반응형 웹 디자인을 적용했습니다. 

### Back-end 기술

- **Java, Spring Boot**
  - 안정적이고 확장 가능한 서버 사이드 애플리케이션 개발을 위해 선택했습니다.
  - RESTful API를 통해 클라이언트와의 효율적인 데이터 통신을 구현했습니다.

- **Naver API, Google Pub/Sub API**
  - 외부 서비스와의 연동을 통해 기능을 확장했습니다.
  - 데이터 전송 및 메시징 서비스를 구현하여 시스템 간 통신을 원활히 했습니다.

- **Oracle SQL Developer**
  - 데이터베이스 관리 및 쿼리 작성을 위해 사용했습니다.
  - 데이터 모델링과 성능 최적화를 통해 데이터 처리를 효율적으로 진행했습니다.

### 버전 및 이슈 관리

- **GitHub, GitHub Issues, GitHub Projects**
  - 팀원 간의 협업을 위한 코드 버전 관리와 이슈 추적을 위해 사용했습니다.
  - 프로젝트 진행 상황을 시각적으로 관리하여 팀의 생산성을 높였습니다.

### 협업 툴

- **Slack, Notion, Figma**
  - Slack: 팀 간의 원활한 소통을 위한 채팅 플랫폼입니다.
  - Notion: 프로젝트 문서화 및 아이디어 정리를 위해 활용했습니다.
  - Figma: UI/UX 디자인 작업을 위한 협업 툴로 사용했습니다.

## 3. 프로젝트 구조
```
teamcostco
├── .mvn
│    └── maven-wrapper.properties
│
├── src
│    └── main
│          ├── java
│          │    ├── config
│          │    │      ├── BcryptUtils.java
│          │    │      └── WebSocketConfig.java
│          │    │
│          │    ├── controller
│          │    │      ├── BoardController.java
│          │    │      ├──    .
│          │    │      ├──    .
│          │    │      └── BoardFixController.java
│          │    │
│          │    ├── dto
│          │    │      ├── category
│          │    │      │       ├── CategoryDTO.java
│          │    │      │       ├──   .
│          │    │      │       ├──   .
│          │    │      │       └── CategoryResponse.java
│          │    │      │
│          │    │      ├── employee
│          │    │      │       └── EmployeeDTO.java
│          │    │      ├──    .
│          │    │      ├──    .
│          │    │      └── login
│          │    │              └── LoginRequestDTO.java
│          │    │
│          │    ├── pagination
│          │    │      ├── PageDetails.java
│          │    │      ├── PaginationRepository.java
│          │    │      └── PaginationResult.java
│          │    │
│          │    ├── repository
│          │    │      ├── NoticeRepository.java
│          │    │      ├──    .
│          │    │      ├──    .
│          │    │      └── WritingRepository.java
│          │    │
│          │    ├── service
│          │    │      ├── CategoryService.java
│          │    │      ├──    .
│          │    │      ├──    .
│          │    │      └── JoinService.java
│          │    │
│          │    ├── websocket
│          │    │      └── NotificationHandler.java
│          │    │
│          │    ├── PageMetadataProvider.java
│          │    ├── S3Config.java
│          │    ├── ServletInitializer.java
│          │    └── TeamcostcoApplication.java
│          │
│          └── resources
│               ├── mapper
│               │      ├── find_mapper.xml
│               │      ├──    .
│               │      ├──    .
│               │      └── products_mapper.xml
│               │
│               ├── static
│               │      ├── css
│               │      │    ├── common
│               │      │    │      ├── theme.css
│               │      │    │      ├── .
│               │      │    │      ├── .
│               │      │    │      └── header.css
│               │      │    │      
│               │      │    ├── component
│               │      │    │      ├── filter.css
│               │      │    │      ├── .
│               │      │    │      ├── .
│               │      │    │      └── search.css
│               │      │    │      
│               │      │    └── contents
│               │      │           ├── inventory.css
│               │      │           ├── .
│               │      │           ├── .
│               │      │           └── notice.css
│               │      │    
│               │      ├── fonts
│               │      │     └── Material_···.woff2
│               │      ├── images
│               │      │    ├── logo-dark.png
│               │      │    ├── .
│               │      │    ├── .
│               │      │    └── profile-default.svg
│               │      │           
│               │      ├── js
│               │      │    ├── common
│               │      │    │      ├── header.js
│               │      │    │      ├── .
│               │      │    │      ├── .
│               │      │    │      └── main.js
│               │      │    │
│               │      │    ├── component
│               │      │    │      ├── filter.js
│               │      │    │      ├── .
│               │      │    │      ├── .
│               │      │    │      └── search.js
│               │      │    │      
│               │      │    ├── contents
│               │      │    │      ├── writer.js
│               │      │    │      ├── .
│               │      │    │      ├── .
│               │      │    │      └── fix.js
│               │      │    │      
│               │      │    └── tinymce
│               │      │           ├── icons
│               │      │           ├── .
│               │      │           ├── .
│               │      │           └── skins
│               │      │    
│               │      └── favicon.ico
│               │
│               ├── templates
│               │      ├── common
│               │      ├── .
│               │      ├── .
│               │      └── index.html
│               │
│               ├── application.properties
│               ├── ezen-project···.json
│               ├── log4jdbc.log4j2.properties
│               ├── logback-spring.xml
│               ├── mybatis-config.xml
│               └── spy.properties
│
├── target
│    ├── classes
│    └── generated-sources
│
├── .gitignore
├── mvnw
├── mvnw.cmd
└── pom.xml
```

## 4. 역할 분담

### 📊강동윤
- **UI**
  - 페이지: 상품발주, 배송 현황
  - 공통 컴포넌트: 테이블, 필터
- **기능**
  - 네이버 API연동 검색 기능 구현, 발주 기능 구현, 배송 현황 정보 서버 연결과 구현

### ✏️김동민
- **UI**
  - 페이지: 재고관리, 재고관리 상세
  - 공통 컴포넌트: 네비게이터
- **기능**
  - 박스 / 테이블 내의 정보 서버 연결과 구현, 재고 수정 과 저장 기능 구현

### 🗂️주형돈
- **UI**
  - 페이지: 다크모드
  - 공통 컴포넌트: 검색창
- **기능**
  - 전체 페이지 다크모드 활성화, 비활성화 구현

### 🔍김동우
- **UI**
  - 페이지: 직원관리 상세, 로그인
- **기능**
  - tiny MCE에디터 api 연동 글 작성, 수정, 삭제 기능 구현, 직원 정보 수정 기능 구현
- **DB 관리**
  - 각종 테이블, 컬럼, 제약 조건 등 전반적인 DB 정보 관리  
 
### 🗒️전상민
- **UI**
  - 페이지: 회원가입, 직원관리, 공지사항
  - 공통 컴포넌트: 카카오 API연동(주소 찾기)
  - 로고 디자인
- **기능**
  - 인적사항, 주소, 중복 확인 등 유효성 검사와 서버 연결 작업, id, pw 찾기 이메일 서비스, 

### 🤝이신비
- **UI**
  - 페이지: 발주관리, 발주관리 상세
  - 공통 컴포넌트: 페이지네이션 기능&버튼
- **기능**
  - 박스 / 테이블 내의 정보 서버 연결과 구현, 발주 처리 기능 구현

### 💼오혜준
- **UI**
  - 페이지: 판매내역, 판매 내역 상세
  - 공통 컴포넌트: 인포박스
- **기능**
  - 박스 / 테이블 내의 정보 서버 연결과 구현

### 📅김민수
- **UI**
  - 페이지: 대시보드, 불량재고
  - 공통 컴포넌트: 헤더
- **기능**
  - 차트 구현, 박스 / 테이블 내의 정보 서버 연결과 구현

## 5. 개발 기간 및 작업 관리

### 개발 기간
- 전체 개발 기간: 2024-08-19 ~ 2024-10-..

### 작업 관리
- Slack, 노션을 사용하여 진행 상황을 공유했습니다. 
- 주간회의를 진행하며 작업 순서와 방향성에 대한 고민을 나누고 Slack에 회의 내용을 기록했습니다.

## 6. 페이지별 기능 

## 로그인 페이지

### [로그인] 

- 아이디와 비밀번호를 입력하면 유효성 검사가 진행되고 통과한 경우 로그인에 성공합니다.

| 로그인 |
|--------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/1_%EB%A1%9C%EA%B7%B8%EC%9D%B8.gif?raw=true" width="850" height="600"/> |

## 대시보드 페이지

### [대시보드]
- 사용자가 기간별 판매 금액, 최다 판매 제품, 판매 대비 재고 비율, 최다 발주 제품 등 많은 정보들을 한눈에 파악할 수 있습니다.
- 필요한 정보들을 1주, 1개월, 1년 단위로 확인할 수 있어 더욱 정보를 확인하기 쉽습니다.

| 정보 확인 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/2_%EB%8C%80%EC%8B%9C%EB%B3%B4%EB%93%9C.gif?raw=true" width="850" height="600"/> |

## 재고 관리 페이지

### [필터]
- 상품코드, 매입가격, 판매가격, 대분류 등
  사용자가 원하는 검색옵션을 지정해 필터를 걸어줄 수 있습니다.
- 필터 적용 후 검색 시 지정된 검색 옵션에 맞는 값이 표시 됩니다.

| 필터 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/3_%EC%9E%AC%EA%B3%A0%20%EA%B4%80%EB%A6%AC%20%ED%95%84%ED%84%B0%20%EC%A0%81%EC%9A%A9.gif?raw=true" width="850" height="600"/> |

### [재고 정보 수정]
- 사용자가 원하는 재고의 제품명, 제품 분류, 브랜드, 구매 / 판매가, 할인율 등을
  수정할 수 있습니다.
- 정보 수정 후 저장 시 실시간으로 수정이 반영됩니다.

| 재고 정보 수정 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/4_%EC%9E%AC%EA%B3%A0%20%EC%83%81%EC%84%B8%EC%A0%95%EB%B3%B4%20%EC%88%98%EC%A0%95.gif?raw=true" width="850" height="600"/> |

## 상품 발주 페이지

### [상품 발주]
- 사용자 원하는 제품명을 검색 시 상품의 이미지, 코드, 품명, 가격, 판매처 등과 함께 검색 결과가 나옵니다.
- 상품 선택과 발주수량 입력 후 발주요청 버튼 클릭 시 간단하게 상품 발주가 완료 됩니다. 

| 상품 발주 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/5_%EC%83%81%ED%92%88%20%EB%B0%9C%EC%A3%BC.gif?raw=true" width="850" height="600"/> |

## 발주 관리 페이지

### [발주 관리]
- 사용자가 손쉽게 발주된 제품을 불량 재고로 옮기거나 발주 완료 처리를 할 수 있습니다. 
- 원하는 제품의 정보 탭에서 발주 처리 버튼 클릭시 간단하게 발주 완료 처리가 됩니다.

| 발주 관리 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/6_%EB%B0%9C%EC%A3%BC%20%EC%B2%98%EB%A6%AC.gif?raw=true" width="850" height="600"/> |

### [발주 관리 필터]
- 판매처, 주문번호, 주문날짜, 상태, 직원이름 등
  사용자가 원하는 검색옵션을 지정해 필터를 걸어줄 수 있습니다.
- 필터 적용 후 검색 시 지정된 검색 옵션에 맞는 값이 표시 됩니다.

| 발주 관리 필터 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/7_%EB%B0%9C%EC%A3%BC%20%EA%B4%80%EB%A6%AC%20%ED%95%84%ED%84%B0%20%EC%A0%81%EC%9A%A9.gif?raw=true" width="850" height="600"/> |

## 불량 재고 페이지

### [불량 재고 확인]
- 사용자의 검수 후 불량 재고로 이동 된 재고들을 확인할 수 있습니다.
- 재고ID, 상품명, 수량, 불량 사유, 날짜등을 확인할 수 있습니다.

| 불량 재고 확인 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/8_%EB%B6%88%EB%9F%89%20%EC%9E%AC%EA%B3%A0%20%ED%99%95%EC%9D%B8.gif?raw=true" width="850" height="600"/> |

## 배송 현황 페이지

### [배송 현황 확인]
- 사용자가 편리하게 배송 현황을 확인할 수 있습니다.
- 구매자, 주소, 인적사항, 배송상태, 판매날짜 등을 확인할 수 있습니다.

| 배송 현황 확인 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/9_%EB%B0%B0%EC%86%A1%20%ED%98%84%ED%99%A9%20%ED%99%95%EC%9D%B8.gif?raw=true" width="850" height="600"/> |

## 판매 내역 페이지

### [판매 내역 확인]
- 사용자가 편리하게 판매 내역을 확인할 수 있습니다.
- 상품명, 판매 수량, 총 가격, 판매 날짜 등을 확인할 수 있습니다.

| 판매 내역 확인 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/10_%ED%8C%90%EB%A7%A4%20%EB%82%B4%EC%97%AD%20%ED%99%95%EC%9D%B8.gif?raw=true" width="850" height="600"/> |

## 직원 관리 페이지

### [직원 정보 수정]
- 사용자가 직원의 정보를 쉽게 수정할 수 있습니다.
- 이메일, 전화번호, ID, PW, 직책, 성별, 인적사항, 주소등을 수정할 수 있습니다.

| 직원 정보 수정 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/11_%EC%A7%81%EC%9B%90%20%EC%A0%95%EB%B3%B4%20%EC%88%98%EC%A0%95.gif?raw=true" width="850" height="600"/> |

## 공지사항 페이지

### [공지사항 글 수정]
- 사용자가 게시판의 글을 편리하게 수정할 수 있습니다.
- 글꼴, 폰트 사이즈, 스타일 등을 쉽게 변경 가능하며 다양한 글 작성이 가능합니다. 

| 공지사항 글 수정 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/12_%EA%B3%B5%EC%A7%80%EC%82%AC%ED%95%AD%20%EA%B8%80%20%EC%88%98%EC%A0%95.gif?raw=true" width="850" height="600"/> |

## 다크모드

### [다크모드 전환]
- 사용자가 다크 모드로 쉽게 전환할 수 있는 기능입니다.
- 버튼 동작으로 다크모드, 기본모드로 빠르게 전환이 되며 
  사용자의 취향에 맞춰 사용 가능합니다.

| 다크모드 전환 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/main/readme_image/13_%EB%8B%A4%ED%81%AC%EB%AA%A8%EB%93%9C%20%EC%A0%84%ED%99%98.gif?raw=true" width="850" height="600"/> |
