# kotlin-lotto

## 계산기

### 기능 요구 사항

* [x] 쉼표(,) 또는 콜론(:)을 구분자로 가지는 문자열을 전달하는 경우 구분자를 기준으로 분리한 각 숫자의 합을 반환 (예: “” => 0, "1,2" => 3, "1,2,3" => 6, “1,2:3” => 6)
* [x] 앞의 기본 구분자(쉼표, 콜론) 외에 커스텀 구분자를 지정할 수 있다. 커스텀 구분자는 문자열 앞부분의 “//”와 “\n” 사이에 위치하는 문자를 커스텀 구분자로 사용한다. 예를 들어 “//;\n1;2;3”과 같이 값을 입력할 경우 커스텀 구분자는 세미콜론(;)이며, 결과 값은 6이 반환되어야 한다.
* [x] 문자열 계산기에 숫자 이외의 값 또는 음수를 전달하는 경우 `RuntimeException` 예외를 throw 한다.


## 로또(자동)

### 기능 요구 사항

* [x] 로또는 중복 없는 숫자 6개(1~45)로 구성된다.
* [x] 로또는 당첨 번호와 일치하는 숫자의 개수를 알려준다.
* [x] 로또 상점은 받은 금액으로 로또를 최대한 많이 발급한다 - 로또 가격 : 1000원.
* 로또 게임은 아래와 같은 순서로 진행된다.
    * [ ] 금액을 입력받는다.
    * [ ] 구매한 로또들의 번호를 출력한다.
    * [ ] 당첨 번호를 입력받는다.
    * [ ] 당첨 통계를 보여준다.
* [ ] 로또 게임은 당첨 번호를 받아 구매한 로또들의 당첨 통계를 집계한다.
* [ ] 로또 게임은 당첨 통계와 구입 금액을 통해 총 수익률을 계산한다.
