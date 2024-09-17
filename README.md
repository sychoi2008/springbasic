### 스프링을 왜 써?
- 객체 지향 언어의 장점 -> 다형성

### 어노테이션이 뭔데? 

### 스프링 컨테이너가 뭔데?
- 1)사용할 객체들을 **Bean으로 등록**시켜 2)**의존관계를 설정**하고 생애를 관리하는 통
- 스프링이 기본적으로 객체를 싱글톤으로 만들어서 관리해줌

### 스프링 컨테이너를 왜 사용하는데?
- 싱글톤 컨테이너의 기능

### 컴포넌트 스캔과 의존관계 자동 주입
- Componenet Scan : @Component 어노테이션이 붙은 클래스들을 다 읽어서 자동으로 Bean으로 등록한다 
  -> 따라서, 사용할 구현체들에게 @Component를 붙인다
  -> 그런데 의존성 주입은 어떻게 할거야!! 이건 그냥 단순히 빈에 등록하는 행위만 한 것
  -> 이 때, @Autowired 등장! 의존관계 자동주입


### @Autowired
- 생성자 자동 주입 : @Component 스캔을 하고, Bean을 등록하기 위해 생성자를 호출한다 ->  @Autowired 발견 -> 스프링 컨테이너에서 주입할 Bean을 꺼내서 주입해줌
  - 생성자 호출하면서 딱 한번만 실행 -> 불변, 필수 

