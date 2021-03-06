# HTML

## 개요
HTML 이란 웹 페이지와 그 내용을 구조화하기 위해 사용하는 코드이다. 예를 들면, 컨텐츠는 여러 개의 문단, 글 머리 목록이 구조화된 것이거나 사진이나 데이터 테이블일 수도 있다.

HTML 은 진짜 프로그래밍 언어가 아니다. 컨텐츠에 구조를 정의하기 위한 마크업 언어이다. 컨텐츠의 서로 다른 부분들을 wrap하거나 enclose하여 다른 형식으로 보이게하거나 특정한 방식으로 동작하도록 하는 일련의 elements로 이루어져 있다.

## HTML element

`<p>Hello World!</p>`

- \<p> : 여는 태그
- \</p> : 닫는 태그
- Hello World! : 컨텐츠
- element : 여는 태그 +  닫는 태그 + 컨텐츠

### Attribute
`<p class="editor-note">Hello World!</p>`

속성은 실제로 컨텐츠로 표시되길 원하지 않는 추가적인 정보를 담고 있다.
위 코드에서 class속성을 이용해 나중에 해당 요소를 특정해 스타일이나 다른 정보를 설정할 때 사용할 수 잇는 식별자를 지정 할 수 있다.

Attiribute가 항상 가져야 하는것
1. element 이름과 attribute 사이에 공백이 있어야 한다.
2. attribute 이름 뒤에는 =가 와야 한다.
3. attribute 값 앞 뒤에 열고 닫는 인용부호(" ")가 있어야 한다. ''도 상관없지만 HTML attribute에는 의례적으로 ""를 더 많이 쓴다.

### Element nesting
`<p>내 고양이는 <strong>아주</strong> 고약해.</p>`
Element를 다른 Element 안에 놓을 수 있다. 이를 nesting 이라고 부른다.

### Empty elements
`<img src="images/example.png" alt="exmaple" />`
해당 element는 두 개의 attiribute를 포함하고 있으나 닫는 태그가 없다. 이러한 컨텐츠가 없는 element를 empty elements라고 부른다.

------------------------------------------------------------------------------

## Block versus inline elements

HTML 에는 크게 두가지 종류의 요소가 있다. 블록 레벨 요소와 인라인 요소 이다.

- 블록 레벨 요소는 웹페이지 상에 블록을 만드는 요소이다. 블록 레벨 요소는 앞뒤 요소 사이에 새로운 줄을 만들고 나타낸다. 블록 레벨 요소는 인라인 요소에 중첩될 수 없다. 블록 레벨 요소간 중첩은 가능하다.

- 인라인 요소는 항상 블록 레벨 요소내에 포함되어 있다. 인라인 요소는 문서의 한 다락같은 큰 범위에는 적용될 수 없고 문장, 단어 같은 작은 부분에 대해서만 적용될 수 있다. 인라인 요소는 새로운 줄을 만들어 내지 않는다.

## 기타

- 빈 요소를 닫을 필요는 없으나 엄격한 유효성 검사를 위해 올바르게 닫는 습관이 필요하다.
- 항상 소문자 태그를 사용한다.
- 닫는 태그를 반드시 사용한다.
- attribute 값을 항상 ""로 묶는다. (그 안에 따옴표를 사용 할 일이 있다면 ''로 사용한다.)
<br />
- 제목을 나타낼 때에는 h 태그를 사용한다.
- 내용이 분리되거나 변경 될 때에는 hr 태그를 사용한다.
- img 태그를 사용할 때 반드시 alt 속성을 사용한다. (올바른 웹페이지 검증을 위해)
- img 태그를 사용할 때 width와 height 속성을 적어두는 것이 좋다. (style 속성으로)
- 레이아웃 네가지 (float, flexbox, framework, grid)
- 레이아웃으로 절때 table을 사용하지 않는다.
