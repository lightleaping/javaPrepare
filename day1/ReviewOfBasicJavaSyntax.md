## Day 1: Java 기본 문법 & 코딩테스트 환경 세팅

목표:

Java 기본 문법 복습
개발 및 코딩테스트 환경 세팅
간단한 구현 문제 풀이

https://chatgpt.com/c/67c3b615-c754-8011-817f-3f78e4d1d96d 

# 변수와 데이터 타입 (int, String 등)
# 연산자 (산술, 논리, 비교, 대입 연산자)
# 제어문 (if-else, switch-case, for/while 반복문)
# 배열 (1차원 & 2차원 배열 사용법)


## 변수와 데이터 타입 (int, String 등)

변수(Variable): 데이터를 저장하는 공간

선언 방법: 타입 변수명 = 값;
예시: int num = 10;

데이터 타입(Data Types): 변수에 저장할 수 있는 데이터 종류

- 기본 데이터 타입

int: 정수 타입 (예: int num = 10;)
double: 실수 타입 (예: double pi = 3.14;)
char: 문자 타입 (예: char grade = 'A';)
boolean: 참/거짓 값 타입 (예: boolean isActive = true;)
String: 문자열 타입 (예: String message = "Hello, Java!";)

```java
int age = 25;      // 정수형
double weight = 72.5; // 실수형
char grade = 'A';   // 문자형
boolean isStudent = true; // 논리형
String greeting = "Hello, World!"; // 문자열
```

## 연산자 (산술, 논리, 비교, 대입 연산자)

연산자는 변수나 값에 대해 연산을 수행하는 기호.

산술 연산자 (Arithmetic Operators): +, -, *, /, %

```java
int a = 10, b = 5;
int sum = a + b; // 15
int remainder = a % b; // 0
```

비교 연산자 (Relational Operators): ==, !=, <, >, <=, >=

```java
int a = 5, b = 10;
boolean isEqual = a == b; // false
boolean isGreater = a > b; // false
```

논리 연산자 (Logical Operators): && (AND), || (OR), ! (NOT)

```java
boolean x = true, y = false;
boolean result = x && y; // false
boolean orResult = x || y; // true
```

!는 boolean 값의 반대를 취할 때 사용하고,
!=는 두 값이 서로 다른지를 비교할 때 사용합니다.

대입 연산자 (Assignment Operators): =, +=, -=, *=, /=

```java
int a = 5;
a += 3; // a = a + 3 -> 8
a *= 2; // a = a * 2 -> 16
```

## 제어문 (if-else, switch-case, for/while 반복문)

- ### 조건문(if, switch)

- if-else: 조건에 따라 실행

```java
int score = 85;
if (score >= 90) {
    System.out.println("A");
} else if (score >= 80) {
    System.out.println("B");
} else {
    System.out.println("C");
}
```

- switch-case: 여러 가지 값에 대한 조건 분기
```java
char grade = 'B';
switch(grade) {
    case 'A':
        System.out.println("Excellent");
        break;
    case 'B':
        System.out.println("Good");
        break;
    case 'C':
        System.out.println("Average");
        break;
    default:
        System.out.println("Invalid grade");
}
```

- ### 반복문(for, while, do-while)

- for문: 지정된 횟수만큼 반복

```java
for (int i = 1; i <= 5; i++) {
    System.out.println(i); // 1 2 3 4 5
}
```

 - while문: 조건이 참인 동안 반복

```java
int i = 1;
while (i <= 5) {
    System.out.println(i); // 1 2 3 4 5
    i++;
}
```

- do-while문: 최소한 한 번은 실행 후 조건을 체크
```java
int i = 1;
do {
    System.out.println(i); // 1 2 3 4 5
    i++;
} while (i <= 5);
```

## 배열 (1차원 & 2차원 배열 사용법)
배열 (Array): 동일한 타입의 데이터를 순차적으로 저장하는 자료구조

- 배열 선언 및 초기화:
```java
int[] arr = {1, 2, 3, 4, 5}; // 배열 선언 및 초기화
System.out.println(arr[0]); // 1
```

- 배열 크기 및 반복문 사용:
```java
int[] arr = {10, 20, 30, 40, 50};
for (int i = 0; i < arr.length; i++) {
    System.out.println(arr[i]); // 10 20 30 40 50
}
```

```java
int[] numbers = {1, 2, 3, 4, 5};
for (int num : numbers) {
    System.out.println(num);
}
```

- 2차원 배열
```java
int[][] matrix = {{1, 2}, {3, 4}, {5, 6}};
for (int i = 0; i < matrix.length; i++) {
    for (int j = 0; j < matrix[i].length; j++) {
        System.out.print(matrix[i][j] + " "); // 1 2 3 4 5 6
    }
    System.out.println();
}
```

