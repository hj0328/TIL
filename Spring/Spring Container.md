# Spring Container

- Bean 객체 생성, 관리, 삭제 및 Bean 객체간의 의존관계를 연결해주는 것을 컨테이너라 함 
따라서 구현체는 코드 수정없이 구현에만 집중
- IoC 컨테이너 또는 DI 컨테이너라고 부름
  - Inversion of Control
    - 컨테이너가 개발자를 대신하여 호출하는 메서드가 필요로 하는 자원을 전달하는 설계 구조
  - Dependency Inversion
    - Runtime 시 IoC의 자원 전달을 수행하는 과정을 의미
    - ex) Bean 객체가 생성 시 필요한 객체 전달
    - Bean 간에 서로 종속되는 상황은 피하자 
    해당 상황 시 BeanCurrentlyInCreationException 예외 발생
- 컴테이너 동작 조작
  - xml 파일에서서 컨테이너의 설정 정보, Bean 관리를 조작가능
    - Runtime 시에는 ApplicationContext 객체를 이용하여 조작가능 ex) getBean 메서드

![image](https://user-images.githubusercontent.com/24749457/187020305-8c973d49-4189-4e55-ac62-f4fde8d69f37.jpeg)



