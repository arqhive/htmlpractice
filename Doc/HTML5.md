# HTML5
W3C가 발표하는 HTML의 최신 버전으로, 2014년 10월 28일 완전히 표준화되었다. 현재 HTML5.2가 최신 표준이다.

HTML5라고 불리우는 개념은 단순히 웹 문서를 작성할 때 사용되는 마크업 랭귀지의 문법적 버전 뿐만 아니라 새로운 DOM API 스펙을 포함하는 것이다.

이전에는 플래시, 실버라이트 등의 외부 플러그인을 통해서만 지원할 수 있던 클라이언트 사이드에서의 사용자 인터페이스를 위한 기능들의 상당수를 브라우저 자체의 기능을 이용해 구현할 수 있게 되었다.

## HTML5 변경 사항

### 선언문
이전 버전의 HTML과 XHTML이 유효성 검사를 위한 선언문이 쓸데없이 길었던 반면, HTML5에서는 간단한게 몇 자만 적으면 된다.

`<!DOCTYPE html>`
HTML 문법을 사용할 때는 위 선언문을 반드시 적어야 한다.

### Semantic Tag
HTML5 에서는 시맨틱 웹을 중요하시여 여러가지 태그를 새롭게 만들었다. 이러한 태그들을 시맨틱 태그라고 한다.

시맨틱 태그를 사용한 레이아웃은 컴퓨터가 읽어낼 수 있다. 이게 무슨 말이냐면, 검색 사이트에서 어디가 내용인지를 알 수 있어서 검색 노출을 용이하게 하고, 궁극적으로 눈으로 페이지를 볼 수 없는 사람들에게 사이트의 어디가 본문인지 아닌지 알려줄 수 있다는 장점이 있다.

#### \<header>
일반적으로 페이지나 해당 섹션의 가장 윗부분에 위치한다. 페이지 맨 위에 쓸 때는 사이트의 제목이 보통 들어가며, 선택적으로 상단바나 검색창 등이 안에 들어갈 수 있다. section이나 article, aside 등으로 묶어놓은 섹션 안의 헤더 용도로 사용해도 된다.


#### \<nav>
내비게이션의 약자로, 일반적으로 상단바 등 사이트를 안내하는 요소에 사용된다. 보통은 안에 \<ul>을 넣어 목록 형태로 사용한다.

#### \<main>
문서의 주된 콘텐츠를 표시한다. 이 태그는 두 개 이상 보여져서는 안된다. 두 개 이상의 main요소를 쓸 경우 하나 이외의 전부를 hidden 속성을 써서 가려야 한다.

#### \<article>
웹 페이지의 내용에 사용하는 태그이다. 문서나 페이지, 사이트에서 독립적으로 배포 혹은 재사용(투고 같은) 할 수 있는 섹션에 사용한다.

#### \<section>
웹 페이지의 섹션에 사용하는 태그이다. 웹 페이지를 의미적으로 각각의 파트로 구분하기 위해 쓰는 태그이다. 이 태그를 사용하면 검색엔진이 긁어가지 않는다는 이야기가 있는데 루머다. HTML5 표준 문서에 보면 "요소의 내용을 배포(syndicate)해도 이치에 맞다면 section 요소 대신 article 요소를 사용하기를 권합니다."라는 부분이 있는데, 이 부분의 해석이 잘못 퍼진 것으로 추정된다.

#### \<aside>
본문의 주요 부분을 표시하고 남은 부분을 설명하는 태그이다. 특별한 일이 아니면 사이드바나 광고창 등 중요하지 않은 부분에 사용된다.

#### \<footer>
일반적으로 페이지나 해당 파트의 가장 아랫부분에 위치한다. 페이지 맨 아래에 쓸 때는 사이트의 라이선스, 주소, 연락처 등을 넣는다.

### 멀티미디어 태그

#### \<audio>
음성, 음악 파일 등을 재생할 수 있는 태그. 웹 브라우저마다 지원하는 확장자가 달라 멀티브라우저 지원을 위해서는 \<source> 태그를 안에 넣어 두가지 이상의 확장자를 가진 음악 파일을 넣어야 한다. 가장 많이 사용하는 조합은 mp3+ogg

#### \<video>
영상 파일을 재생할 수 있는 태그. 사실상 HTML5에서 가장 주목받는 태그이다. 별다른 플러그인 없이도 자체 재생이 가능하다는 점이 가장 큰 장점이다. \<audio> 태그와 마찬가지로 \<source> 태그를 넣어 mp4+ogv의 조합으로 짜주면 거의 대부분의 브라우저를 지원한다.

#### \<canvas>
스크립트를 이용하여 그래픽을 표현하는 태그이다. 일반적으로는 JavaScript를 많이 사용하며, 응용하면 웹에서 게임 앱, 3D 엔진 등을 돌리는 다양한 응용이 가능하다.

