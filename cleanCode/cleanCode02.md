## 의미 있는 이름

#### 의도를 분명히 밝혀라
```java
public List<Cell> getFlaggedCells() {
  List<Cell> flaggedCells = new ArrayList<Cell>();
  for ( Cell cell : gameBoard )
    if ( cell.isFlagged() )
      flaggedCells.add(cell);
  return flaggedCells;
}
```
- 단순히 이름만 고쳐도 함수가 하는 일을 이해하기 쉽다.

#### 그릇된 정보를 피하라
- 헷갈리는 단어를 사용하지 말라는 느낌(?)

#### 의미 있게 구분하라
- 읽는 사람이 차이를 알도록 이름을 지어라
- 잘못된 예
```java
getActiveAccount();
getActiveAccounts();
getActiveAccountInfo();
```
#### 발음하기 쉬운 이름을 사용하라
- 발음하기 어려운 이름은 토론하기 어렵다.

#### 검색하기 쉬운 이름을 사용하라
- 숫자보다 상수를 사용하면 검색이 쉬워짐

#### 인코딩을 피하라

#### 자신의 기억력을 자랑하지 마라

#### 클래스 이름
- 명사나 명사구가 적합하다
- 동사는 피하자

#### 메서드 이름
- 동사나 동사구가 적합
- javabean 표준에 따라 값 앞에 get, set, is를 붙인다.
- 생성자를 중복정의 할 때는 정적 팩토리 메서드를 사용한다. 메서드는 인수를 설명하는 이름을 사용한다.
- [팩토리 메서드 관련](https://tecoble.techcourse.co.kr/post/2020-05-26-static-factory-method/)

#### 기발한 이름은 피하라

#### 한 개념에 한 단어를 사용하라
- 클래스마다 fetch, retrieve, get 으로 제각각 부르면 혼란

#### 말장난을 하지 마라
- 함수안에 기능이 비슷하면 같은 함수명을 하지만 전혀 다른 기능을 한다면 다른 이름으로 해야한다.
- add, insert와 같이

#### 해법 영역에서 가져온 이름을 사용하라
- 기술 개념에는 기술 이름이 가장 적합한 선택이다.

#### 문제 영역에서 가져온 이름을 사용하라

#### 의미 있는 맥락을 추가하라
#### 불필요한 맥락을 없애라
