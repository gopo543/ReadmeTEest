# 📦 TeamCostco SYSTEM README

<img src="https://github.com/gopo543/Exam/blob/develop/%EB%AC%BC%EB%A5%98%20%ED%9A%8C%EC%82%AC_.jpg?raw=true" width="500" height="400"/> 

- 배포 URL : 
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

## 2. 채택한 개발 기술과 브랜치 전략

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

## 브랜치 전략

- **Git-flow** 전략을 기반으로 main, develop 브랜치와 feature 보조 브랜치를 운영했습니다. (예시)
- main, develop, Feat 브랜치로 나누어 개발하였습니다. (예시)
  - **main**: 배포 단계에서만 사용하는 브랜치입니다. (예시)
  - **develop**: 개발 단계에서 git-flow의 master 역할을 하는 브랜치입니다. (예시)
  - **Feat**: 기능 단위로 독립적인 개발 환경을 위해 사용하고, merge 후 각 브랜치는 삭제했습니다. (예시)

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
  - 페이지: 홈, 검색, 게시글 작성, 게시글 수정, 게시글 상세, 채팅방 (예시)
  - 공통 컴포넌트: 게시글 템플릿, 버튼 (예시)
- **기능**
  - 유저 검색, 게시글 등록 및 수정, 게시글 상세 확인, 댓글 등록, 팔로워 게시글 불러오기, 좋아요 기능 (예시)

### ✏️김동민
- **UI**
  - 페이지: 프로필 설정, 프로필 수정, 팔로잉 & 팔로워 리스트, 상품 등록, 상품 수정, 채팅 목록, 404 페이지 (예시)
  - 공통 컴포넌트: 탭메뉴, InputBox, Alert 모달, 댓글 (예시)
- **기능**
  - 프로필 설정 및 수정 페이지 유저 아이디 유효성 및 중복 검사, 상품 등록 및 수정 (예시)

### 🗂️주형돈
- **UI**
  - 페이지: splash 페이지, SNS 로그인 페이지, 로그인, 회원가입 (예시)
  - 공통 컴포넌트: 상품 카드, 사용자 배너 (예시)
- **기능**
  - splash 페이지, SNS 로그인 페이지, 로그인 유효성 및 중복 검사, 회원가입 유효성 및 중복 검사, 이메일 검증, 프로필 설정, 접근 제한 설정 (예시)

### 🔍김동우
- **UI** (예시)
  - 페이지: 사용자 프로필 페이지 (예시)
  - 공통 컴포넌트: 탑배너, 하단 모달창 (예시)
- **기능**
  - 팔로우 & 언팔로우, 로그아웃, 하단 모달창, 댓글 삭제, 게시글 삭제, 상품 삭제, 사용자 게시글 앨범형 이미지, 탑 배너 뒤로가기 버튼, Alert 모달 (예시)
 
### 🗒️전상민
- **UI**
  - 페이지:
  - 공통 컴포넌트: 
- **기능**
  - ...

### 🤝이신비
- **UI**
  - 페이지: 
  - 공통 컴포넌트: 
- **기능**
  - ...

### 💼오혜준
- **UI**
  - 페이지: 
  - 공통 컴포넌트: 
- **기능**
  - ...

### 📅김민수
- **UI**
  - 페이지: 
  - 공통 컴포넌트:
- **기능**
  - ...

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
| <img src="https://github.com/gopo543/Exam/blob/develop/1_%EB%A1%9C%EA%B7%B8%EC%9D%B8.gif?raw=true" width="900" height="600"/> |

## 대시보드 페이지

### [대시보드]
- 사용자가 기간별 판매 금액, 최다 판매 제품, 판매 대비 재고 비율, 최다 발주 제품 등 많은 정보들을 한눈에 파악할 수 있습니다.
- 필요한 정보들을 1주, 1개월, 1년 단위로 확인할 수 있어 더욱 정보를 확인하기 쉽습니다.

| 정보 확인 |
|------|
| <img src="" width="900" height="600"/> |

## 재고 관리 페이지

### [필터]
- 상품코드, 매입가격, 판매가격, 대분류 등
  사용자가 원하는 검색옵션을 지정해 필터를 걸어줄 수 있습니다.
- 필터 적용 후 검색 시 지정된 검색 옵션에 맞는 값이 표시 됩니다.

| 필터 |
|------|
| <img src="https://github.com/gopo543/Exam/blob/develop/4_%EC%9E%AC%EA%B3%A0%20%EA%B4%80%EB%A6%AC%20%ED%95%84%ED%84%B0%20%EC%A0%81%EC%9A%A9.gif?raw=true" width="900" height="600"/> |

### [재고 정보 수정]
- 사용자가 원하는 재고의 제품명, 제품 분류, 브랜드, 구매 / 판매가, 할인율 등을
  수정할 수 있습니다.
