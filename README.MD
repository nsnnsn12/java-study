# 1주차 과제
## 목차
##### 1. JVM이란 무엇인가
##### 2. 컴파일 하는 방법
##### 3. 실행하는 방법
##### 4. 바이트코드란 무엇인가
##### 5. JIT 컴파일러란 무엇이며 어떻게 동작하는지
##### 6. JVM 구성 요소
##### 7. JDK와 JRE의 차이

## 1. JVM
### 1) JVM이란
자바를 실행하기 위한 가상 기계 <br>
자바를 실행하기 위한 가상 컴퓨터
<br><br>
### 2) 일반 애플리케이션 코드와 자바 애플리케이션의 비교
일반 애플리케이션 코드<br>
(애플리케이션) - (OS) - (하드웨어)

자바 애플리케이션 코드<br>
(자바 애플리케이션) - (JVM) - (OS) - (하드웨어)
<br><br>
JVM을 한 번 더 거치고, 하드웨어에 맞게 완전 컴파일된 상태가 아니기에 실행 시 해석(interpret)되기 때문에 속도 저하<br>
-> 바이트코드(컴파일된 자바코드 - JVM이 이해할 수 있는 기계어, JVM은 바이트코드를 해당 OS의 기계어로 변환, OS로 전달) <br>
하드웨어의 기계어로 바로 변환해주는 JIT컴파일러, 향상된 최적화 기술로 속도 저하 감소

<br><br>
## 2. 컴파일
### 1) 컴파일이란
프로그래밍 언어로 작성한 코드를 기계가 알아들을 수 있도록 다른 언어로 옮기는 작업

### 2) 컴파일 종류
- jsp 파일 : 자동으로 WAS에서 Servlet(java 파일)로 변환 뒤 컴파일(class 파일)<br>
- java 파일 : class 파일로  컴파일
- 리눅스 컴파일 과정 :<br><br>
1	program.c<br>
	전처리기(Preprocessor)<br>
	전처리기 구문(#으로 시작하는 구문)을 처리하는 것<br><br>
2	program.i<br>
	컴파일러(Compiler)<br>
	고수준 언어를 저수준 언어로 나타내는 역할<br>
	(저수준언어 : 기계어와 가장 가까운 언어)<br><br>
3	program.s<br>
	어셈블러(Assembler)<br>
	완전히 기계어로 바꾸어 주는 역할<br><br>
4	program.o<br>
	링커(Linker)<br>
	연결해주는 역할<br>
	여러개의 오브젝트 파일을 하나로 합치거나 라이브러리를 합칠 때 필요<br><br>
5	program.exe<br>

<br><br>
## 3. 실행
### 1) Terminal을 사용한 Java 실행 과정
- Terminal 사용 이유 : <br>
IDE 툴이 어떤 기능을 제공하는지, 소스코드 파일 실행 과정은 어떻게 이루어져있는지 이해하기 위해
#### 1))  java 파일 생성하기
메모장 간단한 소스코드 작성
<br>확장자 .java로 변경
<br>
#### 2)) cmd 창으로 java 실행해보기
경로 입력
<br>
#### 3)) 컴파일
Javac는 자바 개발 키트(JDK)에 포함된 Java Compiler
<br>자바 컴파일러는 .java 파일을 .class로 변경(소스코드를 실행파일로 변환한 것)
<br>.class파일은 binary code로 이루어져 있다
<br>javac classpathTest.java 입력, 오류 없을 시 아무런 메시지 없음
<br>classpathTest.class, Display.class 두 파일이 생김(클래스가 두 개 였기 때문)
<br>
#### 4)) class 파일 실행
.class 파일 실행 시에는 확장자 제외 파일명만 입력
<br>실행시키려면 main method가 있어야함(질문) 왜 main 없으면 안되냐
<br>java ClasspathTest 입력
<br>결과 출력

<br><br>
## 4. 바이트코드


<br><br>
## 5. JIT

<br><br>
## 6. JVM

<br><br>
## 7. JDK와 JRE의 차이

