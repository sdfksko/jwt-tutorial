post localhost:8080/join     body값 : username: admin  password: 1234
post localhost:8080/login   header부분에서 authentication jwt토큰 값 확인
get  localhost:8080/admin   header부분에 authentication jwt토큰 값 기입
순으로 실행 시 정상적으로 jwt 인증 확인
세션은 STATELESS 상태로 두었습니다.
아직 인증만 구현하였고, 실제 사용자 ui에서 관리자페이지 클릭 시 토큰값을 넘길 수 있게끔 프론트로 가져와 js부분에서 직접 header에 넣는 방식으로 구현하여 사용자 측에서 에러가 발생하지 않게 직접 공부하며 개발할 예정입니다.
spring security, jwt 등 기존에 배운 웹개발에 조금 더 심화있는 지식을 공부하고 적용해가며 추가적으로 구현할 생각입니다.
그거에 관한 공부자료입니다.


같이 첨부되어있는 spring_react_login 폴더는 간단한 프론트로 화면만 구성 후 실제 서버와 연결하여 실제 로그인 환경을 구현할 생각입니다.


구현 중 조금 더 spring security 이론에 대해 공부가 필요하다 생각하여 잠시 중지하고 이론 공부를 진행 중입니다. (2025.08.28 일시 중지)
이론 공부 후 기존의 spring_react_login은 잠시 중단 후 jwt 심화과정(토큰 만료시 재발행 후 인가) 등에 대해서 먼저 공부 후 관련 자료를 업로드 할 예정입니다. 그 후 spring_react_login 다시 재구성 시작 예정입니다.