### 폼 관련

#### \<output>
계산의 결과값을 전송하는 데에 쓰인다.

#### 새로운 \<input> 의 type 속성 - date, datetime, time, color, range...
자바스크립트를 통해서만 구현됐던 기능이 내장되었다. 현 시점에서는 크롬이 사실상 전부를 지원한다.

#### \<datalist>
\<input>의 type="text"와 같은 속성을 가진 것들에 들어갈 값을 미리 정의하는 태그이다.

### 기타
#### \<menu>
툴바, 팝업 메뉴를 넣을 때 쓴다. 현재는 FireFox에서만 적용된다.

#### \<menuitem>
툴바, 팝업 메뉴의 각 항목을 정의한다.

#### \<details>
보이거나 숨기게 해주는 요약글 형식의 위젯에 사용되는 태그이다. \<summary>태그와 함께 쓰인다.

#### \<embad>
외부 애플리케이션이나 플러그인을 삽입할 때 쓰는 태그이다. 대표적으로 어도비 플래시를 웹페이지에 삽입할 때 이걸 쓴다.

#### \<object>
외부 문서, 매체, 플러그인 등을 웹페이지에 삽입할 때 쓰는 태그이다.

#### \<figure>
그림, 도표, 다이어그램 등의 글의 이해를 돕기 위한 내용들을 나타내는 태그이다.

#### \<figurecaption>
\<figure> 태그 안에 사용되는 태그로, \<figure> 태그 안에 있는 내용의 설명을 적는 태그이다.

#### \<iframe>
외부 문서를 해당 영역에 삽입하는 태그이다.

#### \<time>
기계가 이해하기 쉽게 시간을 표현한다. CSS를 정하지 않았다면 외관상의 변화는 없다.
\<time datetime="2001-05-15 19:00">n시간 전\</time> 같이 datetime에 그레고리력 시간을 넣어 태그를 작성해야 기계가 이해하기 쉬워진다.

#### \<mark>
특정한 부분을 형광펜으로 마킹한다.

### 용도가 바뀐 태그

#### \<s>
더이상 옳지 않은 내용을 나타내는 데에 쓴다. 별도의 CSS 없이 쓰면 브라우저에서는 취소선을 긋는 것이 기본값이다.

#### \<u>
양식상 일반적인 텍스트보다 돋보여야 할때 쓴다. 예를 들어 철자가 틀린 단어나, 중국어로 번역된 고유 명사 등이 있다. 별도의 CSS 없이 쓰면 브라우저에서는 밑줄을 긋는 것이 기본값이다.

#### \<i>
어떠한 이유로 일반적인 텍스트보다 돋보여야 할때 쓴다. 예를 들어 전문 용어, 외국어의 구절 등이 있다. 별도의 CSS 없이 쓰면 브라우저에서는 이탤릭체로 표기하는 것이 기본값이다.
더 적절한 시맨틱 태그가 있을 경우 그쪽을 쓴다.

#### \<hr>
원래 단순한 가로줄을 나타내는 태그였으나, 페이지의 주제가 바뀔 때 내용을 분리시키는 의미가 HTML5에서 추가되었다.

#### \<wbr>
원래 <nobr> 태그 안에서 <br> 태그를 대신하여 강제개행 기능을 하는 태그였으나, HTML5 표준으로 편입되면서 띄어쓰기 없이 이 태그를 사용한 부분에서 자동개행을 하는 기능으로 변경되었다. (<nobr> 태그는 CSS로 대체 가능하여 폐기되었다.)

----------------------------------------------------------------------------

## Sematic Web
컴퓨터가 사람을 대신하여 정보를 읽고, 이해하고 가공하여 새로운 정보를 만들어 낼 수 있도록 이해하기 쉬운 의미를 가진 차세대 지능형 웹. 1998년 월드 와이드 웹의 창시자인 팀 버너스 리(Tim Berners Lee)에 의해 개발, 기계가 읽고 처리할 수 있는 웹이라고 정의하였다. 컴퓨터가 정보를 제공하기 위해 자체적으로 웹상의 정보를 탐색 및 수집하여 논리적으로 추론하는 정보처리 기능을 하고 있다. 인터넷 정보를 의미망으로 통합한 온톨로지(ontology) 형태로 이루어지며, 정보를 이해하고 다양한 정보 간 의미요소를 연결함으로서 지능적 판단에 따라 추출, 가공하는 처리방식을 말한다. 이를 위해 컴퓨터가 인식할 수 있는 언어를 이용해 웹페이지의 정보를 나타내는 방식이 적용되었는데, 시맨틱 마크업 언어로는 XML,RDF등의 언어기술이 표준화되어 있다.