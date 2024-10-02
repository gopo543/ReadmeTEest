# 🛒 TeamCostco Mall README

<img src="https://github.com/gopo543/ReadmeTEest/blob/mall/image/card_1379_1.jpg?raw=true" width="700" height="500"/> 

- 배포 URL : [http://15.165.19.189](http://ezentwix.xyz)

## 프로젝트 소개

- Costco의 물류 프로세스를 혁신하고 효율성을 극대화하기 위한 종합적인 관리 시스템의 쇼핑몰 개발 프로젝트
- 실시간 주문과 사용자의 편의를 위한 찜 목록, 장바구니, 주소지 설정까지 모두 간단하게 가능한 쇼핑몰
- 직관적이며 간단한 ui로 사용자의 쇼핑 시간 단축이 가능하며 남녀노소 사용가능한 쇼핑몰

## 팀원 구성

| 강동윤 | 김동민 | 주형돈 | 김동우 | 황지영| 
|:------:|:------:|:------:|:------:|:------:|
| <img src="https://avatars.githubusercontent.com/u/173039221?v=4" width="50" height="50"/> <br> [@KangDY26](https://github.com/KangDY26) | <img src="https://avatars.githubusercontent.com/u/173039024?v=4" width="50" height="50"/> <br> [@uiwoowP](https://github.com/uiwoowP) | <img src="https://avatars.githubusercontent.com/u/173039030?v=4" width="50" height="50"/> <br> [@hdjoo0820](https://github.com/hdjoo0820) | <img src="https://avatars.githubusercontent.com/u/173039738?v=4" width="50" height="50"/> <br> [@DukkyRacoon](https://github.com/DukkyRacoon) | <img src="https://avatars.githubusercontent.com/u/82192951?s=48&v=4" width="50" height="50"/> <br> [@jiyoungoss](https://github.com/jicongjy/jiyoungoss)

| 전상민 | 이신비 | 오혜준 | 김민수 |
|:------:|:------:|:------:|:------:|
| <img src="https://avatars.githubusercontent.com/u/68059753?v=4" width="50" height="50"/> <br> [@jsm3794](https://github.com/jsm3794) | <img src="https://avatars.githubusercontent.com/u/173039141?v=4" width="50" height="50"/> <br> [@SHINBI116](https://github.com/SHINBI116) | <img src="https://avatars.githubusercontent.com/u/173116759?v=4" width="50" height="50"/> <br> [@Oh-hyejun](https://github.com/Oh-hyejun) | <img src="https://avatars.githubusercontent.com/u/131967955?v=4" width="50" height="50"/> <br> [@gopo543](https://github.com/gopo543) |

## 1. 개발 환경

- Front-end : HTML, CSS, JavaScript
- Back-end : Java, Spring Boot, Oracle SQL Developer
- 버전 및 이슈관리 : Github, Github Issues, Github Project
- 협업 툴 :  Slack, Notion, Figma

## 2. 채택한 개발 기술과 전략

### Front-end 기술

- **HTML, CSS, JavaScript**
  - 웹 페이지의 구조와 스타일을 정의하기 위해 사용되었습니다. 
  - 사용자 경험을 향상시키기 위해 반응형 웹 디자인을 적용했습니다. 

### Back-end 기술

- **Java, Spring Boot**
  - 안정적이고 확장 가능한 서버 사이드 애플리케이션 개발을 위해 선택했습니다.
  - RESTful API를 통해 클라이언트와의 효율적인 데이터 통신을 구현했습니다.

- **Naver API, Google Pub/Sub API, KaKao API, tiny MCE Editer API**
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
│          │    ├── controller
│          │    │      ├── CartPageController.java
│          │    │      ├──    .
│          │    │      ├──    .
│          │    │      └── SearchListPageController.java
│          │    │
│          │    ├── dto
│          │    │      ├── Category
│          │    │      │       ├── CategoryDTO.java
│          │    │      │       ├──   .
│          │    │      │       ├──   .
│          │    │      │       └── CategoryResponse.java
│          │    │      │
│          │    │      ├── cart
│          │    │      │       └── CartDTO.java
│          │    │      ├──    .
│          │    │      ├──    .
│          │    │      └── inventory
│          │    │              └── SmallCategoryDTO.java
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
│          │    │      └── ShippingAddressService.java
│          │    │
│          │    ├── PageMetadataProvider.java
│          │    ├── S3Config.java
│          │    ├── ServletInitializer.java
│          │    └── TeamcostcoApplication.java
│          │
│          └── resources
│               ├── mapper
│               │      ├── cart_mapper.xml
│               │      ├──    .
│               │      ├──    .
│               │      └── products_mapper.xml
│               │
│               ├── static
│               │      ├── css
│               │      │    ├── common
│               │      │    │      ├── footer.css
│               │      │    │      ├── .
│               │      │    │      ├── .
│               │      │    │      └── header.css
│               │      │    │      
│               │      │    ├── component
│               │      │    │      ├── filter.css
│               │      │    │      ├── .
│               │      │    │      ├── .
│               │      │    │      └── sidebar.css
│               │      │    │      
│               │      │    └── contents
│               │      │           ├── aboutus.css
│               │      │           ├── .
│               │      │           ├── .
│               │      │           └── search.css
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
│               │      │    └── contents
│               │      │           ├── intro.js
│               │      │           ├── .
│               │      │           ├── .
│               │      │           └── wishlist.js
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
  - 페이지: 
  - 공통 컴포넌트: 
- **기능**
  - 

### ✏️김동민
- **UI**
  - 페이지: 
  - 공통 컴포넌트: 
- **기능**
  - 

### 🗂️주형돈
- **UI**
  - 페이지: 
  - 공통 컴포넌트: 
- **기능**
  - 

### 🔍김동우
- **UI**
  - 페이지:
  - 공통 컴포넌트: 
- **기능**
  - 
- **DB 관리**
  - 각종 테이블, 컬럼, 제약 조건 등 전반적인 DB 정보 관리

### 🌫️황지영
- **UI**
  - 페이지: 
  - 공통 컴포넌트: 
- **기능**
  - 
 
### 🗒️전상민
- **UI**
  - 페이지: 
  - 공통 컴포넌트: 
- **기능**
  - 

### 🤝이신비
- **UI**
  - 페이지: 
  - 공통 컴포넌트: 
- **기능**
  - 

### 💼오혜준
- **UI**
  - 페이지: 
  - 공통 컴포넌트: 
- **기능**
  - 

### 📅김민수
- **UI**
  - 페이지: 
  - 공통 컴포넌트: 
- **기능**
  - 

## 5. 개발 기간 및 작업 관리

### 개발 기간
- 전체 개발 기간: 2024-08-19 ~ 2024-10-02

### 작업 관리
- Slack, 노션을 사용하여 진행 상황을 공유했습니다. 
- 주간회의를 진행하며 작업 순서와 방향성에 대한 고민을 나누고 Slack에 회의 내용을 기록했습니다.

## 6. 페이지별 기능 

## 메인 페이지

### [메인] 

- 사용자의 한눈에 모든 기능이 들어오게끔 하여 사용자의 편의성을 높였습니다.

| 메인 |
|--------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/mall/image/1_%EB%A9%94%EC%9D%B8%20%ED%8E%98%EC%9D%B4%EC%A7%80.gif?raw=true" width="850" height="600"/> |

## About Us 페이지

### [페이지 소개] 

- 사용자가 사이트의 이해도를 높이기 위한 페이지로서 가볍게 이용할 수 있는 페이지입니다.

| 페이지 소개 |
|--------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/mall/image/2_About%20Us.gif?raw=true" width="850" height="600"/> |


## 로그인 페이지

### [로그인] 

- 카카오로그인 API를 사용함으로서 사용자의 편의성을 증가시키고 로그인을 단순화 시켰습니다.

| 로그인 |
|--------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/mall/image/3_%EB%A1%9C%EA%B7%B8%EC%9D%B8.gif?raw=true" width="850" height="600"/> |

## 배송지 관리 페이지

### [배송지 관리]
- 사용자가 손 쉽게 배송지를 추가, 삭제 가능하며 카카오주소 API를 활용하여 사용자의 편의성을 증가시켰습니다.

| 배송지 관리 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/mall/image/4_%EB%B0%B0%EC%86%A1%EC%A7%80%20%EA%B4%80%EB%A6%AC.gif?raw=true" width="850" height="600"/> |

## 상품 관련 페이지

### [상품 검색, 정보 확인]
- 쉽고 빠르게 검색이 가능하며 직관적인 UI로 빠른 상품 검색과 정보 확인이 가능합니다.

| 상품 검색, 정보 확인 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/mall/image/5_%EC%83%81%ED%92%88%20%EA%B2%80%EC%83%89,%20%EC%A0%95%EB%B3%B4%20%ED%99%95%EC%9D%B8.gif?raw=true" width="850" height="600"/> |

### [상품 찜하기, 찜 목록 확인]
- 사용자의 편의성을 위해 찜 기능을 추가하였으며 편리하게 찜 목록 확인이 가능합니다.

| 상품 찜하기, 찜 목록 확인 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/mall/image/6_%EC%83%81%ED%92%88%20%EC%B0%9C%ED%95%98%EA%B8%B0,%20%EC%B0%9C%20%EB%AA%A9%EB%A1%9D%20%ED%99%95%EC%9D%B8.gif?raw=true" width="850" height="600"/> |

### [장바구니 추가, 장바구니 확인]
- 사용자의 편의성을 위해 장바구니 기능을 추가하였으며 편리하게 장바구니 목록 확인이 가능합니다.-

| 장바구니 추가, 장바구니 확인 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/mall/image/7_%EC%9E%A5%EB%B0%94%EA%B5%AC%EB%8B%88%20%EC%B6%94%EA%B0%80,%20%EC%9E%A5%EB%B0%94%EA%B5%AC%EB%8B%88%20%ED%99%95%EC%9D%B8.gif?raw=true" width="850" height="600"/> |

### [주문, 결제하기]
- 쉽고 빠른 시스템으로 주문, 결제가 한번에 가능하며 사용자의 사이트 이용 시간을 단축하였습니다.

| 주문, 결제하기 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/mall/image/8_%EC%A3%BC%EB%AC%B8,%20%EA%B2%B0%EC%A0%9C%ED%95%98%EA%B8%B0.gif?raw=true" width="850" height="600"/> |

### [주문 내역 확인]
- 사용자가 간편하게 주문 내역을 확인 가능하도록 직관적인 디자인을 하였습니다.

| 주문 내역 확인 |
|------|
| <img src="https://github.com/gopo543/ReadmeTEest/blob/mall/image/9_%EC%A3%BC%EB%AC%B8%20%EB%82%B4%EC%97%AD.gif?raw=true" width="850" height="600"/> |
