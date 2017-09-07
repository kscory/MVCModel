# MVC Model
MVC Model 개념


## MVC 란
사용자 인터페이스로부터 비즈니스 로직을 분리하여 어플리케이션의 시각적 요소나 그 이면에서 실행되는 비즈니스 로직을 서로 영향 없이 쉽게 고칠 수 있는 응용프레임워크의 기반이 되는 패턴
</br> M(Model) / V(View) / C(Controller) 로 구성
#### 1. __Model__ : 데이터를 저장
 * DB 혹은 파일 저장소를 뜻함
 * 데이터 모델을 생성하고 이를 다루는 인터페이스 생성
 * 데이터를 검증하고 모든 오류는 컨트롤러에게 보고
 * 사용자 인터페이스를 직접 다루지 않음

#### 2. __View__ : 사용자 인터페이스 요소
 * 입력 / 출력과 관련
 * 데이터베이스의 직접 접근을 피해야 함
 * 복잡한 로직보다는 최대한 간결하게 표시

#### 3. __Controller__ : 객체 또는 데이터의 흐름을 책임지는 컨포넌트
 * 주로 연결고리 역할
 * 모든 요청 에러와 모델에러를 처리
 * 데이터를 화면에 표시하거나 데이터베이스와 로직을 직접 다루지 않도록 함

![](https://github.com/Lee-KyungSeok/MVCModel/blob/master/picture/MVC1.PNG)

## MVC 장단점
#### 1. 장점
 * 사용자 인터페이스로부터 비즈니스 로직을 분리하여 어플리케이션의 시각적 요소와 그 이면에서 실행되는 비즈니스 로직을 서로 영향 없이 수정 및 유지보수 가능
 * 특정 영역에만 집중할 수 있도록 업무 분할 가능
 * 화면 표시에 영향을 주지 않고 로직 수정 가능

#### 2. 단점
 * 기본기능 설계를 위해 클래스들이 많이 필요하여 복잡해질 가능성 존재
 * 속도가 상대적으로 느릴 수 있음
 * Model과 View가 완전히 독립적이지 않을 수 있음

## 참고 문제
Collection을 활용하여 MVC 형태로 개발
1. [Memo 문제](https://github.com/Lee-KyungSeok/MemoExample)
