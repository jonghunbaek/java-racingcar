## 요구사항 분석
### 기능 요구사항
- [x] 몇 대의 자동차를 생성할 지 입력을 받는다.
- [x] 몇 번을 이동할 지 입력을 받는다.
- [x] 자동차의 이동은 랜덤 값을 전달 받아야 한다.
- [x] 랜덤 값이 4이상인 경우에만 자동차가 이동한다.
- [x] 랜덤 값이 0~9의 범위를 벗어나면 예외를 던져야 한다.
- [x] 각 횟수 별로 이동한 자동차를 화면에 출력한다.

### 4단계 추가 요구사항
- [ ] 3단계에서 구현하지 않은 입력 값에 대한 검증로직 작성
- [x] 자동차에 이름 속성 추가
- [x] 이름은 5자 이하만 가능 -> 예외 테스트, 원시 값 포장으로 해결
- [x] 입력된 자동차 이름들은 ","로 구분
- [x] 자동차 출력 시 이름도 같이 출력
- [x] 경주에서 우승한 차량을 출력하고, 우승차는 2대 이상이 될 수 있다.

### 클래스 역할
- [x] Car는 이동가능한 조건(상수), 엑셀의 가동 범위(상수), 이동 위치(필드변수), 이름(필드 변수)를 속성으로 가지고 엑셀을 밟은 힘에 따라 이동을 하는 메서드를 가진다.
- [x] Cars는 일급 컬렉션으로 복수의 Car객체를 컬렉션에 저장하고 불변상태를 유지한다. 
- [x] CarRacer는 자동차의 엑셀을 밟는 행동(랜덤 숫자를 생성하는 메서드)를 가진다.
- [x] CarRacing(Controller)은 복수의 자동차, 카레이서를 관리한다.
- [x] RacingOutput은 사용자에게 질문, 자동차의 위치를 출력한다.
- [x] RacingInput은 사용자에게 질문에 대한 답을 입력한다.
- [x] CarRacingView는 CarRacing, RacingOutput, RacingInput과 의존 관계를 가지며 자동차 경주 게임을 진행한다.
