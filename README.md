## 0️⃣ 과제 안내

> **도서관 책 대출** 기능 구현하기

### 사용 기술

- Java 17
- Junit5, AssertJ (테스트 코드 작성시 사용)

### 기능 요구사항

- [ ] 도서관은 책을 가질 수 있습니다.
- [ ]  도서관은 생성될 때 생성자를 이용해 책이 추가된 채로 생성될 수 있습니다.
- [ ] 책은 다음과 같은 속성을 지닙니다.
    - 책 제목, 저자, ISBN(국제표준도서번호), 대출가능여부
- [ ] 도서관 이용자는 도서관에서 책을 빌릴 수 있습니다.
- [ ] 도서관 이용자는 빌린 책을 반납할 수 있습니다.
- [ ] 도서관은 현재 책들의 목록을 대출 가능 도서와 대출 불가능 도서로 나누어 조회할 수 있습니다. 조회할 때는 다음 속성을 출력해야 합니다.
    - 책 제목, 저자, ISBN, 대출자의 이름
- [ ] 도서관 이용자는 현재 빌린 도서를 조회할 수 있습니다.

### 제한 사항

- [ ] 한 사람은 최대 2권까지의 책을 빌릴 수 있습니다.
- [ ] 이미 다른 사람이 대출한 책은 반납되기 전까지 대출할 수 없습니다.
- [ ] 이용자는 자신이 빌리지 않은 책을 반납할 수 없습니다.

### 코드 작성 시 유의사항
- [ ] 클래스별로 파일을 구분해야합니다.
- [ ] 캡슐화가 이루어져야 합니다.
- [ ] 패키지, 변수, 메서드 작성시에는 꼭 그에 알맞은 네이밍 컨벤션을 따라야 합니다.

<br>

## 1️⃣ 제출 방법

1. 이 레포지토리를 포크합니다.
2. 본인의 이름으로 브랜치를 만듭니다. (예시: hanul)
3. 메인 함수의 주석을 읽으며 코드를 작성해 주세요.
4. 테스트 코드를 작성해주세요. (선택 사항, 가산점 부여)
5. 3번과 4번 과정을 진행하며 커밋해주세요. (밑 커밋 규칙 참고)
6. 모두 완료한 후 Pull Request를 보내주세요.



## 2️⃣ 평가 기준

| 항목 | 내용 | 비율 |
| --- | --- | --- |
| 코드 가독성 | 코드가 얼마나 술술 잘 읽히는가 | 30% |
| 실행 | 기능이 문제 없이 실행되는가 | 30% |
| 학구열 | 자기주도적으로 모르는 내용을 찾아보며 개발했는가 | 30% |
| 성실성 | 성실한가 | 10% |
| 테스트 | 테스트 코드 작성시 가산점 부여 | 3% (추가) |

<br>


## 3️⃣ 커밋 메시지 규칙

다음 명령어를 사용하면 커밋 템플릿을 통해 커밋 메시지를 작성할 수 있습니다.

```bash
git commit
```

### 형식

커밋 메시지는 머리글, 본문, 바닥글로 구성됩니다.

```html
<머리글>
<!-- 빈 줄 -->
<본문>
<!-- 빈 줄 -->
<바닥글>
```

### 머리글

필수입니다.

```
<유형>: <짧은 요약>
  │         │
  │         └─⫸ 현재, 명령형으로 작성. 마침표 금지.
  │
  └─⫸ 커밋 유형: feat|fix|perf|refactor|test
```

#### 유형

| 유형       | 설명                                                       |
|----------|----------------------------------------------------------|
| feat     | 새로운 기능 추가                                                |
| fix      | 버그 수정                                                    |
| perf     | 성능 개선                                                    |
| refactor | 버그를 수정하거나 기능을 추가하지 않은 코드 리팩토링                            |
| test     | 누락된 테스트 추가 또는 기존 테스트 수정                                  |

#### 요약

변경사항이 "**무엇**"인지 작성합니다.

- 명령형, 현재 시제 사용: "변경함", "변경했음"이 아닌 "변경"으로 작성
- 끝에 마침표(.) 금지
- 한글 사용 권장
- 50자 이내로 작성

### 본문

- 한글 사용 권장
- 한 줄에 72자가 넘지 않도록 주의
- 어떻게 보다는 "무엇"을 "왜" 변경했는지 작성
- 자유로운 형식으로 작성

### 바닥글

선택 사항입니다.

참고 사항이나 추가로 할 말이 있을 떄 작성합니다.


### 명령어 예시
```bash
git commit -m "feat :: 도서관 객체
- ~~ 구체적인 설명
"
```

## 4️⃣참고

다음 글을 참고하면서 진행해주세요!<br>
꼭 이 글이 아니더라도, 다른 글들을 참고하면서 해도 괜찮습니다.<br>

> **포크, 브랜치, Pull Request가 뭔지 모르겠다면?** <br>
[Git을 이용한 협업: Fork 부터 Pull Request 까지](https://seungwubaek.github.io/tools/git/contributing_using_pull_request/)

> **테스트 코드 작성 방법** <br>
[IntelliJ에서 JUnit 사용하기](https://velog.io/@wnajsldkf/JUnit-%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0)

> **자바의 네이밍 컨벤션을 모르겠다면?** <br>
[자바 네이밍 규칙 (java 네이밍 컨벤션)](https://thalals.tistory.com/325)