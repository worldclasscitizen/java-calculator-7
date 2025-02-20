# 📝 기능 명세서

## 🧮 문자열 덧셈 계산기

### ✅ 사용자로부터 문자열을 입력받는다.

- #### 사용자는 문자열을 입력한다.
- #### 입력값은 camp.nextstep.edu.missionutils.Console의 readLine() 메서드를 사용하여 받는다.
- #### 문자열이 공백일 경우, 0을 반환한다.

### ✅ 구분자를 기준으로 문자열에서 요소를 추출한다.

- #### 커스텀 구분자가 포함되어 있는지 판단한다.

    - 입력 문자열의 앞부분이 "//{커스텀_구분자}\n" 형태인지 검사한다.
    - 커스텀 구분자가 존재하는 경우, 이를 저장하여 기본 구분자(쉼표, 콜론)와 함께 사용한다.
    - 커스텀 구분자가 연속으로 입력될 경우, 예외로 처리한다.
    - 커스텀 구분자가 숫자일 경우, 예외로 처리한다.
    - 커스텀 구분자가 공백일 경우, 예외로 처리한다.

- #### 기본 구분자(쉼표, 콜론)와 커스텀 구분자를 기준으로 문자열을 분리하여 리스트를 생성한다.

### ✅ 문자열 요소들을 정수로 변환한다.

- #### 구분자와 숫자 이외의 문자가 포함된 경우, 예외로 처리한다.
- #### 숫자가 실수일 경우, 예외로 처리한다.
- #### 숫자가 int 타입을 넘어가는 큰 수일 경우, 예외로 처리한다.
- #### 숫자가 음수일 경우, 예외로 처리한다.

### ✅ 추출한 숫자들의 합을 계산한다.

### ✅ 숫자의 합을 출력한다.

- #### 계산된 결과를 사용자에게 안내한다.

### ✅ 예외 처리 기능

- #### 커스텀 구분자가 연속으로 입력될 경우, IllegalArgumentException을 발생시키고, 애플리케이션을 종료한다.
- #### 커스텀 구분자가 숫자일 경우, IllegalArgumentException을 발생시키고, 애플리케이션을 종료한다.
- #### 커스텀 구분자가 공백일 경우, IllegalArgumentException을 발생시키고, 애플리케이션을 종료한다.
- #### 문자열에 숫자가 아닌 다른 문자가 포함된 경우, IllegalArgumentException을 발생시키고, 애플리케이션을 종료한다.
- #### 추출한 숫자가 실수일 경우, IllegalArgumentException을 발생시키고, 애플리케이션을 종료한다.
- #### 추출한 숫자가 int 타입을 넘어가는 큰 수일 경우, IllegalArgumentException을 발생시키고, 애플리케이션을 종료한다.
- #### 추출한 숫자가 음수일 경우, IllegalArgumentException을 발생시키고, 애플리케이션을 종료한다.