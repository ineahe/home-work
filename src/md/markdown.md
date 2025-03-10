# 마크다운(Markdown)이란?

마크다운(Markdown)은 텍스트 기반의 언어로 태그나 기호를 사용하여 제목, 목록, 링크, 이미지 등의 서식을 지정하는 간단하고 직관적인 방법.

## 마크다운의 특징

- 문법이 간결하여 읽기 쉽고 작성하기 쉬움.
- HTML로 변환이 가능해 웹에서 쉽게 공유할 수 있음.
- 텍스트로 저장되기 때문에 용량이 적음.
- 문서화, 블로그 작성, 웹 콘텐츠 등에 많이 사용됨.
- 지원하는 프로그램과 플랫폼이 많음. (Github, Discord 등)

---

<br>

# 마크다운(Markdown) 문법

## 1️⃣ 제목(Header)

HTML의 `<h1> <h2> <h3> <h4> <h5> <h6>` 와 같은 역할을 하며 `#`개수에 따라 제목을 나타낼 수 있음.

```
# h1 제목 1
## h2 제목 2
### h3 제목 3
#### h4 제목 4
##### h5 제목 5
###### h6 제목 6

* h1과 h2는 아래처럼 사용도 가능함.
큰제목1
===
부제목2
---
```

> # h1 제목 1
>
> ## h2 제목 2
>
> ### h3 제목 3
>
> #### h4 제목 4
>
> ##### h5 제목 5
>
> ###### h6 제목 6
>
> # 큰제목1
>
> ## 부제목2

<br>

## 2️⃣ 목록(List)

`<ol> <ul> <li>`와 같은 역할을 함.

- 순서 있는 목록 (`1.`, `.` 사용)

```
1. 첫번째
2. 두번째
3. 세번째
```

> 1. 첫번째
> 2. 두번째
> 3. 세번째

- 순서 없는 목록 (`-`, `*`, `+` 사용)

```
- 빼기
* 별
+ 더하기
    + 더하기 2
        + 더하기 3
```

> - 빼기
>
> * 별
>
> - 더하기
>   - 더하기 2
>     - 더하기 3

<br>

## 3️⃣ 강조(Emphasis)

`<em> <strong> <del>` 과 같은 역할을 함.

```
 기울여 쓰기(italic) : * 또는 _ 로 감싼 텍스트
 두껍게 쓰기(bold) : ** 또는 __ 로 감싼 텍스트
 취소선 : ~~ 로 감싼 텍스트
```

> _italic_ _em_ <br> **bold** **strong** <br> ~~del~~

<br>

## 4️⃣ 인용문(Blockquotes)

`>`기호를 사용하고 `<blockquote>`와 같은 역할을 하며 중첩해서 사용 가능함.

```
> 인용문
>
> > 중첩 인용문
> >
> > > 중첩 인용문의 인용
```

> 인용문
>
> > 중첩 인용문
> >
> > > 중첩 인용문의 인용

<br>

## 5️⃣ 줄바꿈(line break)

- 문장 마지막에서 띄어쓰기 2번 이상 입력해서 사용함.
- `<br>` 태그를 사용함.

```
동해물과 백두산이 마르고 닳도록  <!--띄어쓰기 2번-->
하느님이 보우하사 우리나라 만세<br>
애국가
```

> 동해물과 백두산이 마르고 닳도록  
> 하느님이 보우하사 우리나라 만세 <br>
> 애국가

<br>

## 6️⃣ 코드 블록(Code Block)

텍스트를 앞뒤로 `` ` `` 기호로 감싸 사용함. 코드 블록 내에서는 마크다운 문법이 적용되지 않음.

- **인라인 코드** : `` `코드` ``

한 단어나 일부 문장만 코드로 표시하고자 할 때 사용함.

```
`애국가` `대한 사람 대한으로`
```

> `애국가` `대한 사람 대한으로`

<br>

- **블록 코드** : ` ``` ` 를 사용함.

`` ` `` 기호를 3번 이상 입력하고 언어 이름을 명시해 코드 '블록(Block)'을 표현함. <br>
`` ` `` 의 시작 개수와 종료 개수는 같아야 함.

````
```javascript
function test() {
  console.log("언어에 맞춰 강조됨");
}
```
````

> ```javascript
> function test() {
>   console.log("언어에 맞춰 강조됨");
> }
> ```

<br>

## 7️⃣ 수평선(Horizontal Rule)

3개 이상의 `-` `*` `_` 을 입력하여 사용하고 `<hr>`과 같은 역할을 함.

```
---
***
___
```

