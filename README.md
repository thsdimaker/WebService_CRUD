# WebService_CRUD
Spring Boot + AWS


# 개발환경

IDE : IntelliJ IDEA(Community) 2020.3

OS : Windows 10

Java 8(jdk-8u281-windows-x64)

Spring Boot 2.4.1

Gradle 6.7.1


# 개발기한

2021.02.17

: 중간 테스트 및 점검


2021.02.09

: AWS 보안그룹 오류 


2021.02.15

: AWS 연동 시작

2021.02.14

: 로그인 서비스 완성 및 

2021.02.11

: 로그인 서비스 구현 시작

2021.02.03 ~ 2021.02.07

: 문서 정리 및 CRUD 로직 복기

2021.02.02

: 한 챕터에서 오류를 찾는데 거의 하루를 다 보냄

2021.01.31

: CRUD 제작 시작

2021.01.29

: 기본 문서 작성 시작


2021.01.28

: 기초 환경 설정 및 원격저장소 연결 성공.


# 시행착오 및 깨달음

0. 초기 세팅부터 버벅였다.

ㄴ > Bundle.gradle 버전에 따라 지원하지 않는 문제 등.

1. 부모디렉터리와 자식디렉토리 분할문제가 잘 안됬었음.

ㄴ > 여기서 한가지 규칙 : 디렉토리는 소문자로 사용한다는것을 깨달음

2. 프로그래밍 언어를 공부 했던 것과 실제 프로젝트를 만드는것과의 괴리감을 느낌.
마치, 

3. Git 커밋을 마음대로 이동해서 병합 실패 등.. 하루를 개인적으로 다보냈다.
뿐만 아니라 mustache에서 조금만 정확히 봤더라면... 하는 아쉬움이 있었다.

4. Git에 대한 정확한 공부(특히 해당 커밋으로 이동 후 다시 병합할 때의 리스크 Reset과 Revert)
쉬운건 없다... 하루를 버리는 이런 날도 있다는걸 깨달았다. 이부분이 진행이 안되면 뒤는 의미가 없기에..

5. Git main브랜치에서 마음대로 checkout 과 reset을 남발하다가 일을 두번하게되었다.
내가 작성하고 있는 Branch가 어디인지 정확히 알아야 하며, main으로 병합 할 때 방법을 정확히 알아야 겠다.

6. 예전 Java기반의 Framework인 Spring을 다뤄봤었을 때 소흘 했던것과 Spring Boot 와의 상호보완을 해나가야겠다.


# Java 관례

클래스와 필드의 이름은 : 명사

메소드의 이름은 : 동사

여러단어로 구성된 이름은 각 단어의 첫 글자를 대문자로 표시

클래스의 이름도 대문자로 표시

Ex)

[이름](클래스 이름은 대문자로 시작하는 명사)

상품재고 클래스 - GoodsStock

[데이터](필드 이름은 소문자로 시작하는 명사)

재고수량 - goodsCode

상품코드 - stockNum

[기능](메소드 이름은 소문자로 시작하는 동사로 지을 것)

재고를 더한다. - addStock()

재고를 뺀다. - subtrackStock()



## 2021.02.02
# 1차 보고서 : 게시판 CRUD(완성)

![s1](https://user-images.githubusercontent.com/59603054/106556114-37111980-6562-11eb-8ff2-004c9a170f64.png)
![s2](https://user-images.githubusercontent.com/59603054/106556117-37a9b000-6562-11eb-912d-7dcdabd20a6a.png)
![s3](https://user-images.githubusercontent.com/59603054/106556119-37a9b000-6562-11eb-80f9-67534fe60776.png)
![s4](https://user-images.githubusercontent.com/59603054/106556104-34162900-6562-11eb-98d2-f6da35445b2d.png)
![s5](https://user-images.githubusercontent.com/59603054/106556106-35475600-6562-11eb-90e4-a855c49af792.png)
![s6](https://user-images.githubusercontent.com/59603054/106556107-35475600-6562-11eb-837a-aa56d15ebe3a.png)
![s7](https://user-images.githubusercontent.com/59603054/106556108-35dfec80-6562-11eb-8ebd-1a82aa4e26a6.png)
![s8](https://user-images.githubusercontent.com/59603054/106556110-35dfec80-6562-11eb-942a-62ff220ae5de.png)
![s9](https://user-images.githubusercontent.com/59603054/106556111-36788300-6562-11eb-9be5-015b693ca2b6.png)
![s10](https://user-images.githubusercontent.com/59603054/106556112-36788300-6562-11eb-9869-d5c78fd9925e.png)
![s11](https://user-images.githubusercontent.com/59603054/106556113-37111980-6562-11eb-97e0-3b895b15eb69.png)