- 정보 수정 후 저장 시 실시간으로 수정이 반영됩니다.

| 재고 정보 수정 |
|------|
| <img src="https://github.com/gopo543/Exam/blob/develop/4_%EC%9E%AC%EA%B3%A0%20%EC%83%81%EC%84%B8%EC%A0%95%EB%B3%B4%20%EC%88%98%EC%A0%95.gif?raw=true" width="900" height="600"/> |

## 상품 발주 페이지

### [상품 발주]
- 사용자 이름 혹은 계정 ID로 유저를 검색할 수 있습니다. (예시)
- 검색어와 일치하는 단어는 파란색 글씨로 표시됩니다. (예시)
- 클릭 시 해당 유저의 프로필 페이지로 진입합니다. (예시)

| 상품 발주 |
|------|
| <img src="https://github.com/gopo543/Exam/blob/develop/4_%EC%83%81%ED%92%88%20%EB%B0%9C%EC%A3%BC.gif?raw=true" width="900" height="600"/> |

## 발주 관리 페이지

### [발주 관리]
- 사용자 이름 혹은 계정 ID로 유저를 검색할 수 있습니다. (예시)
- 검색어와 일치하는 단어는 파란색 글씨로 표시됩니다. (예시)
- 클릭 시 해당 유저의 프로필 페이지로 진입합니다. (예시)

| 발주 관리 |
|------|
| <img src="https://github.com/gopo543/Exam/blob/develop/5_%EB%B0%9C%EC%A3%BC%20%EC%B2%98%EB%A6%AC.gif?raw=true" width="900" height="600"/> |

### [발주 관리 필터]
- 판매처, 주문번호, 주문날짜, 상태, 직원이름 등
  사용자가 원하는 검색옵션을 지정해 필터를 걸어줄 수 있습니다.
- 필터 적용 후 검색 시 지정된 검색 옵션에 맞는 값이 표시 됩니다.

| 발주 관리 필터 |
|------|
| <img src="https://github.com/gopo543/Exam/blob/develop/5_%ED%95%84%ED%84%B0%20%EC%A0%81%EC%9A%A9.gif?raw=true" width="900" height="600"/> |

## 불량 재고 페이지

### [불량 재고 확인]
- 사용자의 검수 후 불량 재고로 이동 된 재고들을 확인할 수 있습니다.
- 재고ID, 상품명, 수량, 불량 사유, 날짜등을 확인할 수 있습니다.

| 불량 재고 확인 |
|------|
| <img src="https://github.com/gopo543/Exam/blob/develop/6_%EB%B6%88%EB%9F%89%20%EC%9E%AC%EA%B3%A0%20%ED%8E%98%EC%9D%B4%EC%A7%80_%20%EC%82%AC%EC%A7%84.png?raw=true" width="900" height="600"/> |

## 배송 현황 페이지

### [배송 현황 확인]
- 사용자가 편리하게 배송 현황을 확인할 수 있습니다.
- 구매자, 주소, 인적사항, 배송상태, 판매날짜 등을 확인할 수 있습니다.

| 배송 현황 확인 |
|------|
| <img src="https://github.com/gopo543/Exam/blob/develop/7_%EB%B0%B0%EC%86%A1%20%ED%98%84%ED%99%A9%20%ED%8E%98%EC%9D%B4%EC%A7%80%20_%20%EC%82%AC%EC%A7%84.png?raw=true" width="900" height="600"/> |

## 판매 내역 페이지

### [판매 내역 확인]
- 사용자가 편리하게 판매 내역을 확인할 수 있습니다.
- 상품명, 판매 수량, 총 가격, 판매 날짜 등을 확인할 수 있습니다.

| 판매 내역 확인 |
|------|
| <img src="https://github.com/gopo543/Exam/blob/develop/8_%ED%8C%90%EB%A7%A4%20%EB%82%B4%EC%97%AD%20%ED%8E%98%EC%9D%B4%EC%A7%80_%EC%82%AC%EC%A7%84.png?raw=true" width="900" height="600"/> |

## 직원 관리 페이지

### [직원 정보 수정]
- 사용자가 직원의 정보를 쉽게 수정할 수 있습니다.
- 이메일, 전화번호, ID, PW, 직책, 성별, 인적사항, 주소등을 수정할 수 있습니다.

| 직원 정보 수정 |
|------|
| <img src="https://github.com/gopo543/Exam/blob/develop/9_%ED%9A%8C%EC%9B%90%20%EC%A0%95%EB%B3%B4%20%EC%88%98%EC%A0%95.gif?raw=true" width="900" height="600"/> |

## 공지사항 페이지

### [공지사항 글 수정]
- 사용자가 게시판의 글을 편리하게 수정할 수 있습니다.
- 글꼴, 폰트 사이즈, 스타일 등을 쉽게 변경 가능하며 다양한 글 작성이 가능합니다. 

