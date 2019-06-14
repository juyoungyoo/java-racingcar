# 자동차 경주 게임
## 진행 방법
* 자동차 경주 게임 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)


---
# 문자열 사칙 연산 계산기

## 기능 요구사항 
사용자가 입력한 문자열 값에 따라 사칙연산을 수행할 수 있는 계산기를 구현해야 한다.
문자열 계산기는 사칙연산의 계산 우선순위가 아닌 입력 값에 따라 계산 순서가 결정된다. 즉, 수학에서는 곱셈, 나눗셈이 덧셈, 뺄셈 보다 먼저 계산해야 하지만 이를 무시한다.
예를 들어 "2 + 3 * 4 / 2"와 같은 문자열을 입력할 경우 2 + 3 * 4 / 2 실행 결과인 10을 출력해야 한다.

## 요구사항
- [x] 덧셈
- [x] 뺄셈
- [x] 곱하기
- [x] 나누기
- [x] 덧셈 + 뺄셈 + 나누기 + 곱하기 (모든 연산이 포함된 기능 구현) 
- [x] 문자열을 공백기준으로 split 한다.
  - [ ] 공백이 아닌 다른 특수문자가 들어 올 경우 Exception
  - [x] 입력 값이 null 이거나 빈 문자열 일 경우 Exception
  - [ ] 사칙연산의 기호가 아닌 경우 IllegalArgumentException
  
반복적인 패턴을 찾아 반복문으로 구현한다.
공백 문자열을 빈 공백 문자로 분리하려면 String 클래스의 split(" ") 메소드를 활용한다.
