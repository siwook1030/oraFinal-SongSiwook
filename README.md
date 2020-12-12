# 오늘의 라이딩 프로젝트 (송시욱 코드)
---------------------
`해당 Repository는 '오늘의 라이딩 프로젝트' 중, 제가 구현한것만 간추린  .`
### 프로젝트 기획 의도

>자전거 코스를 찾으면 대부분 국토종주나 유명 관광명소 코스만 소개되는 경우가 많아, 간단한 라이딩을 즐길 수 있는 코스는 찾기가 어려운 경우가 많았습니다. 
사용자가 위치, 거리, 시간, 풍경을 직접 선택하고 검색하여 원하는 코스를 쉽고 빠르게 찾을 수 있는 사이트가 있으면 어떨까 하여 이 프로젝트를 개발하게 되었습니다. 
또한 사용자가 직접 자신만의 코스를 만들어 다른 사용자들과 코스를 공유하여 즐길 수 있는 기능을 구현하여 능동적인 부분을 추가하였습니다.   


### 오늘의 라이딩 기능 (송시욱 구현 부분)
`[카카오 지도 API를 사용함]`
1. 자전거 맞춤 코스 검색(searchCourse)
   - 지도에서 원하는 위치를 선택, 거리, 시간을 선택하여 검색
   - 검색조건에 부합하는것 뿐만 아니라 근접하는 코스들도 검색 됨
   

2. 자전거 태그 코스 검색(tagSearchCourse)
   - 코스를 만들 때 태그를 여러개 추가 할 수 있음
   - 맞춤 코스검색과 다르게 태그들로 코스를 더 빠르게 검색 할 수 있음
   

3. 자전거 코스 만들기(makingCourse)
   - 사용자가 gpx파일로 코스를 만들 수 있음
   - gpx파일은 크롬확장프로그램 '바이크 루트'를 통해 카카오지도에서 생성가능
   - 코스를 만드는 도중 '미리보기' 기능을 제공 함
   
4. 자전거 코스 상세보기(detailCourse)
   - 자전거 코스에 대한 상세보기 기능
   - 코스경로, 근처 병원,숙박,카페,관광명소 등 카카오API를 통해 확인 가능
   - 공공데이터를 활용하여 각 지자체 공영자전거 대여위치 및 대여가능 수 확인 가능


4. 번개 게시판 댓글(detailMeeting)
   - 네이버카페 댓글과 기능 유사하게 구현함 
   

5. 로그인(login)
   - 스프링시큐리티 적용
   

6. 회원가입(signUp)
5. 관리자 페이지(admin)
   - 스프링 AOP 적용하여 사용자들의 코스검색내용을 log기록으로 저장함
   - 사용자의 사이트 활동(코스만들기,글쓰기 등)에 따라 랭크를 부여함 (1레벨, 2레벨...)
   - 그래프차트를 이용하여 사용자들의 활동을 파악할 수 있음
   - 사용자가 만든 코스를 수정, 삭제할 수 있고 검색이 될 수 있게 승인 기능이 있음(승인 시 사용자한테 문자 발송)
--------------------------


#### **읽어주셔서 감사합니다  : )**
