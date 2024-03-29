# Dont_BE_Late_Front

# 2023-HUFS SUMMER_HACKATHON
# 통학 셔틀에 대한 불편함을 최소화 주는 웹 서비스
#### Project nickname : 늦지마요
#### Team : Euphoria

-----------------------
## ▶︎Developer

|                                 팀장                                  |                                  팀원                                   |                                   팀원                                   |                                 팀원                                  |
| :-------------------------------------------------------------------: | :------------------------------------------------------------------: | :-------------------------------------------------------------------: | :-------------------------------------------------------------------: |
|                             Back Developer                              |                              Front Developer                             |                             Back Developer                              |                             Front Developer                              |
| <img src="https://github.com/lee0798/back_pro1/assets/71830104/d29e3cee-df20-4944-b395-2297df097a70" width="150" height="150"/> | <img src="https://github.com/lee0798/back_pro1/assets/71830104/34d22164-e7cb-41ec-be2b-35524ff9b137" width="150" height="150"/> | <img src="https://github.com/lee0798/back_pro1/assets/71830104/d29e3cee-df20-4944-b395-2297df097a70" width="150" height="150"/> | <img src="https://github.com/lee0798/back_pro1/assets/71830104/e411b9aa-8c46-4924-9e9b-f2e45843afb4" width="150" height="150"/> |
|                  [황동규]               |                 [조주희]                 |                 [이도환]                 |                 [이산]                 |
## ▶︎Motivation for project
이번학기 에브리 타임, 학교 건의 사항등을 통해 교내 셔틀의 실시간으로 바뀌는 정보들을 얻지 못하는 학생들이 여럿 있었습니다. 셔틀버스를 놓침으로써 시간 낭비, 지각등 학생들이 많은 피해를 받고 이에대한 불만을 토로했습니다. 이에대해 관리자 입장에서는 셔틀 버스 노선별로 실시간으로 바뀌는 정보에 대한 공지(예: 교통체증으로 인한 시간 지연)를 올릴 수 있고, 학생들은 이런 공지를 실시간으로 확인할 수 있으며 이용자 간의 추가적인 정보 교류를 위한 채팅 기능을 추가하여 올바른 정보를 이용 할 수있도록 서비스를 기획해 보았다.

## ▶︎Topic associations
대학생활의 문제점 해결,레빗점프-선제적 대응 기술: 통학하는 학생들의 셔틀버스 운영에 대한 실시간 정보, 건의 사항을 서비스에 적용하며 대학생활 중 등/하교 과정에서 겪을수 있는 교통 문제, 선제적 대응 기술에서 알아서 배려해주는  기술이라는 키워드를 통해 주제를 연관지었다.

## ▶︎Description
늦지마요는 학교에서 제공하는 셔틀을 이용하는 학생들에게 실시간으로 각 노선에 특이 사항이 생기거나 건의사항과 문의사항이 생기게 되면, 실시간으로 해결할 수 있는 환경을 제공해준다.
시중에서는 에브리타임과 같은 대학교내 커뮤니티가 있으나, 이러한 주제있어 보다 사용자 입장에서의 기능이 부족하며, 다수의 학생들이 이용하기 어렵다는 점이있다.

## ▶︎Demer video[2023-06-24 11-14-22.zip](https://github.com/juhui88/Dont_Late_Front/files/11854238/2023-06-24.11-14-22.zip)


## How to run the front end
✪리액트를 사용하여 구현하였고 여러 모듈들을 사용했다. 
1. 로그인 및 회원가입 페이지
   - useForm을 사용하여 유저에게 받은 데이터를 관리해줬고 받은 값은 백엔드로 넘겨서 회원가입과 로그인을 구현했다.
2. 로그인 후 메인페이지
   - 학교 내의 버스 노선 전체를 보여준다. 이는 axios를 통해 get 메서드로 호출하여 정보를 받아왔다..
3. 각 노선별로 공지페이지
   - 그 날의 교통 상황에 따라 관리자의 공지를 보여준다. 이 부분은 관리자의 id를 받아와서 해당 id를 가진 사람만 글을 작성할 수 있도록 했다.
4. 각 노선별 채팅페이지
    - 그 날의 공지를 제외한 추가적인 정보를 서비스 이용자간 공유할 수 있는 채팅기능을 구현 했다.
5. 리스트 노선 정보
    - 자신이 원하는 노선(예: 강남행) 등과 같은 리스트 차트를 통하여 원하는 노선의 정류장의 정차 시간, 지도 위치를 받아 정보를 제공 할 수 있는 기능을 구현했다.

## How to run the back end
AWS EC2와 RDS를 사용해 서버 배포를 진행하였고, Node.js, mysql를 사용하여 구현하였고 여러 모듈을 사용했습니다.
1. User, Map, Post 등의 데이터베이스 설계
2. AWS EC2, RDS를 이용하여 서버 배포
3. 로그인 및 회원가입 페이지 등 기본페이지 라우트 분리 및 설정
4. 로그인 후 메인페이지
5. 각 노선별로 공지페이지
6. 각 노선별 채팅페이지
7. 검색 기능을 통한 노선 정보



## Item Scalability

1. 새로운 기능 추가: 사용자의 편의성과 서비스의 가치를 높일 수 있는 새로운 기능을 추가할 수 있습니다. 예를 들어, 실시간 업데이트된 노선별 운행 상태 정보, 도착 예정 
   시 간, 혼잡도 정보 등을 제공하여 사용자들이 더욱 편리하게 이용할 수 있게 할 수 있습니다.

2. 다양한 플랫폼 지원: 현재 메신저를 통한 실시간 채팅 서비스를 제공하고 계시는데, 확장성을 고려하여 다양한 플랫폼에 대한 지원을 고려할 수 있습니다. 예를 들어, 웹, 
   앱, 소셜 메신저 플랫폼 등 다양한 경로를 통해 사용자들과의 소통을 지원할 수 있습니다.

3. 개인화된 서비스: 사용자들의 선호도와 필요에 따라 개인화된 서비스를 제공할 수 있습니다. 예를 들어, 사용자들이 선호하는 언어로 정보를 제공하거나, 관심 있는 노선에 대 
   한 알림 서비스를 제공할 수 있습니다.

4. 데이터 분석과 예측 기능: 수집된 데이터를 활용하여 향후 노선별 상황을 예측하고, 이를 기반으로 사용자들에게 추천과 조언을 제공할 수 있습니다. 예를 들어, 특정 시간대 
   에 혼잡도가 높은 노선에 대해 경로 변경을 권장하거나, 대체 교통 수단을 제안할 수 있습니다.

5. 확장된 관리자 기능: 관리자들이 노선에 대한 상세한 정보를 업로드하고 수정할 수 있는 기능을 추가할 수 있습니다. 이를 통해 관리자들이 실시간으로 업데이트된 정보를 제 
   공하고, 사용자들에게 정확하고 신뢰할 수 있는 정보를 제공할 수 있습니다.

## Environment

> React 17.0.2
> 
> Node.js 16.9.0
> 
> MySQL 8.0
> 
> Prisma 2.32.x

