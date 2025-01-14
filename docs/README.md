### 기능 목록

1. 사용자가 지불할 금액을 입력한다.
2. 입력값 검증을 수행한다. 잘못된 값이 입력되면 `IllegalArgumentException`를 출력한다.
    - 1000원으로 나누어 떨어지지 않는 경우 예외 처리
    - 수가 아닌 문자가 입력되었을 경우에도 예외 처리
3. 구매한 금액에 맞게 로또를 발행한다.
   로또 발행용 숫자를 6개 뽑는데, 이때 1~45중에서 중복되지 않는 수만 뽑는다.
   한 로또용지 안에서의 수는 중복될 수 없지만, 서로 다른 로또용지의 수는 중복될 수 있다.
   그 후에 발행된 로또 번호를 모두 출력한다.
4. 당첨번호용 숫자를 6개 입력받는다.
   마찬가지로 1~45 중 중복되지 않는 수만 입력 받는다.
    - 수의 범위가 1~45를 넘겼다면 예외 : `LottoValidator`
    - 쉼표로 입력 문자열을 나눌 수 없어도 예외 : `InputValidator`
    - 6개 이상의 수를 입력해도 예외 : `LottoValidator`
    - 수가 아닌 문자가 입력되었을 경우에도 예외 : `InputValidator`
    - 중복되는 수가 있어도 예외 : `LottoValidator`
5. 보너스 번호 1개를 입력받는다.
   1~45 중, 이전에 뽑은 6개의 숫자와 중복되지 않아야 한다.
    - 수의 범위가 1~45를 넘겼다면 예외 : `LottoValidator`
    - 한 개 이상의 수를 입력해도 예외 : `InputValidator`
    - 수가 아닌 문자가 입력되었을 경우에도 예외 : `InputValidator`
    - 중복되는 수가 있어도 예외 : `LottoValidator`
6. 사용자가 구매한 로또 번호와 당첨 번호를 비교/대조한다.
7. 당첨 기준에 따라 당첨 금액을 계산하고, 당첨 내역을 출력한다.
8. 총 수익률을 계산하여 출력한다.