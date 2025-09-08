post localhost:8080/join     body값 : username: admin  password: 1234
post localhost:8080/login   header부분에서 authentication jwt토큰 값 확인
get  localhost:8080/admin   header부분에 authentication jwt토큰 값 기입
순으로 실행 시 정상적으로 jwt 인증 확인
세션은 STATELESS 상태로 두었습니다.
아직 인증만 구현하였고, 실제 사용자 ui에서 관리자페이지 클릭 시 토큰값을 넘길 수 있게끔 프론트로 가져와 js부분에서 직접 header에 넣는 방식으로 구현하여 사용자 측에서 에러가 발생하지 않게 직접 공부하며 개발할 예정입니다.
spring security, jwt 등 기존에 배운 웹개발에 조금 더 심화있는 지식을 공부하고 적용해가며 추가적으로 구현할 생각입니다.
그거에 관한 공부자료입니다.

2025.09.01 springJWT 폴더 추가
기존의 jwt-tutorial에서는 단일 토큰으로 jwt의 기초를 배웠다면 해당 폴더에서는 단일 토큰이 아닌 다중 토큰으로 access토큰과 refresh토큰을 각각 구현하여 조금 더 보안을 강화하고 심화 학습 공부를 진행하며 적용해가고 있습니다.(진행중)