> ---
>
> ---
>
> ---

<br>

## 8️⃣ 링크(Link)

`<a>`와 같은 역할을 함.

- **링크 기본 문법** : `[링크설명](url)` 방식으로 표현하며 url을 `keyword`로 표현함.

```
[Google](https://google.com)
[Naver](https://naver.com "여기에 쓰는 링크 설명은 사용자에게 보이지 않음")
```

> [Google](https://google.com)  
> [Naver](https://naver.com "여기에 쓰는 링크 설명은 사용자에게 보이지 않음")

- **참조 링크** : 문장에서 참조 부분에 사이트를 연결하고자 할 때 사용함.

```
[이름][참조]

문서 안에서 [참조 링크]를 사용할 수 있음.

[참조]: 링크
[참조]: 링크 "설명"
```

> [참조 구글][1]
>
> 문서 안에서 [참조 링크]를 사용할 수 있음.
>
> [1]: https://www.google.com
> [참조 링크]: https://naver.com "문서 안에 참조된 링크"

- **자동 연결** : 일반 URL이나 이메일 주소, 꺾쇠 괄호(`< >`)안의 URL은 자동으로 링크를 생성함.

```
구글 : https://google.com
네이버 : <https://naver.com>
이메일 : address@example.com
```

> 구글 : https://google.com <br>
> 네이버 : <https://naver.com> <br>
> 이메일 : address@example.com

<br>

## 9️⃣ 이미지(Image)

`<img>`와 같은 역할을 하며 링크와 사용법이 비슷하지만 맨 앞에 `!`를 추가함.

- **인라인 이미지** : 이미지 파일 경로로 이미지 직접 삽입

```
![텍스트](/test.png)
```

> ![폼푸그립톡](../assets/images/pomgrip.jpg)

- **링크 이미지** : 이미지 URL을 통한 이미지 삽입

```
![텍스트](이미지 URL)
![텍스트](이미지 URL "설명")
![텍스트][참조]

[참조]: 이미지 주소
[참조]: 이미지 주소 "설명"

* 이미지에 링크 추가 : 마크다운 이미지 문법 코드를 링크 문법 코드로 감싸줌.

[![텍스트](이미지 URL)](링크)
```

> ![폼폼푸린](https://www.sanrio.co.jp/special/characterranking/2022/assets/img/common/characters/pompompurin.png)

> ![하트폼푸](https://www.sanrio.co.jp/special/characterranking/2024/assets/img/common/characters/pompompurin.png "하트날리는폼폼푸린")

> [![상받은폼푸][2]](https://www.sanrio.co.jp/special/characterranking/2022/ko/)

> [2]: https://www.sanrio.co.jp/special/characterranking/2022/assets/img/result_opening/best2.png "폼푸가상받았어요"

<br>

## 🔟 표(Table)

`<table>`과 같은 역할을 함.

- **기본 테이블** : 3개 이상의 `-`을 사용해 행을 구분하며 `|` 버티컬 바를 사용해 열을 구분함.

  ```
  | 헤더1 | 헤더2 | 헤더3 |
  | ---   | ---   | ---   |
  | 셀1   | 셀2   | 셀3   |
  | 셀4   | 셀5   | 셀6   |
  | 셀7   | 셀8  | 셀9  |
  ```

> | 헤더1 | 헤더2 | 헤더3 |
> | ----- | ----- | ----- |
> | 셀1   | 셀2   | 셀3   |
> | 셀4   | 셀5   | 셀6   |
> | 셀7   | 셀8   | 셀9   |

- **정렬된 테이블** : 헤더의 `-`에 `:` 콜론을 사용해 셀 안의 내용을 정렬할 수 있음.

  ```
  | 헤더1 | 헤더2  | 헤더3  |
  | :---  | :---:  | ---:   |
  | Left  | Center | Right  |
  | 1     | 2      | 3      |
  | 4     | 5      | 6      |
  | 7     | 8      | 9      |
  ```

> | 헤더1 | 헤더2  | 헤더3 |
> | :---- | :----: | ----: |
> | Left  | Center | Right |
> | 1     |   2    |     3 |
> | 4     |   5    |     6 |
> | 7     |   8    |     9 |

<br>

## ⏸️ 체크 리스트

- 줄 앞에 - [x]를 써서 완료된 리스트를 표시함.
- 줄 앞에 - [ ]를 써서 미완료된 리스트를 표시함.

  ```
  - [x] 완료된 리스트
  - [ ] 미완료된 리스트
  ```

> - [x] 완료된 리스트
> - [ ] 미완료된 리스트