| 공지사항 글 수정 |
|------|
| <img src="https://github.com/gopo543/Exam/blob/develop/10_%EA%B3%B5%EC%A7%80%EC%82%AC%ED%95%AD%20%EA%B8%80%20%EC%88%98%EC%A0%95.gif?raw=true" width="900" height="600"/> |

## 다크모드

### [다크모드 전환]
- 사용자가 다크 모드로 쉽게 전환할 수 있는 기능입니다.
- 버튼 동작으로 다크모드, 기본모드로 빠르게 전환이 되며 
  사용자의 취향에 맞춰 사용 가능합니다.

| 다크모드 전환 |
|------|
| <img src="https://github.com/gopo543/Exam/blob/develop/11_%EB%8B%A4%ED%81%AC%EB%AA%A8%EB%93%9C%20%ED%99%9C%EC%84%B1%ED%99%94,%20%EB%B9%84%ED%99%9C%EC%84%B1%20%ED%99%94.gif?raw=true" width="900" height="600"/> |

## 7. 프로젝트 후기

### 📊강동윤
깃헙을 통한 협업에 익숙해지는 것, 서로 감정 상하지 않고 무사히 마무리하는 것이 1차적인 목표였어서 항상 이 부분을 명심하면서 작업했습니다.  
각자 페이지를 작업하고 합치는 과정에서 마주친 버그들이 몇 있었는데, 시간에 쫓기느라 해결하기에 급급해서 제대로 트러블슈팅 과정을 기록하지 못한 게 살짝 아쉬운 부분으로 남습니다. 그래도 2022년 한 해 동안 가장 치열하게 살았던 한 달인 것 같습니다. 조원들 모두에게 고생했다고 전하고 싶습니다 (예시)

### ✏️김동민
여러모로 많은 것들을 배울 수 있었던 한 달이었습니다. 혼자서는 할 수 없었던 일이라는 것을 너무 잘 알기에 팀원들에게 정말 감사하다는 말 전하고 싶습니다. 개인적으로 아쉬웠던 부분은 기한 내에 기능을 구현하는 데에만 집중하면서 트러블 슈팅이나 새로 배웠던 것들을 체계적으로 기록하지 못했다는 점입니다. 이렇게 느낀 바가 있으니 이후의 제가 잘 정리하면서 개발할 거라 믿습니다. (예시)

### 🗂️주형돈
팀 프로젝트 시작에 앞서 초기 설정을 진행하며 체계적인 설계의 중요성을 느꼈습니다. 앞으로는 점점 더 체계적이고 효율적으로 프로젝트를 진행할 수 있도록 발전하고 싶습니다.  
정규 수업 직후에 프로젝트를 진행하면서 배운 내용을 직접 구현하는 과정이 어색했지만 어떤 부분이 부족한지 알 수 있는 기회였습니다. 스스로 최대한 노력해보고 팀원들과 함께 해결해 나가면서 협업의 장점을 체감할 수 있었습니다. 하지만 빠르게 작업을 진행하면서 팀원들과 함께 해결한 이슈가 어떤 이슈이며 어떻게 해결했는지에 대해 자세히 작성하지 못한 것이 아쉽습니다.  
’멋쟁이 사자처럼’이라는 같은 목표를 가진 집단에서 프로젝트에 함께할 수 있는 소중한 경험이었습니다. 함께 고생한 조원들 모두 고생하셨습니다! 앞으로도 화이팅해서 함께 목표를 이뤄가고 싶습니다. (예시)

### 🔍김동우
컨벤션을 정하는 것부터 Readme 파일 작성까지 전 과정을 진행하려니 처음 생각보다 많은 에너지를 썼어요. 좋은 의미로 많이 썼다기보다, 제 능력을 십분 발휘하지 못해서 아쉬움이 남는 쪽입니다. 개발한다고 개발만 해서는 안 된다는 것을 몸소 느껴보는 기간이었던 것 같습니다. 이번 기회로 프로젝트를 진행하면서, 제가 잘하는 점과 부족한 점을 확실하게 알고 가는 건 정말 좋습니다. 기술적인 부분에 있어서는 리액트의 컴포넌트화가 주는 장점을 알았습니다. 조금 느린 개발이 되었을지라도 코드 가독성 부분에 있어서 좋았고, 오류가 발생해도 전체가 아닌 오류가 난 컴포넌트와 근접한 컴포넌트만 살펴보면 수정할 수 있는 부분이 너무 편했습니다. 모두 고생 참 많으셨고 리팩토링을 통해 더 나은 프로젝트 완성까지 화이팅입니다. (예시)

### 🗒️전상민

### 🤝이신비

### 💼오혜준

### 📅김민수
