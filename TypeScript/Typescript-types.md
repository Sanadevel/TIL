# 타입스크립트 타입

## 일반 JS와 TS의 차이점인 타입 시스템!!!

C, JAVA 같은 언어처럼 변수의 타입을 명시해주어야함

> let a = 1
> a = true

같은 문법이 JS에서는 가능하지만 TS에서는 불가능함

오류 내용을 보면

> Type 'boolean' is not assignable to type 'number'.

라고 적혀있는데, 이는 a의 현재 타입이 number이기 때문에 boolean 타입인 true가 할당되지 않는다는 뜻이다.

## TS에서 타입을 명시해주는 방법

### Implicit types (명시적)

> const a : number = 1

간단하게 원래 변수를 만들어주던 방식에서 변수명 뒤에 (: 변수 타입)을 적어주기만 하면 된다.

### Explicit types (암묵적)

근데 **귀찮잖아**
그리고 우리 생각보다 TS는 더 똑똑하기 때문에 원래 변수를 선언해주는 방식처럼 해줘도 자동적으로 추론해 변수의 타입을 알아낸다.

> const a = 1 (이미 a의 타입이 number라는 것을 알고 있다.)

## object
