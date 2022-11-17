## 함수

#### 작게만들어라

```java
public static String renderPageWithSetupsAndTeardowns(PageData pageData, boolean isSuite) throws Exception {
  if (isTestPage(pageData))
    includeSetupAndTeardownPages(pageData, isSuites);
   return pageData.getHtml();
}
```

#### 한가지만 해라!
- 함수는 한가지를 해야 한다. 그 한가지를 잘 해야 한다. 그 한 가지만을 해야 한다.

#### 함수 당 추상화 수준은하나로!

#### Switch문
- 추상팩토리에 숨기는 방법(?)

#### 서술적인 이름을 사용하라
- 이름을 정하느라 시간을 들여도 괜찮다.

#### 함수 인수
- 함수에서 이상적인 인수 개수는 0개 이다.
- 4개이상은 특별한 이유가 있어도 사용하면 안된다(?)
- 플래그 인수는 끔찍(?)
- 이항 함수가 무조건 나쁘다는것은 아님, 하지만 그만큼 위험이 따른다는 것을 이해하고 단항 함수로 바꾸도록 애써야한다.

#### 부수 효과를 일으키지 마라!
- 한 가지만 할것같은 함수이름이 두가지를 수행할 때 위험
- 출력 인수

#### 명령과 조회를 분리하라!
```java
if ( set("username", "unclebob") )...
```
- 설정인지 확인인지 애매함
```java
if (attributeExists("username")) {
  setAttribute("username", "unclebob");
  ...
 }
 ```
 #### 오류 코드보다 예외를 사용하라!
 - try ~ catch
 - 의존 자석
 
 #### 반복하지 마라
 - 구조적 프로그래밍
 - AOP
 - COP
 - 중복제거
 
 #### 구조적 프로그래밍
 - 함수는 return 문이 하나여야 한다. 
 - 루프 안에서 break나 continue를 사용해선 안되며 goto는 절대로 안 된다.
 
 #### 함수를 어떻게 짤까?
 - 처음부터 잘 짤 순 없다 그저 고처나갈 
