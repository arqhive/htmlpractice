## Form Method

form 속성에 method로 'get' 혹은 'post'를 사용 할 수 있다.

### GET
form을 submit 할 때 기본 방법은 GET 이다.

GET을 사용하면 폼 데이터가 페이지 주소 필드에 표시된다.

*** 주의 사항 ***
1. 양식 데이터를 이름 / 값 쌍으로 URL에 추가한다.
2. URL의 길이는 3000자 제한이 있다.
3. 중요한 데이터는 GET을 사용하지 말자
4. 사용자가 결과를 북마크하려는 양식 제출에 유용하다.
5. 검색어 문자열과 같은 보안되지 않은 데이터에 좋다.

### POST
post는 submit 된 데이터를 페이지 주소 필드에 표시하지 않는다.

*** 참고 사항 ***
1. POST에는 크기 제한이 없으므로 많은 양의 데이터를 보낼 수 있다.
2. 북마크 불가능

### form attributes
1. accept-charset : 전송될 폼에 특정 charset을 지정 할 수 있다.
2. action : 전송된 폼을 처리할 주소 (생략시 현재 페이지)
3. autocomplete : 자동완성기능 (default: on)
4. enctype : 전송할 데이터의 인코딩 타입을 지정한다 (default: is url-encoded)
5. method : 전송될 폼에 HTTP method 지정 (default: GET)
6. name : 폼을 정의하는 이름
7. novalidate : 브라우저가 폼을 검증하지 않도록 한다.
8. target : action 결과를 표시할 타겟 (default: _self)

### 사용법
각 입력 필드에는 submit 될 때 name 속성이 있어야 한다.

name 속성이 생략된 경우 데이터가 전송되지 않는다.
