# Episode 2

**과목(Subject)**: `[CS311]` 전산기조직  
**교재 범위(Scope)**: `[COD]` Chapter 2

> **알림**: KnowHow Archive 컴퓨터 아키텍쳐 시리즈는 여러 교재를 바탕으로 하고 있습니다. 참고한 교재와 해당하는 코드의 목록은 다음과 같습니다:
> * Computer Organization and Design MIPS Edition, 6th Edition [COD]
> * Computer Architecture: A Quantitative Approach, 6th Edition [CAQ]
> * Operating System Concepts, 10th Edition [OSC]  
>
> 세 권이 모든 에피소드에 쓰이는 것은 아닙니다. 각 에피소드의 교재 범위는 보통 책의 한 챕터 이하인 경우가 많습니다.

**Table of Contents**
- [Episode 2](#episode-2)
  - [서론](#서론)
  - [하드웨어 연산](#하드웨어-연산)

___  

## 서론
**교재 범위(Scope)**: `[COD]` 2.1
컴퓨터에 일을 시키려면 컴퓨터의 언어로 말을 해야 합니다.
> ###  ✔용어
> **명령어(Instruction)**: 컴퓨터 언어의 단어  
> **명령어 집합(Instruction Set (Architecture), ISA)**: 컴퓨터 언어의 어휘 (명령어의 집합)

우리가 사용하는 [COD] 교재가 MIPS를 기반으로 하기 때문에, 본 시리즈에서도 MIPS를 사용할 예정입니다. **MIPS**는 ISA의 하나로, x86와 같은 더 널리 사용되는 ISA에 비해 간단하기 때문에 최근에는 교육용으로 많이 사용되는 편입니다.  

에피소드 2와 3에서는 명령어의 표현 방식을 배움으로써 **내장 프로그램 개념**을 이해하고, 컴퓨터 언어의 구사 능력을 연마하며, 프로그래밍 언어와 컴파일러 최적화가 성능에 미치는 영향, ISA의 발달 과정, 그리고 다른 컴퓨터 언어를 살펴볼 것입니다.

> ### ✔용어
> **내장 프로그램 개념**: 여러 종류의 데이터와 명령어를 메모리에 숫자로 저장할 수 있다는 개념. 이에 따라 내장 프로그램 컴퓨터가 만들어졌음.

___  

## 하드웨어 연산 
**교재 범위(Scope)**: `[COD]` 2.2

MIPS를 비롯한 모든 ISA는 산술 연산을 수행하는 산술 명령어가 있습니다. MIPS의 산술 명령어는 다음과 같이 생겼습니다.

```
add a, b, c   
```
이 명령어는 b와 c를 더해 a에 넣으라는 뜻입니다. 즉, `a=b+c`와 같습니다.

`add`를 