hello-world

# Mark-Down 사용법
- Git에서 보면 *.md로 된 File이 있음(README.md) -> MarkDown 문법으로된 ASCII문서임
- .adoc(ASCII Documents)등이 비슷한 MarkDown 문서임
  - 작성 : 메모장, VS-Code(VS-Codium)등 ASCII-Editor에서 작성 가능

### 코드 블럭 작성 <code>｀</code>를 사용
- 여러줄 코드를 작성시 <code>｀</code> 기호 또는 <code>~</code>를 세번 쓴 코드 블럭 사용가능
<pre>~~~cpp
블럭으로 표현 시
void function(){}
~~~</pre>
~~~cpp
블럭으로 표현 시
void function(){}
~~~

#### 제목 => HTML <code>&lt;h1&gt;</code>, <code>&lt;h2&gt;</code>, ~ <code>&lt;h6&gt;</code> 태그로 변환되어 Header<"제목">을 표현
- "#"으로 입력 => <code>#제목</code> -> <code>&lt;h1&gt;</code>, <code>##제목</code> -> <code>&lt;h2&gt;</code>, <code>###제목</code> -> <code>&lt;h3&gt;</code> ...<code>######제목</code> -> <code>&lt;h6&gt;</code>

#### 강조 => <code>&lt;em&gt;</code> 기울임, <code>&lt;strong&gt;</code> 두꺼움, <code>&lt;del&gt;</code> 취소선

#### 목록 => <code>&lt;ol&gt;</code>, <code>&lt;ul&gt;</code>, <code>&lt;li&gt;</code> 태그로 변환되는 목록(list)을 나타냄
- <code> 1.</code>로 시작시 <code>&lt;ol&gt;</code> 변환
- <code> - </code>로 시작시 <code>&lt;ul&gt;</code> 변환

#### 링크 => <code>&lt;a&gt;</code>
- `[이름](링크)` => `[google](https://www.google.com)` => 결과 : [google](https://www.google.com)
- `[이름](링크"설명")`

#### 이미지 => `![이름](링크 "설명")` => 이미지 출력됨
- `<img>`로 변환되는 `'이미지(images)'`를 표현
<pre>
![대체텍스트](이미지주소)
![대체텍스트](이미지주소 "설명")
![대체텍스트][참조]

[참조]: 이미지주소
[참조]: 이미지주소 "설명"
  
--------------------------------------------------------------------------------------
  
![대체 텍스트(Alternative Text)](https://picsum.photos/1000/500 "링크 설명(Title)")
![이미지입니다!][Image]

[Image]: https://picsum.photos/500/400 "이미지입니다!"
</pre>
예제 결과물 입니다.
![대체 텍스트(Alternative Text)](https://picsum.photos/1000/500 "링크 설명(Title)")
![이미지입니다!][Image]

[Image]: https://picsum.photos/500/300 "이미지입니다!"
