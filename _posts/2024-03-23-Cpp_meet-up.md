---
layout: post
title: C++ Korea 2024 Meet-up
date: 2024-03-23 00:00 +0900
tags: record 
---

# C++ Korea 2024 Meet-up

> 처음 C++ Korea meet-up에 나와봤다

## OpenCL 프로그램 작성해본 후기 - 박동하님

아직 이해 못한 내용과 주관적인 판단의 색을 구분하자...   

**Open-CL**
가속기-기반 병렬 프로그래밍을 위한 체계

Vcpkg 패키지 매니저 확장을 위해서, window에서 이런 일을 하려면
+ OpenCL, OpenGL과 같은게 필요하다... ?
  
Angle -> OpenCL 로 이전하면ㅇ스스로 오버헤드가 줄지 않을까

여러 학문에 대한 만남과 학습을 통해 대비 해야한다...    

CPU, GPU 가속에 대한 분야

> 메뉴얼부터 읽는다

### OpenCL Architecture - Model

3가지 관점에서 이해하고 싶다
+ 문법
+ 번역기
+ 실행기

Platform model, Execution model

Memory model

### OpenCL Architecture - Platform

Device

Context

### OpenCL Architecture - Runtime

Commnad Queue

Memory object

Sampler

Progrma

Event

### OpenCL의 C

C99 + C11의 일부 기능

OpenCL Model에 맞는 언어 기능만 추가된 형태

OpenCL 프로그래밍에서는 , CPU에 전달하는 코드와 가속기에 전달하는 코드( 가속이 가능한 부분 )가 다르다...

### C++ for OpenCL language

### 실습 계획

메뉴얼의 ERROR 부분 따라하기
+ 컴파일러 오류 메세지와 친해져야 한다!!!!!!!

> 부족한 지식
> Tenser flow
> 가속기가 필요한 GPU? CPU? 뭔지
> Khronos

---

## C++23을 준비하는 개발자를 위한 몇가지 준비사항 - 한상곤 교수님

### C++ 시작하는 개발자를 위하여

> 주니어들과 일 하면서 느낀 것들

### 2023년의 C++

2023년에 진행된ㅂ대부분 업무에 포함된 "프레임워크" `PyTorch`

C++을 사용한느 개발자를 찾을 수 없음

여전히 강력하고, "경제적"인 언어 C++
+ 하지만 다들 이상하게 배움
+ 심지어ㅡ 뱌우지 않았지만 사용도 가능함( C와 코딩테스트 떄문 )

**C++에 대한 오해**

C++은 C가 아니라고 해도 안 믿어줌
+ C++은 C의 슈퍼셋이 아님

21세기에 20세기 C++을 학습   
+ c++26이 논의되는 시점에 최신 C++을 배우자

### 우리가 준비 해야할 것

**CMake**를 배워라

+ C++ 문법보다 먼저 배웁시다
+ VSCode를 사용하지 말고, CLion을 사용하거나 VS를 사용


**Ref**
  + C++ 세미나 ( 박동하님의 영상 )을 참고
  + CppCon 등 영상도 참고

> 프로그래머가 자본을 획득하는 방법이 "코드를 다른 개발자에게 올바르게 전달, 해당 코드를 기반으로 서비스를 만들어서 제공

### 디버깅 없는 IDE는 주의

VSCode 그만 써라

C++은 컴파일러에 따라 동작 방식이 달라진다..   

VS2022라는 전문적인 도구가 개인 사용자에게 무료이다.   

리눅스라면 CLion을 사용해라....

디버거를 이용해서 안을 볼 수 있는 것을 사용해라

**좋은 교재를 선택해라**

C++ auto가 안나오는 책은 일단 덮어라

### 부족한 부분은 youtube나 인프런 등으로 채워라

최근 개설 된 강의만 들어라!!!!!

### 전문가가 되는 법

**C++ 20에 맞춰서 코드를 재작성해라**

진행중인 프로젝트에 간단한 테스트 코드와 패키지 관리자를 추가해라
+ nuget/vcpkg/conan 드을 적용해서 빌드 환경을 비롯해서 배포 환경을 구성

**발표준비를 하지 말고, 발표를 해라**

일단 발표하고, 틀린 점을 수용해라

그 틀린 점을 수용하는 과정을 또 발표해라

전문가가 되고 싶다면, 전문가가 하는 행동을 적극적으로 활용하세요

테스트 코드 등을 적용

~~

### 결론

+ C++은 여전히 강력하고 좋은 언어

+ 실습 및 학습 환경을 통제할 것
  + 좋은게 좋은게 아닐 수 있다
  + CMake 등은 학습 초기 부터 꼼꼼하게 배울 것

+ C++17 이상을 학습할 것

+ 가능함녀 튜토리얼/핸즈온으로 진행
  + 자료구조 등으로 C++을 학습하는 것은 좋은 방법이 아님
  + 프로젝트 기반으로 학습을 진



## AI와 함께하는 페어 프로그래밍 : 개발의 새 지평 - 김용현님

> Copilot을 활용하여 코딩 효율ㅇ과 창의성을 끌어올리기
> AI는 우리 대체될 수 없지만, 우리는 AI를 활용하는 사람에게 대체 될 수 있다.

SSE? MMX?

### GPT를 조금 더 전문성 있게 사용하는 법

Temperature

0에 가까울 수록 정적인 글

1에 가까울 수록 창의적인 글


Conversation

미리 질문을 던지고, 이렇게 답하는 역할이다 라고 말하기


System Role( Optional )

Assistant에 대한 간단한 설명, 성격의 특성, 지켜야 할 지침과 규칙, 참고할 만한 데이터나 정보


### Microsoft Azure OpenAI Studio

에서 gPT 모델을 사용 해볼 수 있다

### Prompt Engineering

주석에다가 AI가 할 일을 적어라


### Github Copilot


## 고성능 컴퓨팅을 위한 COMPILER INFRASTRUCTURE

C++ KOREA

인터프리팅, 컴파일


## QnA

디자인 패턴 중 포인터 임플리멘테이션 정도는 배워라
+ 리팩토링

mook 101, 201 강의 연번에 맞게 학습 추천

오픈소스 프로젝트는 흥미에 맞는걸로 해라

간단한 프로젝트를 진행해 보는 것을 추천
+ 채팅 프로그램 .. 등

취업할 때 포폴운

유연함, 포텐셜, 흡수력이 좋다는걸 어필해라 > 굳이 c++일 필요는 없다

회사마다 다르게 포폴을 전략적으로 준비해라

대기업이라면 짧고 굵게 스샷 뭐 확실하게

스타트업이라면 조금 길어도~

