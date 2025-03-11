✅ 객체지향 프로그래밍(OOP) 기초 개념 도입

1. 클래스(Class)란?
2. 메서드(Method) 사용법
3. static 메서드 활용 (함수형 스타일로 문제 풀이 가능하게 연습)

## 1. 클래스(Class)란?

클래스는 객체를 생성하는 설계도(틀) 역할.

```java
class Car {  // Car 클래스 선언
    String brand;  // 필드 (변수)
    int speed;  // 필드 (변수)

    void drive() {  // 메서드 (함수)
        System.out.println(brand + "가 " + speed + "km/h로 달립니다.");
    }
}
```

객체(Object)란?

객체는 클래스(설계도)를 기반으로 생성된 실체(인스턴스).
만들어진 하나의 클래스를 사용해서 여러 개의 객체들을 생성 가능.

```java
public class Main {
    public static void main(String[] args) {
        Car myCar = new Car();  // Car 객체 생성
        myCar.brand = "BMW";  // 필드 값 설정
        myCar.speed = 120;  

        myCar.drive();  // 메서드 호출
    }
}
```

## 2. 메서드(Method)란?

메서드는 특정 동작(기능)을 수행하는 코드 블록.

```java
class Calculator {
    // 메서드 선언
    int add(int a, int b) {
        return a + b;  // 두 수의 합 반환
    }
}
```

```java
public class Main {
    public static void main(String[] args) {
        Calculator calc = new Calculator();  // 객체 생성
        int result = calc.add(5, 7);  // 메서드 호출
        System.out.println("결과: " + result);
    }
}
```

## 3. static 메서드 활용

static 메서드: 클래스를 사용할 때, 객체를 생성하지 않고 바로 호출할 수 있는 메서드.
즉, 객체를 만들지 않고도 사용 가능한 메서드.

```java
class MathUtil {
    public static int square(int num) {
        return num * num;
    }
}
```

```java
public class Main {
    public static void main(String[] args) {
        int squared = MathUtil.square(4);  // 객체 생성 없이 바로 호출
        System.out.println("4의 제곱: " + squared);
    }
}
```

static 메서드를 활용한 문제 풀이 연습

문제: 배열의 최대값 찾기

```java
class MathUtil {
    public static int findMax(int[] arr) {
        int max = arr[0];
        for (int num : arr) {
            if (num > max) {
                max = num;
            }
        }
        return max;
    }
}

public class Main {
    public static void main(String[] args) {
        int[] numbers = {3, 7, 2, 9, 5};
        System.out.println("최대값: " + MathUtil.findMax(numbers));
    }
}
```

## 요약

클래스(Class) 객체를 생성하는 설계도	class Car {}
객체(Object) 클래스에서 만들어진 실체	Car myCar = new Car();
메서드(Method) 특정 기능을 수행하는 코드 블록	int add(int a, int b) { return a + b; }
static 메서드	객체 생성 없이 호출 가능	public static int square(int num) {}












