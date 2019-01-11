## event

### 1. window events (body 태그에 적용)

#### onafterprint, onbeforeprint
페이지가 인쇄 되기 전, 인쇄 된 후 할 이벤트

#### onbeforeunload
문서를 언로드(이탈 할 때) 페이지를 나가시겠습니까? 와 같은 이벤트 삽입 가능

#### onerror
외부 파일이 정상적으로 로드 되지 않을때

#### onhashchange
북마크 앵커에 대한 링크를 클릭 할때

#### onload
문서 로드가 완료 되었을 때, 브라우저 버전 확인, 쿠키 처리 등등.. 캐시에서 로드 될때 발생 안함

#### onpageshow
페이지가 로드 될때마다 실행하는 이벤트

#### onresize
창 사이즈를 조절 할 때 발생하는 이벤트

#### onunload
페이지가 언로드 되거나 브라우저 창을 닫으면 실행된다.
페이지를 다시 로드 하면 onunload 및 onload도 트리거 된다.


### 2. form events

#### onblur
요소가 포커스를 읽는 순간 실행 된다.

#### oncontextmenu
컨텍스트 메뉴를 열기 위해 요소를 마우스 오른쪽 버튼으로 클릭 할 때
(oncontextmenu는 모든 브라우저가 지원하지만 contextmenu는 파이어폭스만 지원)

#### onfocus
요소가 포커스를 얻을 때

#### oninput, onchange
input 또는 textarea 요소의 값이 변경 될 때, onchange는 요소가 포커스를 잃을 때 발생하지만 oninput는 값이 변경 직후 발생됨, onchange는 select에도 사용된다.

#### oninvalid
제출할 input 요소가 유효하지 않은 경우 (safari 미지원)

#### onreset (form에 지정)
reset이 발생한 경우 발생하는 이벤트

#### onsearch
input type="search" 요소에서 엔터키를 누르거나 x버튼을 누를 때 발생 (엣지, 파이어폭스 미지원)

#### onselect
텍스트를 선택하면 실행된다. (텍스트를 블록 처리 한 경우)

#### onsubmit
폼 제출 할 때 실행

### 3. Keyboard events
해당 요소에서 실행 하는 이벤트임

#### onkeydown
사용자가 키를 누를 때

#### onkeypress
사용자가 키를 누를 때, 모든 키에 대해 동작하지 않으므로 onkeydown을 대신 사용한다.

#### onkeyup
사용자가 키보드에서 키를 놓을 때

### 4. Mouse events

#### onclick
클릭 했을 때

#### ondblclick
더블 클릭 했을 때

#### onmousedown, onmouseup, onclick (마우스 좌 클릭)

#### onmousedown, onmouseup, oncontextmenu (마우스 우 클릭)

#### onmousemove
마우스 포인터가 해당 요소 위에 있을 때

#### onmouseout, onmouseover
마우스 포인터가 해당 요소 위에 있을 때, 그리고 없을 때

#### onwheel
마우스의 휠 혹은 터치 패드로 요소를 스크롤하거나 확대 할때 발생 (사파리 미지원)

### 5. drag drop events
추후 알아본다.

### 6. Clipboard events

#### oncopy
사용자가 요소의 내용을 복사할 때 발생하는 이벤트.
이미지 복사할 때도 발생

#### oncut
사용자가 요소의 내용을 자를때 발생하는 이벤트.
contenteditable 속성을 true 설정 하지 않은 이상 잘라낼 수 없다.

#### onpaste
사용자가 요소에 내용을 붙여넣을때 발생하는 이벤트.
주로 input type="text" 에서 사용 됨
contenteditable 속성을 true 설정 하지 않은 이상 붙여 넣을 수 없다.
