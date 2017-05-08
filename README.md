# BTNcafe 유니티 프로젝트 코딩 컨벤션
BTNcafe에서 진행하는 프로젝트 중 유니티를 기반으로 개발되는 프로젝트는 다음 규칙에 따라야 합니다.

***※ 이 페이지는 계속 업데이트 되므로, 자주 확인하시기 바랍니다.***

## 유니티 리소스 관련

### 파일 명
* 파일명은 모두 대문자로 시작해야 하며, [Camel Case](https://en.wikipedia.org/wiki/Camel_case)로 작성해야 합니다. (이름 중간에 `_`를 사용하지 마십시오.) (예: DeepWater.png)

### 게임 오브젝트
* 씬의 게임 오브젝트는 모두 대문자로 시작해야 하며, [Camel Case](https://en.wikipedia.org/wiki/Camel_case)로 작성해야 합니다. (이름 중간에 `_`를 사용하지 마십시오.)

### 스크립트
* 스크립트의 이름은 대문자로 시작해야 하며, 내장된 클래스의 이름과 동일해야합니다.

## C# 코딩 관련
* 모든 클래스 이름, 변수 명, 함수, 메소드 등은 [Camel Case](https://en.wikipedia.org/wiki/Camel_case)로 작성해야 합니다. (이름 중간에 `_`를 사용하지 마십시오.)
* 똑같은 코드를 복사 붙혀넣기 하지 마십시오. 함수 형태로 만드시기 바랍니다.
* 타입을 즉각 알 수 없는 `var`를 사용하지 마십시오.
* 전반적인 코딩 스타일은 모두 비주얼 스튜디오의 제안을 따릅니다. 비주얼 스튜디오 상에서 모든 코드를 `Ctrl + C`, `Ctrl + V` 했을 때 맞추어지는 코드입니다.
* 변수 초기화는 `Start` 함수에서 하지 말고 선언 즉시 초기화합니다.
* `if` 내부 조건문이 너무 길다면 칸을 내려 적당히 분리해줍니다.

`for`, `if`, `while`등의 뒤에는 한칸 띄웁니다.
```
// 잘못된 경우
if(true)

// 잘된 경우
if (true)
```

### 연산자
쉼표나 연산자 사이는 무조건 띄어 씁니다.
```
// 잘못된 경우
1+2+3

// 잘된 경우
1 + 2 + 3
```

### 클래스
* 클래스 이름은 반드시 대문자로 시작해야 합니다.
* 스크립트의 이름 또한 대문자로 시작해야 하며, 내장된 클래스의 이름과 동일해야합니다.
* 모든 클래스 내 변수 및 함수들은 `public`, `protected`, `private`등 범위 지정자를 반드시 작성합니다.

### 함수
* 함수의 이름은 대문자로 시작해야 합니다.
* 파라미터의 이름은 소문자로 시작해야 합니다.
* `Start` 및 `Update` 등 유니티 기본 함수는 모두 `private`로 선언합니다.
* 함수와 함수 선언 사이를 붙히지 않고 한칸 띄어줍니다.

### 변수
* 모든 클래스 내 변수는 소문자로 시작해야 합니다.

변수 명을 의미가 있는 이름으로 지어야 합니다. `a`, `b`, `c` 등의 변수를 만들지 마시기 바랍니다. 단, 반복문의 인덱스를 위한 `i`, `j`, `k` 등은 편의 상 용인됩니다.

```c#
// 이렇게 작성하지 마시기 바랍니다.
int a = 123;

// 이렇게 의미를 꼭 부여하시기 바랍니다.
int npcLevel = 123;
```

### 주석
* 너무나 당연한 내용에 대해서는 결코 주석을 달지 않습니다.

주석을 작성할 때 `//` 뒤에는 반드시 스페이스를 하나 붙힙니다.

```c#
//이렇게 쓰지 마십시오.
// 이렇게 쓰십시오.
```

주석은 코드 오른쪽이 아닌, 위에 작성합니다.
```c#
int number = 1; // 이렇게 쓰지 마십시오.

// 이렇게 쓰십시오.
int number = 1;
```

### 중괄호
모든 중괄호는 반드시 한칸 내려서 작성합니다.
```c#
if (true)
{
    // 이렇게 작성합니다.
}
```