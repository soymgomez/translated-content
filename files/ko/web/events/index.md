---
title: 이벤트 참조
slug: Web/Events
tags:
  - Event
  - Overview
  - Reference
translation_of: Web/Events
---
<p>DOM 이벤트는 발생한 흥미로운 것을 코드에 알리기 위해 전달됩니다. 각 이벤트는 {{DOMxRef("Event")}} 인터페이스를 기반으로한 객체에 의해 표현되며 발생한 것에 대한 부가적인 정보를 얻는데 사용되는 추가적인 커스텀 필드 또는 함수를 가질수도 있습니다. 이벤트는 렌더링 모델에서 기본적인 사용자 인터렉션부터 발생한 것에대한 자동 알림까지 모든 것을 나타낼 수 있습니다.</p>

<p>이 글은 전달될 수 있는 이벤트의 목록을 제공합니다. 일부는 공식 명세에 정의된 표준 이벤트이며, 다른 일부는 특정 브라우저에서 내부적으로 사용되는 이벤트입니다. 예로, Mozilla 특정 이벤트는 <a href="https://developer.mozilla.org/ko/docs/Mozilla/%EC%95%A0%EB%93%9C%EC%98%A8%EB%93%A4">부가 기능</a>이 브라우저와 상호작용하기 위해 나열되었습니다.</p>

<h2 id="가장_일반적인_카테고리">가장 일반적인 카테고리</h2>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="리소스_이벤트">리소스 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("cached")}}</td>
   <td>매니페스트에 나열된 리소스가 다운로드되었고, 애플리케이션이 캐시될 때.</td>
  </tr>
  <tr>
   <td>{{Event("error")}}</td>
   <td>리소스 로드가 실패했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("abort")}}</td>
   <td>리소스 로딩이 중단되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("load")}}</td>
   <td>리소스와 그 의존 리소스의 로딩이 끝났을 때.</td>
  </tr>
  <tr>
   <td>{{Event("beforeunload")}}</td>
   <td>window, document 및 그 리소스가 언로드되려고 할 때.</td>
  </tr>
  <tr>
   <td>{{Event("unload")}}</td>
   <td>document 또는 의존 리소스가 언로드될 때.</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="네트워크_이벤트">네트워크 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("online")}}</td>
   <td>브라우저가 네트워크 접근을 얻었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("offline")}}</td>
   <td>브라우저가 네트워크 접근을 잃었을 때.</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="포커스_이벤트">포커스 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("focus")}}</td>
   <td>엘리먼트가 포커스를 받았을 때(버블링하지 않음).</td>
  </tr>
  <tr>
   <td>{{Event("blur")}}</td>
   <td>엘리먼트가 포커스를 잃었을 때(버블링하지 않음).</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="웹소켓_이벤트">웹소켓 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/open_websocket">open</a></code></td>
   <td>웹소켓 연결이 수립되었을 때.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/message_websocket">message</a></code></td>
   <td>웹소켓을 통해 메시지를 받았을 때.</td>
  </tr>
  <tr>
   <td>{{Event("error")}}</td>
   <td>웹소켓 연결이 어떤 문제로 닫혔을 때(예로, 일부 데이터가 전송되지 못했을 때).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/close_websocket">close</a></code></td>
   <td>웹소켓 연결이 닫혔을 때.</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="세션_기록_이벤트">세션 기록 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("pagehide")}}</td>
   <td>세션 기록 항목이 사라지고 있을 때.</td>
  </tr>
  <tr>
   <td>{{Event("pageshow")}}</td>
   <td>세션 기록 항목이 들어오고 있을 때.</td>
  </tr>
  <tr>
   <td>{{Event("popstate")}}</td>
   <td>세션 기록 항목이 이동하고 있을 때(특정 경우에서).</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="CSS_애니메이션_이벤트">CSS 애니메이션 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("animationstart")}}</td>
   <td><a href="https://developer.mozilla.org/en-US/docs/CSS/CSS_animations">CSS 애니메이션</a>이 시작되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("animationend")}}</td>
   <td><a href="https://developer.mozilla.org/en-US/docs/CSS/CSS_animations">CSS 애니메이션</a>이 완료되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("animationiteration")}}</td>
   <td><a href="https://developer.mozilla.org/en-US/docs/CSS/CSS_animations">CSS 애니메이션</a>이 반복되었을 때.</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="CSS_전이_이벤트">CSS 전이 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("transitionstart")}}</td>
   <td><a href="/en-US/docs/Web/CSS/CSS_Transitions">CSS 전이</a>가 실제로 시작되었을 때(딜레이 후에 실행되었을 때).</td>
  </tr>
  <tr>
   <td>{{Event("transitioncancel")}}</td>
   <td><a href="/en-US/docs/Web/CSS/CSS_Transitions">CSS 전이</a>가 취소되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("transitionend")}}</td>
   <td><a href="/en-US/docs/Web/CSS/CSS_Transitions">CSS 전이</a>가 완료되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("transitionrun")}}</td>
   <td><a href="/en-US/docs/Web/CSS/CSS_Transitions">CSS 전이</a>가 실행을 시작했을 때(딜레이 시작전에 실행되었을 때).</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="폼_이벤트">폼 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">Event Name</th>
   <th scope="col">Fired When</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("reset")}}</td>
   <td>리셋 버튼이 눌렸을 때</td>
  </tr>
  <tr>
   <td>{{Event("submit")}}</td>
   <td>제출 버튼이 눌렸을 때</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="Printing_Events">Printing Events</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("beforeprint")}}</td>
   <td>프린트 대화상자가 열렸을 때</td>
  </tr>
  <tr>
   <td>{{Event("afterprint")}}</td>
   <td>프린트 대화상자가 닫혔을 때</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="텍스트_작성_이벤트">텍스트 작성 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("compositionstart")}}</td>
   <td>텍스트 입력 통로가 준비되었을 때(키보드 입력을 위한 키 다운과 유사하지만, 음성 인식과 같은 다른 입력과도 동작합니다).</td>
  </tr>
  <tr>
   <td>{{Event("compositionupdate")}}</td>
   <td>작성될 텍스트 통로에 문자가 추가되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("compositionend")}}</td>
   <td>텍스트 입력 통로가 완료되었거나 취소되었을 때.</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="뷰_이벤트">뷰 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("fullscreenchange")}}</td>
   <td>엘리먼트가 전체화면 모드로 변경되었거나 일반 모드로 돌아왔을 때.</td>
  </tr>
  <tr>
   <td>{{Event("fullscreenerror")}}</td>
   <td>기술적인 이유나 권한 거절을 이유로 전체화면 모드 전환이 불가능했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("resize")}}</td>
   <td>다큐먼트 뷰가 리사이즈되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("scroll")}}</td>
   <td>다큐먼트 뷰나 엘리먼트가 스크롤되었을 때.</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="클립보드_이벤트">클립보드 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("cut")}}</td>
   <td>선택이 잘라내어진 후 클립보드로 복사되었을 때</td>
  </tr>
  <tr>
   <td>{{Event("copy")}}</td>
   <td>선택이 클립보드로 복사되었을 때</td>
  </tr>
  <tr>
   <td>{{Event("paste")}}</td>
   <td>클립보드의 항목이 붙여너어졌을 때</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="키보드_이벤트">키보드 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("keydown")}}</td>
   <td>키가 눌렸을 때</td>
  </tr>
  <tr>
   <td>{{Event("keypress")}}</td>
   <td>쉬프트, Fn, CapsLock 을 제외한 키가 눌린 상태일 때(연속적으로 실행됨.).</td>
  </tr>
  <tr>
   <td>{{Event("keyup")}}</td>
   <td>키 누름이 해제될 때</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="마우스_이벤트">마우스 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("mouseenter")}}</td>
   <td>포인팅 장치가 리스너가 등록된 엘리먼트 위로 이동했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("mouseover")}}</td>
   <td>포인팅 장치가 리스너가 등록된 엘리먼트나 그 자식 엘리먼트의 위로 이동했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("mousemove")}}</td>
   <td>포인팅 장치가 엘리먼트 위에서 이동했을 때(마우스가 이동하는동안 계속 실행됨.)</td>
  </tr>
  <tr>
   <td>{{Event("mousedown")}}</td>
   <td>포인팅 장치 버튼이 엘리먼트 위에서 눌렸을 때.</td>
  </tr>
  <tr>
   <td>{{Event("mouseup")}}</td>
   <td>포인팅 장치 버튼이 엘리먼트 위에서 놓였을 때.</td>
  </tr>
  <tr>
   <td>{{Event("auxclick")}}</td>
   <td>포인팅 장치 버튼(주가 아닌 버튼)이 엘리먼트에서 눌렸다가 놓였을 때.</td>
  </tr>
  <tr>
   <td>{{Event("click")}}</td>
   <td>포인팅 장치 버튼(모든 버튼; 주 버튼만 해당될 예정)이 엘리먼트에서 눌렸다가 놓였을 때.</td>
  </tr>
  <tr>
   <td>{{Event("dblclick")}}</td>
   <td>포인팅 장치 버튼이 엘리먼트에서 두 번 클릭되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("contextmenu")}}</td>
   <td>마우스의 오른쪽 버튼이 클릭되었을 때(컨텍스트 메뉴가 표시되기 전).</td>
  </tr>
  <tr>
   <td>{{Event("wheel")}}</td>
   <td>포인팅 장치의 휠 버튼이 어떤 방향이든 회전되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("mouseleave")}}</td>
   <td>포인팅 장치가 리스너가 등록된 엘리먼트 밖으로 이동했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("mouseout")}}</td>
   <td>포인팅 장치가 리스너가 등록된 엘리먼트 또는 그 자식 엘리먼트의 밖으로 이동했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("select")}}</td>
   <td>어떤 텍스트가 선택되고 있을 때.</td>
  </tr>
  <tr>
   <td>{{Event("pointerlockchange")}}</td>
   <td>포인터가 잠겼거나 해제되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("pointerlockerror")}}</td>
   <td>기술적인 이유나 권한 거절을 이유로 포인터 잠금이 불가했을 때.</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="드래그_앤_드랍_이벤트">드래그 앤 드랍 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("dragstart")}}</td>
   <td>사용자가 엘리먼트나 텍스트 선택을 드래그하기 시작할 때.</td>
  </tr>
  <tr>
   <td>{{Event("drag")}}</td>
   <td>엘리먼트나 텍스트 선택이 드래그되고 있을 때(350ms 마다 연속적으로 실행됨).</td>
  </tr>
  <tr>
   <td>{{Event("dragend")}}</td>
   <td>드래그 작업이 끝났을 때(마우스 버튼을 놓거나 escape 키를 눌러서).</td>
  </tr>
  <tr>
   <td>{{Event("dragenter")}}</td>
   <td>드래그된 엘리먼트나 텍스트 선택이 유효한 드랍 대상에 들어왔을 때.</td>
  </tr>
  <tr>
   <td>{{Event("dragover")}}</td>
   <td>엘리먼트나 텍스트 선택이 유효한 드랍 대상위로 드래그되었을 때(350ms 마다 연속적으로 실행됨.).</td>
  </tr>
  <tr>
   <td>{{Event("dragleave")}}</td>
   <td>드래그된 엘리먼트나 텍스트 선택이 유효한 드랍 대상에서 나갈 때.</td>
  </tr>
  <tr>
   <td>{{Event("drop")}}</td>
   <td>엘리먼트가 유효한 드랍 대상에 드랍되었을 때.</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="미디어_이벤트">미디어 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("durationchange")}}</td>
   <td><code>duration</code> 속성이 업데이트되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("loadedmetadata")}}</td>
   <td>메타데이터가 로드되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("loadeddata")}}</td>
   <td>미디어의 첫 번째 프레임이 로딩을 마쳤을 때.</td>
  </tr>
  <tr>
   <td>{{Event("canplay")}}</td>
   <td>브라우저가 미디어를 실행할 수 있지만, 컨텐츠의 버퍼링없이 중단되지 않고 미디어를 끝까지 재생하기엔 로딩된 데이터가 충분하지않다고 측정했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("canplaythrough")}}</td>
   <td>브라우저가 컨텐츠 버퍼링 중단 없이 미디어를 끝까지 재생할 수 있다고 측정했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("ended")}}</td>
   <td>미디어의 끝에 도달해 재생이 멈추었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("emptied")}}</td>
   <td>미디어가 비었을 때. 예로, 이 이벤트는 미디어가 이미 로딩되었고(또는 부분적으로 로딩되었고), <a href="/en-US/docs/XPCOM_Interface_Reference/NsIDOMHTMLMediaElement" rel="internal"><code>load()</code></a> 메소드가 리로드를 위해 호출되었을때 전송됩니다.</td>
  </tr>
  <tr>
   <td>{{Event("stalled")}}</td>
   <td>유저 애이전트가 미디어 데이터 페치를 시도했지만, 데이터가 예상치 못하게 전송되지 않을 때.</td>
  </tr>
  <tr>
   <td>{{Event("suspend")}}</td>
   <td>미디어 데이터 로딩이 유예되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("play")}}</td>
   <td>재생이 시작되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("playing")}}</td>
   <td>일시정지나 데이터 부족으로 딜레이된 후로부터 재생할 준비가 되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("pause")}}</td>
   <td>재생이 일시정지 되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("waiting")}}</td>
   <td>일시적인 데이터 부족으로 재생이 중지되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("seeking")}}</td>
   <td>찾기 작업이 시작되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("seeked")}}</td>
   <td>찾기 작업이 완료되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("ratechange")}}</td>
   <td>재생률이 변경되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("timeupdate")}}</td>
   <td><code>currentTime</code> 속성으로 나타나는 시간이 업데이트되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("volumechange")}}</td>
   <td>볼륨이 변경되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("complete")}}</td>
   <td>{{DOMxRef("OfflineAudioContext")}} 의 렌더링이 종료되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("audioprocess")}}</td>
   <td>{{DOMxRef("ScriptProcessorNode")}} 의 입력 버퍼의 처리가 준비되었을 때.</td>
  </tr>
 </tbody>
</table>
</div>

<div style="overflow: auto;">
<table class="standard-table">
 <caption>
 <h3 id="진행_이벤트">진행 이벤트</h3>
 </caption>
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("loadstart")}}</td>
   <td>진행이 시작되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("progress")}}</td>
   <td>진행중일 때.</td>
  </tr>
  <tr>
   <td>{{Event("error")}}</td>
   <td>진행이 실패했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("timeout")}}</td>
   <td>프리셋 타임 만료로 진행이 종료되었을 때.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/abort_(ProgressEvent)">abort</a></code></td>
   <td>진행이 종료되었을 때(에러가 아닌 이유).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/load_(ProgressEvent)">load</a></code></td>
   <td>진행이 성공했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("loadend")}}</td>
   <td>진행이 멈추었을 때("error", "abort" 또는 "load" 가 디스패치된 후).</td>
  </tr>
 </tbody>
</table>
</div>

<h3 id="저장소_이벤트">저장소 이벤트</h3>

<p>{{Event("change")}} (<a href="#non-standard_events">Non-standard events</a> 를 보세요)<br>
 {{Event("storage")}}</p>

<h3 id="업데이트_이벤트">업데이트 이벤트</h3>

<p>{{Event("checking")}}<br>
 {{Event("downloading")}}<br>
 {{Event("error")}}<br>
 {{Event("noupdate")}}<br>
 {{Event("obsolete")}}<br>
 {{Event("updateready")}}</p>

<h3 id="값_변경_이벤트">값 변경 이벤트</h3>

<p>{{Event("broadcast")}}<br>
 {{Event("CheckboxStateChange")}}<br>
 {{Event("hashchange")}}<br>
 {{Event("input")}}<br>
 {{Event("RadioStateChange")}}<br>
 {{Event("readystatechange")}}<br>
 {{Event("ValueChange")}}</p>

<h3 id="분류되지_않은_이벤트">분류되지 않은 이벤트</h3>

<p>{{Event("invalid")}}<br>
 {{Event("localized")}}<br>
 <code><a href="/en-US/docs/Web/Reference/Events/message_webworker">message</a></code><br>
 <code><a href="/en-US/docs/Web/Reference/Events/message_webmessaging">message</a></code><br>
 <code><a href="/en-US/docs/Web/Reference/Events/message_serversentevents">message</a></code><br>
 <code><a href="/en-US/docs/Web/Reference/Events/open_serversentevents">open</a></code><br>
 {{Event("show")}}</p>

<h2 id="덜_일반적이고_비표준인_이벤트">덜 일반적이고 비표준인 이벤트</h2>

<h3 id="Abortable_페치_이벤트">Abortable 페치 이벤트</h3>

<div style="overflow: auto;">
<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("abort_(dom_abort_api)", "abort")}}</td>
   <td>DOM 요청이 중단되었을 때. 예, {{DOMxRef("AbortController.abort()")}} 사용.</td>
  </tr>
 </tbody>
</table>
</div>

<h3 id="WebVR_이벤트">WebVR 이벤트</h3>

<div style="overflow: auto;">
<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("vrdisplayconnect")}}</td>
   <td>호환되는 {{DOMxRef("VRDisplay")}} 가 컴퓨터에 연결되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("vrdisplaydisconnect")}}</td>
   <td>호환되는 {{DOMxRef("VRDisplay")}} 가 컴퓨터로부터 연결해제되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("vrdisplayactivate")}}</td>
   <td>VR 디스플레이가 표시될 수 있을 때. 예, HMD 가 움직여 대기모드에서 나오거나, 착용에의해 준비될 때.</td>
  </tr>
  <tr>
   <td>{{Event("vrdisplaydeactivate")}}</td>
   <td>{{DOMxRef("VRDisplay")}} 가 더 이상 표시될 수 없을 때. 예, 비활성 기간으로 인해 HMD 가 대기 또는 슬립모드로 빠졌을 때.</td>
  </tr>
  <tr>
   <td>{{Event("vrdisplayblur")}}</td>
   <td>브라우저, OS 또는 VR 장치로부터 어떤 이유에 의해 {{DOMxRef("VRDisplay")}} 로의 프리젠테이션이 중단되었을 때. 예, 사용자가 시스템 메뉴나 브라우저와 인터렉팅하는동안 추적이나 경험 손실을 방지.</td>
  </tr>
  <tr>
   <td>{{Event("vrdisplayfocus")}}</td>
   <td>흐릿해진 이후에 {{DOMxRef("VRDisplay")}} 로의 프리젠테이션이 재개될 때.</td>
  </tr>
  <tr>
   <td>{{Event("vrdisplaypresentchange")}}</td>
   <td>{{DOMxRef("VRDisplay")}} 의 프리젠팅 상태가 변경할 때. 예, 프리젠팅에서 프리젠팅이 아닌 것이 될 때, 또는 그 반대.</td>
  </tr>
 </tbody>
</table>
</div>

<h3 id="SVG_이벤트">SVG 이벤트</h3>

<p>{{Event("SVGAbort")}}<br>
 {{Event("SVGError")}}<br>
 {{Event("SVGLoad")}}<br>
 {{Event("SVGResize")}}<br>
 {{Event("SVGScroll")}}<br>
 {{Event("SVGUnload")}}<br>
 {{Event("SVGZoom")}}</p>

<h3 id="데이터베이스_이벤트">데이터베이스 이벤트</h3>

<p><code><a href="/en-US/docs/Web/Reference/Events/abort_indexedDB">abort</a></code><br>
 <code><a href="/en-US/docs/Web/Reference/Events/blocked_indexedDB">blocked</a></code><br>
 <code><a href="/en-US/docs/Web/Reference/Events/complete_indexedDB">complete</a></code><br>
 {{Event("error")}} (<a href="/en-US/docs/Web/Reference/Events/error">link</a>)<br>
 <code><a href="/en-US/docs/Web/Reference/Events/success_indexedDB">success</a></code><br>
 <code><a href="/en-US/docs/Web/Reference/Events/upgradeneeded_indexedDB">upgradeneeded</a></code><br>
 <code><a href="/en-US/docs/Web/Reference/Events/versionchange_indexedDB">versionchange</a></code></p>

<h3 id="알림_이벤트">알림 이벤트</h3>

<p><a href="/en-US/docs/Web/Reference/Events/AlertActive">AlertActive</a><br>
 <a href="/en-US/docs/Web/Reference/Events/AlertClose">AlertClose</a></p>

<h3 id="CSS_이벤트">CSS 이벤트</h3>

<p><a href="/en-US/docs/Web/Reference/Events/CssRuleViewRefreshed">CssRuleViewRefreshed</a><br>
 <a href="/en-US/docs/Web/Reference/Events/CssRuleViewChanged">CssRuleViewChanged</a><br>
 <a href="/en-US/docs/Web/Reference/Events/CssRuleViewCSSLinkClicked">CssRuleViewCSSLinkClicked</a></p>

<h3 id="Script_이벤트">Script 이벤트</h3>

<p>{{Event("afterscriptexecute")}}<br>
 {{Event("beforescriptexecute")}}</p>

<h3 id="메뉴_이벤트">메뉴 이벤트</h3>

<p>{{Event("DOMMenuItemActive")}}<br>
 {{Event("DOMMenuItemInactive")}}</p>

<h3 id="Window_이벤트">Window 이벤트</h3>

<p><a href="/en-US/docs/Web/Reference/Events/DOMWindowCreated">DOMWindowCreated</a><br>
 <a href="/en-US/docs/Web/Reference/Events/DOMTitleChanged">DOMTitleChanged</a><br>
 <a href="/en-US/docs/Web/Reference/Events/DOMWindowClose">DOMWindowClose</a><br>
 <a href="/en-US/docs/Web/Reference/Events/SSWindowClosing">SSWindowClosing</a><br>
 <a href="/en-US/docs/Web/Reference/Events/SSWindowStateReady">SSWindowStateReady</a><br>
 <a href="/en-US/docs/Web/Reference/Events/SSWindowStateBusy">SSWindowStateBusy</a><br>
 <a href="/en-US/docs/Web/Reference/Events/close_event">close</a></p>

<h3 id="Document_이벤트">Document 이벤트</h3>

<p><a href="/en-US/docs/Web/Reference/Events/DOMLinkAdded">DOMLinkAdded</a><br>
 <a href="/en-US/docs/Web/Reference/Events/DOMLinkRemoved">DOMLinkRemoved</a><br>
 <a href="/en-US/docs/Web/Reference/Events/DOMMetaAdded">DOMMetaAdded</a><br>
 <a href="/en-US/docs/Web/Reference/Events/DOMMetaRemoved">DOMMetaRemoved</a><br>
 <a href="/en-US/docs/Web/Reference/Events/DOMWillOpenModalDialog">DOMWillOpenModalDialog</a><br>
 <a href="/en-US/docs/Web/Reference/Events/DOMModalDialogClosed">DOMModalDialogClosed</a></p>

<h3 id="팝업_이벤트">팝업 이벤트</h3>

<p>{{Event("popuphidden")}}<br>
 {{Event("popuphiding")}}<br>
 {{Event("popupshowing")}}<br>
 {{Event("popupshown")}}<br>
 <a href="/en-US/docs/Web/Reference/Events/DOMPopupBlocked">DOMPopupBlocked</a></p>

<h3 id="탭_이벤트">탭 이벤트</h3>

<p><a href="/en-US/docs/Web/Reference/Events/TabOpen">TabOpen</a><br>
 <a href="/en-US/docs/Web/Reference/Events/TabClose">TabClose</a><br>
 <a href="/en-US/docs/Web/Reference/Events/TabSelect">TabSelect</a><br>
 <a href="/en-US/docs/Web/Reference/Events/TabShow">TabShow</a><br>
 <a href="/en-US/docs/Web/Reference/Events/TabHide">TabHide</a><br>
 <a href="/en-US/docs/Web/Reference/Events/TabPinned">TabPinned</a><br>
 <a href="/en-US/docs/Web/Reference/Events/TabUnpinned">TabUnpinned</a><br>
 <a href="/en-US/docs/Web/Reference/Events/SSTabClosing">SSTabClosing</a><br>
 <a href="/en-US/docs/Web/Reference/Events/SSTabRestoring">SSTabRestoring</a><br>
 <a href="/en-US/docs/Web/Reference/Events/SSTabRestored">SSTabRestored</a><br>
 {{Event("visibilitychange")}}</p>

<h3 id="배터리_이벤트">배터리 이벤트</h3>

<p>{{Event("chargingchange")}}<br>
 {{Event("chargingtimechange")}}<br>
 {{Event("dischargingtimechange")}}<br>
 {{Event("levelchange")}}</p>

<h3 id="호출_이벤트">호출 이벤트</h3>

<p>{{Event("alerting")}}<br>
 {{Event("busy")}}<br>
 {{Event("callschanged")}}<br>
 {{Event("cfstatechange")}}<br>
 {{Event("connected")}}<br>
 {{Event("connecting")}}<br>
 {{Event("dialing")}}<br>
 {{Event("disconnected")}}<br>
 {{Event("disconnecting")}}<br>
 {{Event("error_(Telephony)","error")}}<br>
 {{Event("held")}}, {{Event("holding")}}<br>
 {{Event("incoming")}}<br>
 {{Event("resuming")}}<br>
 {{Event("statechange")}}<br>
 {{Event("voicechange")}}</p>

<h3 id="센서_이벤트">센서 이벤트</h3>

<p>{{Event("compassneedscalibration")}}<br>
 {{Event("devicelight")}}<br>
 {{Event("devicemotion")}}<br>
 {{Event("deviceorientation")}}<br>
 {{Event("deviceproximity")}}<br>
 {{Event("MozOrientation")}}<br>
 {{Event("orientationchange")}}<br>
 {{Event("userproximity")}}</p>

<h3 id="스마트카드_이벤트">스마트카드 이벤트</h3>

<p>{{Event("icccardlockerror")}}<br>
 {{Event("iccinfochange")}}<br>
 {{Event("smartcard-insert")}}<br>
 {{Event("smartcard-remove")}}<br>
 {{Event("stkcommand")}}<br>
 {{Event("stksessionend")}}<br>
 {{Event("cardstatechange")}}</p>

<h3 id="SMS_및_USSD_이벤트">SMS 및 USSD 이벤트</h3>

<p>{{Event("delivered")}}<br>
 {{Event("received")}}<br>
 {{Event("sent")}}<br>
 {{Event("ussdreceived")}}</p>

<h3 id="프레임_이벤트">프레임 이벤트</h3>

<p>{{Event("mozbrowserclose")}}<br>
 {{Event("mozbrowsercontextmenu")}}<br>
 {{Event("mozbrowsererror")}}<br>
 {{Event("mozbrowsericonchange")}}<br>
 {{Event("mozbrowserlocationchange")}}<br>
 {{Event("mozbrowserloadend")}}<br>
 {{Event("mozbrowserloadstart")}}<br>
 {{Event("mozbrowseropenwindow")}}<br>
 {{Event("mozbrowsersecuritychange")}}<br>
 {{Event("mozbrowsershowmodalprompt")}} (<a href="/en-US/docs/Web/Reference/Events/mozbrowsershowmodalprompt">link</a>)<br>
 {{Event("mozbrowsertitlechange")}}<br>
 <a href="/en-US/docs/Web/Reference/Events/DOMFrameContentLoaded">DOMFrameContentLoaded</a></p>

<h3 id="DOM_뮤테이션_이벤트">DOM 뮤테이션 이벤트</h3>

<p><code><a href="/en-US/docs/DOM/Mutation_events">DOMAttributeNameChanged</a></code><br>
 <code><a href="/en-US/docs/DOM/Mutation_events">DOMAttrModified</a></code><br>
 <code><a href="/en-US/docs/DOM/Mutation_events">DOMCharacterDataModified</a></code><br>
 {{Event("DOMContentLoaded")}}<br>
 <code><a href="/en-US/docs/DOM/Mutation_events">DOMElementNameChanged</a></code><br>
 <code><a href="/en-US/docs/DOM/Mutation_events">DOMNodeInserted</a></code><br>
 <code><a href="/en-US/docs/DOM/Mutation_events">DOMNodeInsertedIntoDocument</a></code><br>
 <code><a href="/en-US/docs/DOM/Mutation_events">DOMNodeRemoved</a></code><br>
 <code><a href="/en-US/docs/DOM/Mutation_events">DOMNodeRemovedFromDocument</a></code><br>
 <code><a href="/en-US/docs/DOM/Mutation_events">DOMSubtreeModified</a></code></p>

<h3 id="터치_이벤트">터치 이벤트</h3>

<p><a href="/en-US/docs/Web/Reference/Events/MozEdgeUIGesture">MozEdgeUIGesture</a><br>
 <a href="/en-US/docs/Web/Reference/Events/MozMagnifyGesture">MozMagnifyGesture</a><br>
 <a href="/en-US/docs/Web/Reference/Events/MozMagnifyGestureStart">MozMagnifyGestureStart</a><br>
 <a href="/en-US/docs/Web/Reference/Events/MozMagnifyGestureUpdate">MozMagnifyGestureUpdate</a><br>
 <a href="/en-US/docs/Web/Reference/Events/MozPressTapGesture">MozPressTapGesture</a><br>
 <a href="/en-US/docs/Web/Reference/Events/MozRotateGesture">MozRotateGesture</a><br>
 <a href="/en-US/docs/Web/Reference/Events/MozRotateGestureStart">MozRotateGestureStart</a><br>
 <a href="/en-US/docs/Web/Reference/Events/MozRotateGestureUpdate">MozRotateGestureUpdate</a><br>
 <a href="/en-US/docs/Web/Reference/Events/MozSwipeGesture">MozSwipeGesture</a><br>
 <a href="/en-US/docs/Web/Reference/Events/MozTapGesture">MozTapGesture</a><br>
 <a href="/en-US/DOM/Touch_events_(Mozilla_experimental)">MozTouchDown</a><br>
 <a href="/en-US/DOM/Touch_events_(Mozilla_experimental)">MozTouchMove</a><br>
 <a href="/en-US/DOM/Touch_events_(Mozilla_experimental)">MozTouchUp</a><br>
 {{Event("touchcancel")}}<br>
 {{Event("touchend")}}<br>
 {{Event("touchenter")}}<br>
 {{Event("touchleave")}}<br>
 {{Event("touchmove")}}<br>
 {{Event("touchstart")}}</p>

<h3 id="포인터_이벤트">포인터 이벤트</h3>

<p>{{Event("pointerover")}}<br>
 {{Event("pointerenter")}}<br>
 {{Event("pointerdown")}}<br>
 {{Event("pointermove")}}<br>
 {{Event("pointerup")}}<br>
 {{Event("pointercancel")}}<br>
 {{Event("pointerout")}}<br>
 {{Event("pointerleave")}}<br>
 {{Event("gotpointercapture")}}<br>
 {{Event("lostpointercapture")}}</p>

<h2 id="표준_이벤트">표준 이벤트</h2>

<p>다음 이벤트들은 공식 웹 명세에 정의되어있으며, 브라우저사이에서 공통입니다. 각 이벤트는 이벤트의 수신자에게 전송되는 객체를 나타내는 인터페이스 및 이벤트를 정의한 명세 또는 명세로의 링크를 나열합니다(따라서 각 이벤트와 제공된 데이터에 대한 정보를 찾을 수 있습니다).</p>

<div style="overflow: auto;">
<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">Event Type</th>
   <th scope="col">Specification</th>
   <th scope="col">Fired when...</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("abort")}}</td>
   <td>{{DOMxRef("UIEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-abort" style="white-space: nowrap;">DOM L3</a></td>
   <td>The loading of a resource has been aborted.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/abort_(ProgressEvent)">abort</a></code></td>
   <td>{{DOMxRef("ProgressEvent")}}</td>
   <td><a href="http://www.w3.org/TR/progress-events/">Progress</a> and <a href="http://www.w3.org/TR/XMLHttpRequest/#event-xhr-abort">XMLHttpRequest</a></td>
   <td>Progression has been terminated (not due to an error).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/abort_indexedDB">abort</a></code></td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/IndexedDB/#database-interface">IndexedDB</a></td>
   <td>A transaction has been aborted.</td>
  </tr>
  <tr>
   <td>{{Event("afterprint")}}{{gecko_minversion_inline("6")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/html5/webappapis.html#printing">HTML5</a></td>
   <td>The associated document has started printing or the print preview has been closed.</td>
  </tr>
  <tr>
   <td>{{Event("animationend")}}</td>
   <td>{{DOMxRef("AnimationEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/css3-animations/#animation-events" style="white-space: nowrap;">CSS Animations</a></td>
   <td>A <a href="/en-US/docs/CSS/CSS_animations">CSS animation</a> has completed.</td>
  </tr>
  <tr>
   <td>{{Event("animationiteration")}}</td>
   <td>{{DOMxRef("AnimationEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/css3-animations/#animation-events" style="white-space: nowrap;">CSS Animations</a></td>
   <td>A <a href="/en-US/docs/CSS/CSS_animations">CSS animation</a> is repeated.</td>
  </tr>
  <tr>
   <td>{{Event("animationstart")}}</td>
   <td>{{DOMxRef("AnimationEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/css3-animations/#animation-events" style="white-space: nowrap;">CSS Animations</a></td>
   <td>A <a href="/en-US/docs/CSS/CSS_animations">CSS animation</a> has started.</td>
  </tr>
  <tr>
   <td>{{Event("appinstalled")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="/en-US/docs/Web/Manifest" style="white-space: nowrap;">Web App Manifest</a></td>
   <td>A web application is successfully installed as a <a href="https://developer.mozilla.org/en-US/Apps/Progressive">progressive web app</a>.</td>
  </tr>
  <tr>
   <td>{{Event("audioprocess")}}</td>
   <td>{{DOMxRef("AudioProcessingEvent")}} {{Deprecated_Inline}}</td>
   <td>{{SpecName('Web Audio API', '#AudioProcessingEvent', 'audioprocess')}}</td>
   <td>The input buffer of a {{DOMxRef("ScriptProcessorNode")}} is ready to be processed.</td>
  </tr>
  <tr>
   <td>{{Event("audioend")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>The user agent has finished capturing audio for speech recognition.</td>
  </tr>
  <tr>
   <td>{{Event("audiostart")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>The user agent has started to capture audio for speech recognition.</td>
  </tr>
  <tr>
   <td>{{Event("beforeprint")}} {{gecko_minversion_inline("6")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/html5/webappapis.html#printing">HTML5</a></td>
   <td>The associated document is about to be printed or previewed for printing.</td>
  </tr>
  <tr>
   <td>{{Event("beforeunload")}}</td>
   <td>{{DOMxRef("BeforeUnloadEvent")}}</td>
   <td><a href="http://www.w3.org/TR/html5/browsers.html#unloading-documents">HTML5</a></td>
   <td>The window, the document and its resources are about to be unloaded.</td>
  </tr>
  <tr>
   <td>{{Event("beginEvent")}}</td>
   <td>{{DOMxRef("TimeEvent")}}</td>
   <td><a href="http://www.w3.org/TR/SVG/interact.html#SVGEvents">SVG</a></td>
   <td>A <a href="/en-US/docs/SVG/SVG_animation_with_SMIL">SMIL</a> animation element begins.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/blocked_indexedDB">blocked</a></code></td>
   <td></td>
   <td><a href="http://www.w3.org/TR/IndexedDB/#request-api">IndexedDB</a></td>
   <td>An open connection to a database is blocking a <code>versionchange</code> transaction on the same database.</td>
  </tr>
  <tr>
   <td>{{Event("blur")}}</td>
   <td>{{DOMxRef("FocusEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-blur" style="white-space: nowrap;">DOM L3</a></td>
   <td>An element has lost focus (does not bubble).</td>
  </tr>
  <tr>
   <td>{{Event("boundary")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("SpeechSynthesisEvent")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>The spoken utterance reaches a word or sentence boundary</td>
  </tr>
  <tr>
   <td>{{Event("cached")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/html/wg/drafts/html/master/browsers.html#offline">Offline</a></td>
   <td>The resources listed in the manifest have been downloaded, and the application is now cached.</td>
  </tr>
  <tr>
   <td>{{Event("canplay")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-canplay" style="white-space: nowrap;">HTML5 media</a></td>
   <td>The user agent can play the media, but estimates that not enough data has been loaded to play the media up to its end without having to stop for further buffering of content.</td>
  </tr>
  <tr>
   <td>{{Event("canplaythrough")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-canplaythrough" style="white-space: nowrap;">HTML5 media</a></td>
   <td>The user agent can play the media up to its end without having to stop for further buffering of content.</td>
  </tr>
  <tr>
   <td>{{Event("change")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-2-Events/events.html">DOM L2</a>, <a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/common-input-element-attributes.html#event-input-change">HTML5</a></td>
   <td>The <code>change</code> event is fired for {{HTMLElement("input")}}, {{HTMLElement("select")}}, and {{HTMLElement("textarea")}} elements when a change to the element's value is committed by the user.</td>
  </tr>
  <tr>
   <td>{{Event("chargingchange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="https://dvcs.w3.org/hg/dap/raw-file/tip/battery/Overview.html" style="white-space: nowrap;">Battery status</a></td>
   <td>The battery begins or stops charging.</td>
  </tr>
  <tr>
   <td>{{Event("chargingtimechange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="https://dvcs.w3.org/hg/dap/raw-file/tip/battery/Overview.html" style="white-space: nowrap;">Battery status</a></td>
   <td>The <code>chargingTime</code> attribute has been updated.</td>
  </tr>
  <tr>
   <td>{{Event("checking")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/html/wg/drafts/html/master/browsers.html#offline">Offline</a></td>
   <td>The user agent is checking for an update, or attempting to download the cache manifest for the first time.</td>
  </tr>
  <tr>
   <td>{{Event("click")}}</td>
   <td>{{DOMxRef("MouseEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-click" style="white-space: nowrap;">DOM L3</a></td>
   <td>A pointing device button has been pressed and released on an element.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/close_websocket">close</a></code></td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/websockets/">WebSocket</a></td>
   <td>A WebSocket connection has been closed.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/complete_indexedDB">complete</a></code></td>
   <td></td>
   <td><a href="http://www.w3.org/TR/IndexedDB/#transaction">IndexedDB</a></td>
   <td>A transaction successfully completed.</td>
  </tr>
  <tr>
   <td>{{Event("complete")}}</td>
   <td>{{DOMxRef("OfflineAudioCompletionEvent")}} {{Deprecated_Inline}}</td>
   <td>{{SpecName('Web Audio API', '#OfflineAudioCompletionEvent-section', 'OfflineAudioCompletionEvent')}}</td>
   <td>The rendering of an {{DOMxRef("OfflineAudioContext")}} is terminated.</td>
  </tr>
  <tr>
   <td>{{Event("compositionend")}}{{gecko_minversion_inline("9")}}</td>
   <td>{{DOMxRef("CompositionEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-compositionend" style="white-space: nowrap;">DOM L3</a></td>
   <td>The composition of a passage of text has been completed or canceled.</td>
  </tr>
  <tr>
   <td>{{Event("compositionstart")}}{{gecko_minversion_inline("9")}}</td>
   <td>{{DOMxRef("CompositionEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-compositionstart" style="white-space: nowrap;">DOM L3</a></td>
   <td>The composition of a passage of text is prepared (similar to keydown for a keyboard input, but works with other inputs such as speech recognition).</td>
  </tr>
  <tr>
   <td>{{Event("compositionupdate")}}{{gecko_minversion_inline("9")}}</td>
   <td>{{DOMxRef("CompositionEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-compositionupdate" style="white-space: nowrap;">DOM L3</a></td>
   <td>A character is added to a passage of text being composed.</td>
  </tr>
  <tr>
   <td>{{Event("contextmenu")}}</td>
   <td>{{DOMxRef("MouseEvent")}}</td>
   <td><a href="https://html.spec.whatwg.org/multipage/forms.html#context-menus">HTML5</a></td>
   <td>The right button of the mouse is clicked (before the context menu is displayed).</td>
  </tr>
  <tr>
   <td>{{Event("copy")}}</td>
   <td>{{DOMxRef("ClipboardEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/clipboard-apis/#copy-event">Clipboard</a></td>
   <td>The text selection has been added to the clipboard.</td>
  </tr>
  <tr>
   <td>{{Event("cut")}}</td>
   <td>{{DOMxRef("ClipboardEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/clipboard-apis/#cut-event">Clipboard</a></td>
   <td>The text selection has been removed from the document and added to the clipboard.</td>
  </tr>
  <tr>
   <td>{{Event("dblclick")}}</td>
   <td>{{DOMxRef("MouseEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-dblclick" style="white-space: nowrap;">DOM L3</a></td>
   <td>A pointing device button is clicked twice on an element.</td>
  </tr>
  <tr>
   <td>{{Event("devicechange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{SpecName("Media Capture")}}</td>
   <td>A media device such as a camera, microphone, or speaker is connected or removed from the system.</td>
  </tr>
  <tr>
   <td>{{Event("devicelight")}}</td>
   <td>{{DOMxRef("DeviceLightEvent")}} {{Experimental_Inline}}</td>
   <td><a class="external" href="http://dvcs.w3.org/hg/dap/raw-file/tip/light/Overview.html" lang="en" title="The definition of 'Ambient Light Events' in that specification.">Ambient Light Events</a></td>
   <td>Fresh data is available from a light sensor.</td>
  </tr>
  <tr>
   <td>{{Event("devicemotion")}}</td>
   <td>{{DOMxRef("DeviceMotionEvent")}} {{Experimental_Inline}}</td>
   <td><a class="external" href="http://dev.w3.org/geo/api/spec-source-orientation.html" lang="en" title="The 'Device Orientation Events' specification">Device Orientation Events</a></td>
   <td>Fresh data is available from a motion sensor.</td>
  </tr>
  <tr>
   <td>{{Event("deviceorientation")}}</td>
   <td>{{DOMxRef("DeviceOrientationEvent")}} {{Experimental_Inline}}</td>
   <td><a class="external" href="http://dev.w3.org/geo/api/spec-source-orientation.html" lang="en" title="The 'Device Orientation Events' specification">Device Orientation Events</a></td>
   <td>Fresh data is available from an orientation sensor.</td>
  </tr>
  <tr>
   <td>{{Event("deviceproximity")}}</td>
   <td>{{DOMxRef("DeviceProximityEvent")}} {{Experimental_Inline}}</td>
   <td><a class="external" href="http://dvcs.w3.org/hg/dap/raw-file/tip/proximity/Overview.html" lang="en" title="The definition of 'Proximity Events' in that specification.">Proximity Events</a></td>
   <td>Fresh data is available from a proximity sensor (indicates an approximated distance between the device and a nearby object).</td>
  </tr>
  <tr>
   <td>{{Event("dischargingtimechange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="https://dvcs.w3.org/hg/dap/raw-file/tip/battery/Overview.html">Battery status</a></td>
   <td>The <code>dischargingTime</code> attribute has been updated.</td>
  </tr>
  <tr>
   <td><code>DOMActivate</code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("UIEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-DOMActivate" style="white-space: nowrap;">DOM L3</a></td>
   <td>A button, link or state changing element is activated (use {{Event("click")}} instead).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/DOM/Mutation_events">DOMAttributeNameChanged</a></code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("MutationNameEvent")}}</td>
   <td><a href="http://www.w3.org/TR/2011/WD-DOM-Level-3-Events-20110531/#event-type-DOMAttributeNameChanged" style="white-space: nowrap;">DOM L3</a> Removed</td>
   <td>The name of an attribute changed (use <a href="/en-US/docs/DOM/MutationObserver">mutation observers</a> instead).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/DOM/Mutation_events">DOMAttrModified</a></code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("MutationEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-DOMAttrModified" style="white-space: nowrap;">DOM L3</a></td>
   <td>The value of an attribute has been modified (use <a href="/en-US/docs/DOM/MutationObserver">mutation observers</a> instead).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/DOM/Mutation_events">DOMCharacterDataModified</a></code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("MutationEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-DOMCharacterDataModified" style="white-space: nowrap;">DOM L3</a></td>
   <td>A text or another <a href="/en-US/docs/DOM/CharacterData">CharacterData</a> has changed (use <a href="/en-US/docs/DOM/MutationObserver">mutation observers</a> instead).</td>
  </tr>
  <tr>
   <td>{{Event("DOMContentLoaded")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-end.html#the-end">HTML5</a></td>
   <td>The document has finished loading (but not its dependent resources).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/DOM/Mutation_events">DOMElementNameChanged</a></code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("MutationNameEvent")}}</td>
   <td><a href="http://www.w3.org/TR/2011/WD-DOM-Level-3-Events-20110531/#event-type-DOMElementNameChanged" style="white-space: nowrap;">DOM L3</a> Removed</td>
   <td>The name of an element changed (use <a href="/en-US/docs/DOM/MutationObserver">mutation observers</a> instead).</td>
  </tr>
  <tr>
   <td><code>DOMFocusIn</code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("FocusEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-DOMFocusIn" style="white-space: nowrap;">DOM L3</a></td>
   <td>An element has received focus (use {{Event("focus")}} or {{Event("focusin")}} instead).</td>
  </tr>
  <tr>
   <td><code>DOMFocusOut</code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("FocusEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-DOMFocusOut" style="white-space: nowrap;">DOM L3</a></td>
   <td>An element has lost focus (use {{Event("blur")}} or {{Event("focusout")}} instead).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/DOM/Mutation_events">DOMNodeInserted</a></code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("MutationEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-DOMNodeInserted" style="white-space: nowrap;">DOM L3</a></td>
   <td>A node has been added as a child of another node (use <a href="/en-US/docs/DOM/MutationObserver">mutation observers</a> instead).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/DOM/Mutation_events">DOMNodeInsertedIntoDocument</a></code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("MutationEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-DOMNodeInsertedIntoDocument" style="white-space: nowrap;">DOM L3</a></td>
   <td>A node has been inserted into the document (use <a href="/en-US/docs/DOM/MutationObserver">mutation observers</a> instead).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/DOM/Mutation_events">DOMNodeRemoved</a></code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("MutationEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-DOMNodeRemoved" style="white-space: nowrap;">DOM L3</a></td>
   <td>A node has been removed from its parent node (use <a href="/en-US/docs/DOM/MutationObserver">mutation observers</a> instead).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/DOM/Mutation_events">DOMNodeRemovedFromDocument</a></code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("MutationEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-DOMNodeRemovedFromDocument" style="white-space: nowrap;">DOM L3</a></td>
   <td>A node has been removed from the document (use <a href="/en-US/docs/DOM/MutationObserver">mutation observers</a> instead).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/DOM/Mutation_events">DOMSubtreeModified</a></code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("MutationEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-DOMSubtreeModified" style="white-space: nowrap;">DOM L3</a></td>
   <td>A change happened in the document (use <a href="/en-US/docs/DOM/MutationObserver">mutation observers</a> instead).</td>
  </tr>
  <tr>
   <td>{{Event("downloading")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/html/wg/drafts/html/master/browsers.html#offline">Offline</a></td>
   <td>The user agent has found an update and is fetching it, or is downloading the resources listed by the cache manifest for the first time.</td>
  </tr>
  <tr>
   <td>{{Event("drag")}}</td>
   <td>{{DOMxRef("DragEvent")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/dnd.html#event-drag">HTML5</a></td>
   <td>An element or text selection is being dragged (every 350ms).</td>
  </tr>
  <tr>
   <td>{{Event("dragend")}}</td>
   <td>{{DOMxRef("DragEvent")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/dnd.html#event-dragend">HTML5</a></td>
   <td>A drag operation is being ended (by releasing a mouse button or hitting the escape key).</td>
  </tr>
  <tr>
   <td>{{Event("dragenter")}}</td>
   <td>{{DOMxRef("DragEvent")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/dnd.html#event-dragenter">HTML5</a></td>
   <td>A dragged element or text selection enters a valid drop target.</td>
  </tr>
  <tr>
   <td>{{Event("dragleave")}}</td>
   <td>{{DOMxRef("DragEvent")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/dnd.html#event-dragleave">HTML5</a></td>
   <td>A dragged element or text selection leaves a valid drop target.</td>
  </tr>
  <tr>
   <td>{{Event("dragover")}}</td>
   <td>{{DOMxRef("DragEvent")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/dnd.html#event-dragover">HTML5</a></td>
   <td>An element or text selection is being dragged over a valid drop target (every 350ms).</td>
  </tr>
  <tr>
   <td>{{Event("dragstart")}}</td>
   <td>{{DOMxRef("DragEvent")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/dnd.html#event-dragstart">HTML5</a></td>
   <td>The user starts dragging an element or text selection.</td>
  </tr>
  <tr>
   <td>{{Event("drop")}}</td>
   <td>{{DOMxRef("DragEvent")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/dnd.html#event-drop">HTML5</a></td>
   <td>An element is dropped on a valid drop target.</td>
  </tr>
  <tr>
   <td>{{Event("durationchange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-durationchange">HTML5 media</a></td>
   <td>The <code>duration</code> attribute has been updated.</td>
  </tr>
  <tr>
   <td>{{Event("emptied")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-emptied">HTML5 media</a></td>
   <td>The media has become empty; for example, this event is sent if the media has already been loaded (or partially loaded), and the <a href="/en-US/docs/XPCOM_Interface_Reference/NsIDOMHTMLMediaElement" rel="internal"><code>load()</code></a> method is called to reload it.</td>
  </tr>
  <tr>
   <td>{{Event("end_(SpeechRecognition)","end")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>The speech recognition service has disconnected.</td>
  </tr>
  <tr>
   <td>{{Event("end_(SpeechSynthesis)","end")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("SpeechSynthesisEvent")}}</td>
   <td>{{SpecName("Web Speech API")}}</td>
   <td>The utterance has finished being spoken.</td>
  </tr>
  <tr>
   <td>{{Event("ended")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-ended">HTML5 media</a></td>
   <td>Playback has stopped because the end of the media was reached.</td>
  </tr>
  <tr>
   <td>{{Event("ended_(Web_Audio)", "ended")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{SpecName("Web Audio API")}}</td>
   <td>Playback has stopped because the end of the media was reached.</td>
  </tr>
  <tr>
   <td>{{Event("endEvent")}}</td>
   <td>{{DOMxRef("TimeEvent")}}</td>
   <td><a href="http://www.w3.org/TR/SVG/interact.html#SVGEvents">SVG</a></td>
   <td>A <a href="/en-US/docs/SVG/SVG_animation_with_SMIL">SMIL</a> animation element ends.</td>
  </tr>
  <tr>
   <td>{{Event("error")}}</td>
   <td>{{DOMxRef("UIEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-error" style="white-space: nowrap;">DOM L3</a></td>
   <td>A resource failed to load.</td>
  </tr>
  <tr>
   <td>{{Event("error")}}</td>
   <td>{{DOMxRef("ProgressEvent")}}</td>
   <td><a href="http://www.w3.org/TR/progress-events/">Progress</a><span> and </span><a href="http://www.w3.org/TR/XMLHttpRequest/#event-xhr-error">XMLHttpRequest</a></td>
   <td>Progression has failed.</td>
  </tr>
  <tr>
   <td>{{Event("error")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/html/wg/drafts/html/master/browsers.html#offline">Offline</a></td>
   <td>An error occurred while downloading the cache manifest or updating the content of the application.</td>
  </tr>
  <tr>
   <td>{{Event("error")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/websockets/">WebSocket</a></td>
   <td>A WebSocket connection has been closed with prejudice (some data couldn't be sent for example).</td>
  </tr>
  <tr>
   <td>{{Event("error")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://dev.w3.org/html5/eventsource/">Server Sent Events</a></td>
   <td>An event source connection has been failed.</td>
  </tr>
  <tr>
   <td>{{Event("error")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/IndexedDB/#request-api">IndexedDB</a></td>
   <td>A request caused an error and failed.</td>
  </tr>
  <tr>
   <td>{{Event("error_(SpeechRecognitionError)","error")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>A speech recognition error occurs.</td>
  </tr>
  <tr>
   <td>{{Event("error_(SpeechSynthesisError)","error")}}</td>
   <td>{{DOMxRef("SpeechSynthesisErrorEvent")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>An error occurs that prevents the utterance from being successfully spoken.</td>
  </tr>
  <tr>
   <td>{{Event("focus")}}</td>
   <td>{{DOMxRef("FocusEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-focus" style="white-space: nowrap;">DOM L3</a></td>
   <td>An element has received focus (does not bubble).</td>
  </tr>
  <tr>
   <td>{{Event("focusin")}}</td>
   <td>{{DOMxRef("FocusEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-focusIn" style="white-space: nowrap;">DOM L3</a></td>
   <td>An element is about to receive focus (bubbles).</td>
  </tr>
  <tr>
   <td>{{Event("focusout")}}</td>
   <td>{{DOMxRef("FocusEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-focusout" style="white-space: nowrap;">DOM L3</a></td>
   <td>An element is about to lose focus (bubbles).</td>
  </tr>
  <tr>
   <td>{{Event("fullscreenchange")}}{{gecko_minversion_inline("9")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="https://dvcs.w3.org/hg/fullscreen/raw-file/tip/Overview.html#api">Full Screen</a></td>
   <td>An element was turned to fullscreen mode or back to normal mode.</td>
  </tr>
  <tr>
   <td>{{Event("fullscreenerror")}}{{gecko_minversion_inline("9")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="https://dvcs.w3.org/hg/fullscreen/raw-file/tip/Overview.html#api">Full Screen</a></td>
   <td>It was impossible to switch to fullscreen mode for technical reasons or because the permission was denied.</td>
  </tr>
  <tr>
   <td>{{Event("gamepadconnected")}}</td>
   <td>{{DOMxRef("GamepadEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/gamepad/#the-gamepadconnected-event">Gamepad</a></td>
   <td>A gamepad has been connected.</td>
  </tr>
  <tr>
   <td>{{Event("gamepaddisconnected")}}</td>
   <td>{{DOMxRef("GamepadEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/gamepad/#the-gamepaddisconnected-event">Gamepad</a></td>
   <td>A gamepad has been disconnected.</td>
  </tr>
  <tr>
   <td>{{Event("gotpointercapture")}}</td>
   <td>{{DOMxRef("PointerEvent")}}</td>
   <td><a href="http://www.w3.org/TR/pointerevents/#the-gotpointercapture-event">Pointer Events</a></td>
   <td>Element receives pointer capture.</td>
  </tr>
  <tr>
   <td>{{Event("hashchange")}}</td>
   <td>{{DOMxRef("HashChangeEvent")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/history.html#event-hashchange">HTML5</a></td>
   <td>The fragment identifier of the URL has changed (the part of the URL after the #).</td>
  </tr>
  <tr>
   <td>{{Event("lostpointercapture")}}</td>
   <td>{{DOMxRef("PointerEvent")}}</td>
   <td><a href="http://www.w3.org/TR/pointerevents/#the-lostpointercapture-event">Pointer Events</a></td>
   <td>Element lost pointer capture.</td>
  </tr>
  <tr>
   <td>{{Event("input")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/html5/forms.html#common-event-behaviors">HTML5</a></td>
   <td>The value of an element changes or the content of an element with the attribute <a href="/en-US/docs/DOM/Element.contentEditable">contenteditable</a> is modified.</td>
  </tr>
  <tr>
   <td>{{Event("invalid")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/association-of-controls-and-forms.html#constraint-validation">HTML5</a></td>
   <td>A submittable element has been checked and doesn't satisfy its constraints.</td>
  </tr>
  <tr>
   <td>{{Event("keydown")}}</td>
   <td>{{DOMxRef("KeyboardEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-keydown" style="white-space: nowrap;">DOM L3</a></td>
   <td>A key is pressed down.</td>
  </tr>
  <tr>
   <td>{{Event("keypress")}}</td>
   <td>{{DOMxRef("KeyboardEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-keypress" style="white-space: nowrap;">DOM L3</a></td>
   <td>A key is pressed down and that key normally produces a character value (use input instead).</td>
  </tr>
  <tr>
   <td>{{Event("keyup")}}</td>
   <td>{{DOMxRef("KeyboardEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-keyup" style="white-space: nowrap;">DOM L3</a></td>
   <td>A key is released.</td>
  </tr>
  <tr>
   <td>{{Event("languagechange")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{ SpecName('HTML5.1', '#dom-navigator-languages', 'NavigatorLanguage.languages') }}</td>
   <td>The user's preferred languages have changed.</td>
  </tr>
  <tr>
   <td>{{Event("levelchange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="https://dvcs.w3.org/hg/dap/raw-file/tip/battery/Overview.html">Battery status</a></td>
   <td>The <code>level</code> attribute has been updated.</td>
  </tr>
  <tr>
   <td>{{Event("load")}}</td>
   <td>{{DOMxRef("UIEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-load" style="white-space: nowrap;">DOM L3</a></td>
   <td>A resource and its dependent resources have finished loading.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/load_(ProgressEvent)">load</a></code></td>
   <td>{{DOMxRef("ProgressEvent")}}</td>
   <td><a href="http://www.w3.org/TR/progress-events/">Progress</a><span> <span>and </span></span><a href="http://www.w3.org/TR/XMLHttpRequest/#event-xhr-load">XMLHttpRequest</a></td>
   <td>Progression has been successful.</td>
  </tr>
  <tr>
   <td>{{Event("loadeddata")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-loadeddata">HTML5 media</a></td>
   <td>The first frame of the media has finished loading.</td>
  </tr>
  <tr>
   <td>{{Event("loadedmetadata")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-loadedmetadata">HTML5 media</a></td>
   <td>The metadata has been loaded.</td>
  </tr>
  <tr>
   <td>{{Event("loadend")}}</td>
   <td>{{DOMxRef("ProgressEvent")}}</td>
   <td><a href="http://www.w3.org/TR/progress-events/">Progress</a><span> <span>and </span></span><a href="http://www.w3.org/TR/XMLHttpRequest/#event-xhr-loadend">XMLHttpRequest</a></td>
   <td>Progress has stopped (after "error", "abort" or "load" have been dispatched).</td>
  </tr>
  <tr>
   <td>{{Event("loadstart")}}</td>
   <td>{{DOMxRef("ProgressEvent")}}</td>
   <td><a href="http://www.w3.org/TR/progress-events/">Progress </a><span>and </span><a href="http://www.w3.org/TR/XMLHttpRequest/#event-xhr-loadstart">XMLHttpRequest</a></td>
   <td>Progress has begun.</td>
  </tr>
  <tr>
   <td>{{Event("mark")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("SpeechSynthesisEvent")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>The spoken utterance reaches a named SSML "mark" tag.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/message_websocket">message</a></code></td>
   <td>{{DOMxRef("MessageEvent")}}</td>
   <td><a href="http://www.w3.org/TR/websockets/">WebSocket</a></td>
   <td>A message is received through a WebSocket.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/message_webworker">message</a></code></td>
   <td>{{DOMxRef("MessageEvent")}}</td>
   <td><a href="http://www.w3.org/TR/workers/#communicating-with-a-dedicated-worker">Web Workers</a></td>
   <td>A message is received from a Web Worker.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/message_webmessaging">message</a></code></td>
   <td>{{DOMxRef("MessageEvent")}}</td>
   <td><a href="http://www.w3.org/TR/webmessaging/">Web Messaging</a></td>
   <td>A message is received from a child (i)frame or a parent window.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/message_serversentevents">message</a></code></td>
   <td>{{DOMxRef("MessageEvent")}}</td>
   <td><a href="http://dev.w3.org/html5/eventsource/">Server Sent Events</a></td>
   <td>A message is received through an event source.</td>
  </tr>
  <tr>
   <td>{{Event("messageerror")}}</td>
   <td>{{DOMxRef("MessageEvent")}}</td>
   <td>{{DOMxRef("MessagePort")}}, <a href="/en-US/docs/Web/API/Web_Workers_API">Web Workers</a>, <a href="/en-US/docs/Web/API/Broadcast_Channel_API">Broadcast Channel</a>, {{DOMxRef("Window")}}</td>
   <td>A message error is raised when a message is received by an object.</td>
  </tr>
  <tr>
   <td>{{Event("message_(ServiceWorker)","message")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("ServiceWorkerMessageEvent")}} or {{DOMxRef("ExtendableMessageEvent")}}, depending on context.</td>
   <td><a href="/en-US/docs/Web/API/Service_Worker_API">Service Workers</a></td>
   <td>A message is received from a service worker, or a message is received in a service worker from another context.</td>
  </tr>
  <tr>
   <td>{{Event("mousedown")}}</td>
   <td>{{DOMxRef("MouseEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-mousedown" style="white-space: nowrap;">DOM L3</a></td>
   <td>A pointing device button (usually a mouse) is pressed on an element.</td>
  </tr>
  <tr>
   <td>{{Event("mouseenter")}}</td>
   <td>{{DOMxRef("MouseEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-mouseenter" style="white-space: nowrap;">DOM L3</a></td>
   <td>A pointing device is moved onto the element that has the listener attached.</td>
  </tr>
  <tr>
   <td>{{Event("mouseleave")}}</td>
   <td>{{DOMxRef("MouseEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-mouseleave" style="white-space: nowrap;">DOM L3</a></td>
   <td>A pointing device is moved off the element that has the listener attached.</td>
  </tr>
  <tr>
   <td>{{Event("mousemove")}}</td>
   <td>{{DOMxRef("MouseEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-mousemove" style="white-space: nowrap;">DOM L3</a></td>
   <td>A pointing device is moved over an element.</td>
  </tr>
  <tr>
   <td>{{Event("mouseout")}}</td>
   <td>{{DOMxRef("MouseEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-mouseout" style="white-space: nowrap;">DOM L3</a></td>
   <td>A pointing device is moved off the element that has the listener attached or off one of its children.</td>
  </tr>
  <tr>
   <td>{{Event("mouseover")}}</td>
   <td>{{DOMxRef("MouseEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-mouseover" style="white-space: nowrap;">DOM L3</a></td>
   <td>A pointing device is moved onto the element that has the listener attached or onto one of its children.</td>
  </tr>
  <tr>
   <td>{{Event("mouseup")}}</td>
   <td>{{DOMxRef("MouseEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-mouseup" style="white-space: nowrap;">DOM L3</a></td>
   <td>A pointing device button is released over an element.</td>
  </tr>
  <tr>
   <td>{{Event("nomatch")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("SpeechRecognitionEvent")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>The speech recognition service returns a final result with no significant recognition.</td>
  </tr>
  <tr>
   <td>{{Event("notificationclick")}}</td>
   <td>{{DOMxRef("NotificationEvent")}} {{Experimental_Inline}}</td>
   <td>{{SpecName('Web Notifications','#dom-serviceworkerglobalscope-onnotificationclick','onnotificationclick')}}</td>
   <td>A system notification<span style="line-height: 19.0909080505371px;"> spawned by {{DOMxRef("ServiceWorkerRegistration.showNotification()")}} has been clicked.</span></td>
  </tr>
  <tr>
   <td>{{Event("noupdate")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/html/wg/drafts/html/master/browsers.html#offline">Offline</a></td>
   <td>The manifest hadn't changed.</td>
  </tr>
  <tr>
   <td>{{Event("obsolete")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/html/wg/drafts/html/master/browsers.html#offline">Offline</a></td>
   <td>The manifest was found to have become a 404 or 410 page, so the application cache is being deleted.</td>
  </tr>
  <tr>
   <td>{{Event("offline")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/offline.html#event-offline">HTML5 offline</a></td>
   <td>The browser has lost access to the network.</td>
  </tr>
  <tr>
   <td>{{Event("online")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/offline.html#event-online">HTML5 offline</a></td>
   <td>The browser has gained access to the network (but particular websites might be unreachable).</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/open_websocket">open</a></code></td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/websockets/">WebSocket</a></td>
   <td>A WebSocket connection has been established.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/open_serversentevents">open</a></code></td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://dev.w3.org/html5/eventsource/">Server Sent Events</a></td>
   <td>An event source connection has been established.</td>
  </tr>
  <tr>
   <td>{{Event("orientationchange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/screen-orientation/">Screen Orientation</a></td>
   <td>The orientation of the device (portrait/landscape) has changed</td>
  </tr>
  <tr>
   <td>{{Event("pagehide")}}</td>
   <td>{{DOMxRef("PageTransitionEvent")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/history.html#event-pagehide">HTML5</a></td>
   <td>A session history entry is being traversed from.</td>
  </tr>
  <tr>
   <td>{{Event("pageshow")}}</td>
   <td>{{DOMxRef("PageTransitionEvent")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/history.html#event-pageshow">HTML5</a></td>
   <td>A session history entry is being traversed to.</td>
  </tr>
  <tr>
   <td>{{Event("paste")}}</td>
   <td>{{DOMxRef("ClipboardEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/clipboard-apis/#paste-event">Clipboard</a></td>
   <td>Data has been transferred from the system clipboard to the document.</td>
  </tr>
  <tr>
   <td>{{Event("pause")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-pause">HTML5 media</a></td>
   <td>Playback has been paused.</td>
  </tr>
  <tr>
   <td>{{Event("pause_(SpeechSynthesis)", "pause")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("SpeechSynthesisEvent")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>The utterance is paused part way through.</td>
  </tr>
  <tr>
   <td>{{Event("pointercancel")}}</td>
   <td>{{DOMxRef("PointerEvent")}}</td>
   <td><a href="http://www.w3.org/TR/pointerevents/#the-pointercancel-event">Pointer Events</a></td>
   <td>The pointer is unlikely to produce any more events.</td>
  </tr>
  <tr>
   <td>{{Event("pointerdown")}}</td>
   <td>{{DOMxRef("PointerEvent")}}</td>
   <td><a href="http://www.w3.org/TR/pointerevents/#the-pointerdown-event">Pointer Events</a></td>
   <td>The pointer enters the active buttons state.</td>
  </tr>
  <tr>
   <td>{{Event("pointerenter")}}</td>
   <td>{{DOMxRef("PointerEvent")}}</td>
   <td><a href="http://www.w3.org/TR/pointerevents/#the-pointerenter-event">Pointer Events</a></td>
   <td>Pointing device is moved inside the hit-testing boundary.</td>
  </tr>
  <tr>
   <td>{{Event("pointerleave")}}</td>
   <td>{{DOMxRef("PointerEvent")}}</td>
   <td><a href="http://www.w3.org/TR/pointerevents/#the-pointerleave-event">Pointer Events</a></td>
   <td>Pointing device is moved out of the hit-testing boundary.</td>
  </tr>
  <tr>
   <td>{{Event("pointerlockchange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/pointerlock/#pointerlockchange-and-pointerlockerror-events">Pointer Lock</a></td>
   <td>The pointer was locked or released.</td>
  </tr>
  <tr>
   <td>{{Event("pointerlockerror")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/pointerlock/#pointerlockchange-and-pointerlockerror-events">Pointer Lock</a></td>
   <td>It was impossible to lock the pointer for technical reasons or because the permission was denied.</td>
  </tr>
  <tr>
   <td>{{Event("pointermove")}}</td>
   <td>{{DOMxRef("PointerEvent")}}</td>
   <td><a href="http://www.w3.org/TR/pointerevents/#the-pointermove-event">Pointer Events</a></td>
   <td>The pointer changed coordinates.</td>
  </tr>
  <tr>
   <td>{{Event("pointerout")}}</td>
   <td>{{DOMxRef("PointerEvent")}}</td>
   <td><a href="http://www.w3.org/TR/pointerevents/#the-pointerout-event">Pointer Events</a></td>
   <td>The pointing device moved out of hit-testing boundary or leaves detectable hover range.</td>
  </tr>
  <tr>
   <td>{{Event("pointerover")}}</td>
   <td>{{DOMxRef("PointerEvent")}}</td>
   <td><a href="http://www.w3.org/TR/pointerevents/#the-pointerover-event">Pointer Events</a></td>
   <td>The pointing device is moved into the hit-testing boundary.</td>
  </tr>
  <tr>
   <td>{{Event("pointerup")}}</td>
   <td>{{DOMxRef("PointerEvent")}}</td>
   <td><a href="http://www.w3.org/TR/pointerevents/#the-pointerup-event">Pointer Events</a></td>
   <td>The pointer leaves the active buttons state.</td>
  </tr>
  <tr>
   <td>{{Event("play")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-play">HTML5 media</a></td>
   <td>Playback has begun.</td>
  </tr>
  <tr>
   <td>{{Event("playing")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-playing">HTML5 media</a></td>
   <td>Playback is ready to start after having been paused or delayed due to lack of data.</td>
  </tr>
  <tr>
   <td>{{Event("popstate")}}</td>
   <td>{{DOMxRef("PopStateEvent")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/history.html#event-popstate">HTML5</a></td>
   <td>A session history entry is being navigated to (in certain cases).</td>
  </tr>
  <tr>
   <td>{{Event("progress")}}</td>
   <td>{{DOMxRef("ProgressEvent")}}</td>
   <td><a href="http://www.w3.org/TR/progress-events/">Progress</a><span> <span>and </span></span><a href="http://www.w3.org/TR/XMLHttpRequest/#event-xhr-progress">XMLHttpRequest</a></td>
   <td>In progress.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/progress_(appcache_event)">progress</a></code></td>
   <td>{{DOMxRef("ProgressEvent")}}</td>
   <td><a href="http://www.w3.org/html/wg/drafts/html/master/browsers.html#offline">Offline</a></td>
   <td>The user agent is downloading resources listed by the manifest.</td>
  </tr>
  <tr>
   <td>{{Event("push")}}</td>
   <td>{{DOMxRef("PushEvent")}} {{Experimental_Inline}}</td>
   <td>{{SpecName("Push API")}}</td>
   <td>A <a href="/en-US/docs/Web/API/Service_Worker_API">Service Worker</a> has received a push message.</td>
  </tr>
  <tr>
   <td>{{Event("pushsubscriptionchange")}}</td>
   <td>{{DOMxRef("PushEvent")}} {{Experimental_Inline}}</td>
   <td>{{SpecName("Push API")}}</td>
   <td>A <a href="/en-US/docs/Web/API/PushSubscription">PushSubscription</a> has expired.</td>
  </tr>
  <tr>
   <td>{{Event("ratechange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-ratechange">HTML5 media</a></td>
   <td>The playback rate has changed.</td>
  </tr>
  <tr>
   <td>{{Event("readystatechange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><span>HTML5 <span>and </span></span><a href="http://www.w3.org/TR/XMLHttpRequest/#event-xhr-readystatechange">XMLHttpRequest</a></td>
   <td>The readyState attribute of a document has changed.</td>
  </tr>
  <tr>
   <td>{{Event("repeatEvent")}}</td>
   <td>{{DOMxRef("TimeEvent")}}</td>
   <td><a href="http://www.w3.org/TR/SVG/interact.html#SVGEvents">SVG</a></td>
   <td>A <a href="/en-US/docs/SVG/SVG_animation_with_SMIL">SMIL</a> animation element is repeated.</td>
  </tr>
  <tr>
   <td>{{Event("reset")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-2-Events/events.html">DOM L2</a>, <a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/association-of-controls-and-forms.html#form-submission-0#resetting-a-form">HTML5</a></td>
   <td>A form is reset.</td>
  </tr>
  <tr>
   <td>{{Event("resize")}}</td>
   <td>{{DOMxRef("UIEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-resize" style="white-space: nowrap;">DOM L3</a></td>
   <td>The document view has been resized.</td>
  </tr>
  <tr>
   <td>{{Event("resourcetimingbufferfull")}}</td>
   <td>{{DOMxRef("Performance")}}</td>
   <td><a href="https://w3c.github.io/resource-timing/#dom-performance-onresourcetimingbufferfull">Resource Timing</a></td>
   <td>The browser's resource timing buffer is full.</td>
  </tr>
  <tr>
   <td>{{Event("result")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("SpeechRecognitionEvent")}} {{Experimental_Inline}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>The speech recognition service returns a result — a word or phrase has been positively recognized and this has been communicated back to the app.</td>
  </tr>
  <tr>
   <td>{{Event("resume")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("SpeechSynthesisEvent")}} {{Experimental_Inline}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>A paused utterance is resumed.</td>
  </tr>
  <tr>
   <td>{{Event("scroll")}}</td>
   <td>{{DOMxRef("UIEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-scroll" style="white-space: nowrap;">DOM L3</a></td>
   <td>The document view or an element has been scrolled.</td>
  </tr>
  <tr>
   <td>{{Event("seeked")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-seeked">HTML5 media</a></td>
   <td>A <em>seek</em> operation completed.</td>
  </tr>
  <tr>
   <td>{{Event("seeking")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-seeking">HTML5 media</a></td>
   <td>A <em>seek</em> operation began.</td>
  </tr>
  <tr>
   <td>{{Event("select")}}</td>
   <td>{{DOMxRef("UIEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-select" style="white-space: nowrap;">DOM L3</a></td>
   <td>Some text is being selected.</td>
  </tr>
  <tr>
   <td>{{Event("selectstart")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{ SpecName('Selection API')}}</td>
   <td>A selection just started.</td>
  </tr>
  <tr>
   <td>{{Event("selectionchange")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{ SpecName('Selection API')}}</td>
   <td>The selection in the document has been changed.</td>
  </tr>
  <tr>
   <td>{{Event("show")}}</td>
   <td>{{DOMxRef("MouseEvent")}}</td>
   <td><a href="http://www.w3.org/TR/html5/interactive-elements.html#context-menus">HTML5</a></td>
   <td>A contextmenu event was fired on/bubbled to an element that has a <a href="/en-US/docs/DOM/element.contextmenu">contextmenu</a> attribute</td>
  </tr>
  <tr>
   <td>{{Event("slotchange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{ SpecName('DOM WHATWG')}}</td>
   <td>The node contents of a {{DOMxRef("HTMLSlotElement")}} ({{htmlelement("slot")}}) have changed.</td>
  </tr>
  <tr>
   <td>{{Event("soundend")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>Any sound — recognisable speech or not — has stopped being detected.</td>
  </tr>
  <tr>
   <td>{{Event("soundstart")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>Any sound — recognisable speech or not — has been detected.</td>
  </tr>
  <tr>
   <td>{{Event("speechend")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>Speech recognised by the speech recognition service has stopped being detected.</td>
  </tr>
  <tr>
   <td>{{Event("speechstart")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>Sound that is recognised by the speech recognition service as speech has been detected.</td>
  </tr>
  <tr>
   <td>{{Event("stalled")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-stalled">HTML5 media</a></td>
   <td>The user agent is trying to fetch media data, but data is unexpectedly not forthcoming.</td>
  </tr>
  <tr>
   <td>{{Event("start_(SpeechRecognition)","start")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>The speech recognition service has begun listening to incoming audio with intent to recognize grammars associated with the current <code>SpeechRecognition</code>.</td>
  </tr>
  <tr>
   <td>{{Event("start_(SpeechSynthesis)","start")}}</td>
   <td>{{DOMxRef("SpeechSynthesisEvent")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>The utterance has begun to be spoken.</td>
  </tr>
  <tr>
   <td>{{Event("storage")}}</td>
   <td>{{DOMxRef("StorageEvent")}}</td>
   <td><a href="http://www.w3.org/TR/webstorage/#the-storage-event">Web Storage</a></td>
   <td>A storage area (<a href="/en-US/docs/DOM/Storage#localStorage">localStorage</a> or <a href="/en-US/docs/DOM/Storage#sessionStorage">sessionStorage</a>) has changed.</td>
  </tr>
  <tr>
   <td>{{Event("submit")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-2-Events/events.html">DOM L2</a>, <a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/association-of-controls-and-forms.html#form-submission-algorithm">HTML5</a></td>
   <td>A form is submitted.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/success_indexedDB">success</a></code></td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/IndexedDB/#request-api">IndexedDB</a></td>
   <td>A request successfully completed.</td>
  </tr>
  <tr>
   <td>{{Event("suspend")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-suspend">HTML5 media</a></td>
   <td>Media data loading has been suspended.</td>
  </tr>
  <tr>
   <td>{{Event("SVGAbort")}}</td>
   <td>{{DOMxRef("SVGEvent")}}</td>
   <td><a href="http://www.w3.org/TR/SVG/interact.html#SVGEvents">SVG</a></td>
   <td>Page loading has been stopped before the <a href="/en-US/docs/SVG">SVG</a> was loaded.</td>
  </tr>
  <tr>
   <td>{{Event("SVGError")}}</td>
   <td>{{DOMxRef("SVGEvent")}}</td>
   <td><a href="http://www.w3.org/TR/SVG/interact.html#SVGEvents">SVG</a></td>
   <td>An error has occurred before the <a href="/en-US/docs/SVG">SVG</a> was loaded.</td>
  </tr>
  <tr>
   <td>{{Event("SVGLoad")}}</td>
   <td>{{DOMxRef("SVGEvent")}}</td>
   <td><a href="http://www.w3.org/TR/SVG/interact.html#SVGEvents">SVG</a></td>
   <td>An <a href="/en-US/docs/SVG">SVG</a> document has been loaded and parsed.</td>
  </tr>
  <tr>
   <td>{{Event("SVGResize")}}</td>
   <td>{{DOMxRef("SVGEvent")}}</td>
   <td><a href="http://www.w3.org/TR/SVG/interact.html#SVGEvents">SVG</a></td>
   <td>An <a href="/en-US/docs/SVG">SVG</a> document is being resized.</td>
  </tr>
  <tr>
   <td>{{Event("SVGScroll")}}</td>
   <td>{{DOMxRef("SVGEvent")}}</td>
   <td><a href="http://www.w3.org/TR/SVG/interact.html#SVGEvents">SVG</a></td>
   <td>An <a href="/en-US/docs/SVG">SVG</a> document is being scrolled.</td>
  </tr>
  <tr>
   <td>{{Event("SVGUnload")}}</td>
   <td>{{DOMxRef("SVGEvent")}}</td>
   <td><a href="http://www.w3.org/TR/SVG/interact.html#SVGEvents">SVG</a></td>
   <td>An <a href="/en-US/docs/SVG">SVG</a> document has been removed from a window or frame.</td>
  </tr>
  <tr>
   <td>{{Event("SVGZoom")}}</td>
   <td>{{DOMxRef("SVGZoomEvent")}}</td>
   <td><a href="http://www.w3.org/TR/SVG/interact.html#SVGEvents">SVG</a></td>
   <td>An <a href="/en-US/docs/SVG">SVG</a> document is being zoomed.</td>
  </tr>
  <tr>
   <td>{{Event("timeout")}}</td>
   <td>{{DOMxRef("ProgressEvent")}}</td>
   <td><a href="http://www.w3.org/TR/XMLHttpRequest/#event-xhr-timeout">XMLHttpRequest</a></td>
   <td></td>
  </tr>
  <tr>
   <td>{{Event("timeupdate")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-timeupdate">HTML5 media</a></td>
   <td>The time indicated by the <code>currentTime</code> attribute has been updated.</td>
  </tr>
  <tr>
   <td>{{Event("touchcancel")}}</td>
   <td>{{DOMxRef("TouchEvent")}}</td>
   <td><a href="http://www.w3.org/TR/touch-events/">Touch Events</a></td>
   <td>A touch point has been disrupted in an implementation-specific manners (too many touch points for example).</td>
  </tr>
  <tr>
   <td>{{Event("touchend")}}</td>
   <td>{{DOMxRef("TouchEvent")}}</td>
   <td><a href="http://www.w3.org/TR/touch-events/#the-touchend-event">Touch Events</a></td>
   <td>A touch point is removed from the touch surface.</td>
  </tr>
  <tr>
   <td>{{Event("touchmove")}}</td>
   <td>{{DOMxRef("TouchEvent")}}</td>
   <td><a href="http://www.w3.org/TR/touch-events/#the-touchmove-event">Touch Events</a></td>
   <td>A touch point is moved along the touch surface.</td>
  </tr>
  <tr>
   <td>{{Event("touchstart")}}</td>
   <td>{{DOMxRef("TouchEvent")}}</td>
   <td><a href="http://www.w3.org/TR/touch-events/#the-touchstart---------event">Touch Events</a></td>
   <td>A touch point is placed on the touch surface.</td>
  </tr>
  <tr>
   <td>{{Event("transitionend")}}</td>
   <td>{{DOMxRef("TransitionEvent")}} {{Experimental_Inline}}</td>
   <td><a href="http://www.w3.org/TR/css3-transitions/#transition-events">CSS Transitions</a></td>
   <td>A <a href="/en-US/docs/CSS/CSS_transitions">CSS transition</a> has completed.</td>
  </tr>
  <tr>
   <td>{{Event("unload")}}</td>
   <td>{{DOMxRef("UIEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-unload" style="white-space: nowrap;">DOM L3</a></td>
   <td>The document or a dependent resource is being unloaded.</td>
  </tr>
  <tr>
   <td>{{Event("updateready")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://dev.w3.org/html5/spec/offline.html">Offline</a></td>
   <td>The resources listed in the manifest have been newly redownloaded, and the script can use <code>swapCache()</code> to switch to the new cache.</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/upgradeneeded_indexedDB">upgradeneeded</a></code></td>
   <td></td>
   <td><a href="http://www.w3.org/TR/IndexedDB/#request-api">IndexedDB</a></td>
   <td>An attempt was made to open a database with a version number higher than its current version. A <code>versionchange</code> transaction has been created.</td>
  </tr>
  <tr>
   <td>{{Event("userproximity")}}</td>
   <td>{{DOMxRef("UserProximityEvent")}} {{Experimental_Inline}}</td>
   <td>{{SpecName("Proximity Events")}}</td>
   <td>Fresh data is available from a proximity sensor (indicates whether the nearby object is <code>near</code> the device or not).</td>
  </tr>
  <tr>
   <td>{{Event("voiceschanged")}} {{Experimental_Inline}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td>{{SpecName('Web Speech API')}}</td>
   <td>The list of {{DOMxRef("SpeechSynthesisVoice")}} objects that would be returned by the {{DOMxRef("SpeechSynthesis.getVoices()")}} method has changed (when the {{Event("voiceschanged")}} event fires.)</td>
  </tr>
  <tr>
   <td><code><a href="/en-US/docs/Web/Reference/Events/versionchange_indexedDB">versionchange</a></code></td>
   <td></td>
   <td><a href="http://www.w3.org/TR/IndexedDB/#database-interface">IndexedDB</a></td>
   <td>A <code>versionchange</code> transaction completed.</td>
  </tr>
  <tr>
   <td>{{Event("visibilitychange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.w3.org/TR/page-visibility/#sec-visibilitychange-event">Page visibility</a></td>
   <td>The content of a tab has become visible or has been hidden.</td>
  </tr>
  <tr>
   <td>{{Event("volumechange")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-volumechange">HTML5 media</a></td>
   <td>The volume has changed.</td>
  </tr>
  <tr>
   <td>{{Event("waiting")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/the-video-element.html#event-media-waiting">HTML5 media</a></td>
   <td>Playback has stopped because of a temporary lack of data.</td>
  </tr>
  <tr>
   <td>{{Event("wheel")}}{{gecko_minversion_inline("17")}}</td>
   <td>{{DOMxRef("WheelEvent")}}</td>
   <td><a href="http://www.w3.org/TR/DOM-Level-3-Events/#event-type-wheel" style="white-space: nowrap;">DOM L3</a></td>
   <td>A wheel button of a pointing device is rotated in any direction.</td>
  </tr>
 </tbody>
</table>
</div>

<h2 id="비표준_이벤트">비표준 이벤트</h2>

<div style="overflow: auto;">
<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">이벤트명</th>
   <th scope="col">이벤트 타입</th>
   <th scope="col">명세</th>
   <th scope="col">발생하는 시점</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("afterscriptexecute")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><em>Mozilla Specific</em></td>
   <td>스크립트가 실행되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("beforescriptexecute")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><em>Mozilla Specific</em></td>
   <td>스크립트가 실행될 때 쯤.</td>
  </tr>
  <tr>
   <td>{{Event("beforeinstallprompt")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><em>Chrome specific</em></td>
   <td>사용자가 웹사이트를 모바일의 홈 화면에 저장하기 위한 프롬프트를 했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("cardstatechange")}}</td>
   <td></td>
   <td><em>Firefox OS specific</em></td>
   <td>{{DOMxRef("MozMobileConnection.cardState")}} 속성이 값을 변경할 때.</td>
  </tr>
  <tr>
   <td>{{Event("change")}}</td>
   <td>{{DOMxRef("DeviceStorageChangeEvent")}}</td>
   <td><em>Firefox OS specific</em></td>
   <td>이 이벤트는 파일이 주어진 저장소에서 생성, 수정, 삭제될 때마다 실행됩니다.</td>
  </tr>
  <tr>
   <td>{{Event("connectionInfoUpdate")}}</td>
   <td></td>
   <td><a href="http://mxr.mozilla.org/mozilla-central/source/dom/wifi/nsIWifi.idl?rev=3e586802f478#176"><em>Firefox OS specific</em></a></td>
   <td>신호 강도에 대한 정보와 링크 속도가 업데이트 되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("cfstatechange")}}</td>
   <td></td>
   <td><em>Firefox OS specific</em></td>
   <td>착신 전환 상태가 변경될 때.</td>
  </tr>
  <tr>
   <td>{{Event("datachange")}}</td>
   <td></td>
   <td><em>Firefox OS specific</em></td>
   <td>{{DOMxRef("MozMobileConnection.data")}} 객체가 값을 변경할 때.</td>
  </tr>
  <tr>
   <td>{{Event("dataerror")}}</td>
   <td></td>
   <td><em>Firefox OS specific</em></td>
   <td>{{DOMxRef("MozMobileConnection.data")}} 객체가 <abbr title="Radio Interface Layer">RIL</abbr> 로부터 에러를 수신했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("DOMMouseScroll")}}{{Deprecated_Inline}}</td>
   <td></td>
   <td><em>Mozilla specific</em></td>
   <td>포인팅 장치의 휠 버튼이 회전했을 때(detail 속성은 라인의 수 입니다). (대신 {{Event("wheel")}} 을 사용하세요)</td>
  </tr>
  <tr>
   <td><code>dragdrop</code> {{Deprecated_Inline}}</td>
   <td><code>DragEvent</code></td>
   <td><em>Mozilla specific</em></td>
   <td>엘리먼트가 드랍됐을 때(대신 {{Event("drop")}} 을 사용하세요).</td>
  </tr>
  <tr>
   <td><code>dragexit</code> {{Deprecated_Inline}}</td>
   <td><code>DragEvent</code></td>
   <td><em>Mozilla specific</em></td>
   <td>드래그 작업이 종료될 때(대신 {{Event("dragend")}} 를 사용하세요).</td>
  </tr>
  <tr>
   <td><code>draggesture</code> {{Deprecated_Inline}}</td>
   <td><code>DragEvent</code></td>
   <td><em>Mozilla specific</em></td>
   <td>사용자가 엘리먼트나 텍스트 선택을 드래그하기 시작할 때(대신 {{Event("dragstart")}} 를 사용하세요).</td>
  </tr>
  <tr>
   <td>{{Event("icccardlockerror")}}</td>
   <td></td>
   <td><em>Firefox OS specific</em></td>
   <td>{{DOMxRef("MozMobileConnection.unlockCardLock()")}} 또는 {{DOMxRef("MozMobileConnection.setCardLock()")}} 메소드가 실패할 때.</td>
  </tr>
  <tr>
   <td>{{Event("iccinfochange")}}</td>
   <td></td>
   <td><em>Firefox OS specific</em></td>
   <td>{{DOMxRef("MozMobileConnection.iccInfo")}} 객체가 변경할 때.</td>
  </tr>
  <tr>
   <td>{{Event("localized")}}</td>
   <td></td>
   <td><em><a href="https://github.com/fabi1cazenave/webL10n">Mozilla Specific</a></em></td>
   <td>페이지가 data-l10n-* 속성을 사용해 지역화되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("mousewheel")}}{{Deprecated_Inline}}</td>
   <td></td>
   <td><a href="http://msdn.microsoft.com/en-us/library/ie/ms536951%28v=vs.85%29.aspx"><em>IE invented</em></a></td>
   <td>포인팅 장치의 휠 버튼이 회전했을 때.</td>
  </tr>
  <tr>
   <td>{{Event("MozAudioAvailable")}}</td>
   <td>{{DOMxRef("Event")}}</td>
   <td><em>Mozilla specific</em></td>
   <td>오디오 버퍼가 가득차고 해당되는 원본 샘플이 사용가능 할 때.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozBeforeResize"><code>MozBeforeResize</code></a> {{deprecated_inline}}</td>
   <td></td>
   <td><em>Mozilla specific</em></td>
   <td>창이 리사이즈 될 때 쯤.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowseractivitydone")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>어떤 활동이 완료될 때 전송됩니다(전체 설명 미정.)</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserasyncscroll")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>브라우저 {{HTMLElement("iframe")}} 의 스크롤 위치가 변경될 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowseraudioplaybackchange")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>브라우저 {{HTMLElement("iframe")}} 컨텐츠의 오디오 재생이 시작되거나 중지될 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowsercaretstatechanged")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>브라우저 {{HTMLElement("iframe")}} 컨텐츠내의 선택된 텍스트가 변경할 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserclose")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>브라우저 {{HTMLElement("iframe")}} 에서 window.close() 가 호출될 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowsercontextmenu")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>브라우저 {{HTMLElement("iframe")}} 이 컨텍스트 메뉴 열기를 시도할 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserdocumentfirstpaint")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>브라우저 {{HTMLElement("iframe")}} 내의 다큐먼트에서 새로운 페인트가 발생할 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowsererror")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>브라우저 iframe 에서 컨텐츠 로딩을 시도하는동안 에러가 발생할 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserfindchange")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>브라우저 {{HTMLElement("iframe")}} 컨텐츠에서 검색 작업이 실행될 때(<a href="/en-US/docs/Web/API/HTMLIFrameElement#Search_methods">HTMLIFrameElement search methods</a> 문서를 보세요.)</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserfirstpaint")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>{{HTMLElement("iframe")}} 이 첫 번째로 컨텐츠를 페인트할 때(about:blank 에서의 첫 페인트는 포함하지 않습니다.)</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowsericonchange")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>브라우저 iframe 의 favicon 이 변경될 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserlocationchange")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>브라우저 iframe 의 위치가 변경될 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserloadend")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>브라우저 iframe 이 모든 자원의 로딩을 마쳤을 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserloadstart")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>브라우저 irame 이 새로운 페이지 로딩을 시작할 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowsermanifestchange")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>열린 웹 앱이 포함된 브라우저 {{HTMLElement("iframe")}} 의 경우, 앱 매니페스트의 경로가 변경될 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowsermetachange")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>{{htmlelement("meta")}} 엘리먼트가 브라우저 {{HTMLElement("iframe")}} 의 컨텐츠에서 추가, 제거, 변경될 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowseropensearch")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>검색 엔진의 링크가 발견되었을 때.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowseropentab")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>Sent when a new tab is opened within a browser {{HTMLElement("iframe")}} as a result of the user issuing a command to open a link target in a new tab (for example <kbd>ctrl</kbd>/<kbd>cmd</kbd> + click.)</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowseropenwindow")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>Sent when {{DOMxRef("window.open()")}} is called within a browser iframe.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserresize")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>Sent when the browser {{HTMLElement("iframe")}}'s window size has changed.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserscroll")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>Sent when the browser {{HTMLElement("iframe")}} content scrolls.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserscrollareachanged")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>Sent when the available scrolling area  in the browser {{HTMLElement("iframe")}} changes. This can occur on resize and when the page size changes (while loading for example.)</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserscrollviewchange")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>Sent when asynchronous scrolling (i.e. APCZ) starts or stops.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowsersecuritychange")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>Sent when the SSL state changes within a browser iframe.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserselectionstatechanged")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>Sent when the text selected inside the browser {{HTMLElement("iframe")}} content changes. Note that this is deprecated, and newer implementations use {{Event("mozbrowsercaretstatechanged")}} instead.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowsershowmodalprompt")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>Sent when {{DOMxRef("window.alert","alert()")}}, {{DOMxRef("window.confirm","confirm()")}} or {{DOMxRef("window.prompt","prompt()")}} are called within a browser iframe</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowsertitlechange")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>Sent when the document.title changes within a browser iframe.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowserusernameandpasswordrequired")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>Sent when an HTTP authentification is requested.</td>
  </tr>
  <tr>
   <td>{{Event("mozbrowservisibilitychange")}}</td>
   <td></td>
   <td><em>Firefox OS <a href="/en-US/docs/Web/API/Browser_API">Browser API</a>-specific</em></td>
   <td>Sent when the visibility state of the current browser iframe {{HTMLElement("iframe")}} changes, for example due to a call to {{DOMxRef("HTMLIFrameElement.setVisible","setVisible()")}}.</td>
  </tr>
  <tr>
   <td>{{Event("MozGamepadButtonDown")}}</td>
   <td></td>
   <td><em>To be specified</em></td>
   <td>A gamepad button is pressed down.</td>
  </tr>
  <tr>
   <td>{{Event("MozGamepadButtonUp")}}</td>
   <td></td>
   <td><em>To be specified</em></td>
   <td>A gamepad button is released.</td>
  </tr>
  <tr>
   <td>{{Event("MozMousePixelScroll")}} {{Deprecated_Inline}}</td>
   <td></td>
   <td><em>Mozilla specific</em></td>
   <td>The wheel button of a pointing device is rotated (detail attribute is a number of pixels). (use wheel instead)</td>
  </tr>
  <tr>
   <td>{{Event("MozOrientation")}} {{Deprecated_Inline}}</td>
   <td></td>
   <td><em>Mozilla specific</em></td>
   <td>Fresh data is available from an orientation sensor (see deviceorientation).</td>
  </tr>
  <tr>
   <td>{{Event("MozScrolledAreaChanged")}}</td>
   <td>{{DOMxRef("UIEvent")}}</td>
   <td><em>Mozilla specific</em></td>
   <td>The document view has been scrolled or resized.</td>
  </tr>
  <tr>
   <td>{{Event("moztimechange")}}</td>
   <td></td>
   <td><em>Mozilla specific</em></td>
   <td>The time of the device has been changed.</td>
  </tr>
  <tr>
   <td><a href="/en-US/DOM/Touch_events_(Mozilla_experimental)">MozTouchDown</a> {{Deprecated_Inline}}</td>
   <td></td>
   <td><em>Mozilla specific</em></td>
   <td>A touch point is placed on the touch surface (use touchstart instead).</td>
  </tr>
  <tr>
   <td><a href="/en-US/DOM/Touch_events_(Mozilla_experimental)">MozTouchMove</a> {{Deprecated_Inline}}</td>
   <td></td>
   <td><em>Mozilla specific</em></td>
   <td>A touch point is moved along the touch surface (use touchmove instead).</td>
  </tr>
  <tr>
   <td><a href="/en-US/DOM/Touch_events_(Mozilla_experimental)">MozTouchUp</a> {{Deprecated_Inline}}</td>
   <td></td>
   <td><em>Mozilla specific</em></td>
   <td>A touch point is removed from the touch surface (use touchend instead).</td>
  </tr>
  <tr>
   <td>{{Event("alerting")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>The correspondent is being alerted (his/her phone is ringing).</td>
  </tr>
  <tr>
   <td>{{Event("busy")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>The line of the correspondent is busy.</td>
  </tr>
  <tr>
   <td>{{Event("callschanged")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>A call has been added or removed from the list of current calls.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/DOM/onconnected">onconnected</a> {{Event("connected")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>A call has been connected.</td>
  </tr>
  <tr>
   <td>{{Event("connecting")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>A call is about to connect.</td>
  </tr>
  <tr>
   <td>{{Event("delivered")}}</td>
   <td>{{DOMxRef("SMSEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>An SMS has been successfully delivered.</td>
  </tr>
  <tr>
   <td>{{Event("dialing")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>The number of a correspondent has been dialed.</td>
  </tr>
  <tr>
   <td>{{Event("disabled")}}</td>
   <td></td>
   <td><a href="http://mxr.mozilla.org/mozilla-central/source/dom/wifi/nsIWifi.idl?rev=3e586802f478#182"><em>Firefox OS specific</em></a></td>
   <td>Wifi has been disabled on the device.</td>
  </tr>
  <tr>
   <td>{{Event("disconnected")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>A call has been disconnected.</td>
  </tr>
  <tr>
   <td>{{Event("disconnecting")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>A call is about to disconnect.</td>
  </tr>
  <tr>
   <td>{{Event("enabled")}}</td>
   <td></td>
   <td><a href="http://mxr.mozilla.org/mozilla-central/source/dom/wifi/nsIWifi.idl?rev=3e586802f478#182"><em>Firefox OS specific</em></a></td>
   <td>Wifi has been enabled on the device.</td>
  </tr>
  <tr>
   <td>{{Event("error_(Telephony)","error")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>An error occurred.</td>
  </tr>
  <tr>
   <td>{{Event("held")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>A call has been held.</td>
  </tr>
  <tr>
   <td>{{Event("holding")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>A call is about to be held.</td>
  </tr>
  <tr>
   <td>{{Event("incoming")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>A call is being received.</td>
  </tr>
  <tr>
   <td>{{Event("received")}}</td>
   <td>{{DOMxRef("SMSEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>An SMS has been received.</td>
  </tr>
  <tr>
   <td>{{Event("resuming")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>A call is about to resume.</td>
  </tr>
  <tr>
   <td>{{Event("sent")}}</td>
   <td>{{DOMxRef("SMSEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>An SMS has been sent.</td>
  </tr>
  <tr>
   <td>{{Event("statechange")}}</td>
   <td>{{DOMxRef("CallEvent")}}</td>
   <td><em>To be specified</em></td>
   <td>The state of a call has changed.</td>
  </tr>
  <tr>
   <td>{{Event("statuschange")}}</td>
   <td></td>
   <td><a href="http://mxr.mozilla.org/mozilla-central/source/dom/wifi/nsIWifi.idl?rev=3e586802f478#156"><em>Firefox OS specific</em></a></td>
   <td>The status of the Wifi connection changed.</td>
  </tr>
  <tr>
   <td>{{Event("overflow")}}</td>
   <td>{{DOMxRef("UIEvent")}}</td>
   <td><em>Mozilla specific</em></td>
   <td>An element has been overflowed by its content or has been rendered for the first time in this state (only works for elements styled with <code>overflow</code> != <code>visible</code>).</td>
  </tr>
  <tr>
   <td>{{Event("smartcard-insert")}}</td>
   <td></td>
   <td><em>Mozilla specific</em></td>
   <td>A <a href="/en-US/docs/JavaScript_crypto">smartcard</a> has been inserted.</td>
  </tr>
  <tr>
   <td>{{Event("smartcard-remove")}}</td>
   <td></td>
   <td><em>Mozilla specific</em></td>
   <td>A <a href="/en-US/docs/JavaScript_crypto">smartcard</a> has been removed.</td>
  </tr>
  <tr>
   <td>{{Event("stkcommand")}}</td>
   <td></td>
   <td><em>Firefox OS specific</em></td>
   <td>The <abbr title="SIM Application Toolkit">STK</abbr> Proactive Command is issued from <abbr title="Integrated Circuit Card">ICC</abbr>.</td>
  </tr>
  <tr>
   <td>{{Event("stksessionend")}}</td>
   <td></td>
   <td><em>Firefox OS specific</em></td>
   <td>The <abbr title="SIM Application Toolkit">STK</abbr> Session is terminated by <abbr title="Integrated Circuit Card">ICC</abbr>.</td>
  </tr>
  <tr>
   <td><code>text</code></td>
   <td></td>
   <td><em>Mozilla Specific</em></td>
   <td>A generic composition event occurred.</td>
  </tr>
  <tr>
   <td>{{Event("touchenter")}}</td>
   <td>{{DOMxRef("TouchEvent")}}</td>
   <td><a href="http://www.w3.org/TR/touch-events/#the-touchstart---------event">Touch Events</a> Removed</td>
   <td></td>
  </tr>
  <tr>
   <td>{{Event("touchleave")}}</td>
   <td>{{DOMxRef("TouchEvent")}}</td>
   <td><a href="http://www.w3.org/TR/touch-events/#the-touchstart---------event">Touch Events</a> Removed</td>
   <td></td>
  </tr>
  <tr>
   <td>{{Event("underflow")}}</td>
   <td>{{DOMxRef("UIEvent")}}</td>
   <td><em>Mozilla specific</em></td>
   <td>An element is no longer overflowed by its content (only works for elements styled with <code>overflow</code> != <code>visible</code>).</td>
  </tr>
  <tr>
   <td><code>uploadprogress</code> {{Deprecated_Inline}}</td>
   <td>{{DOMxRef("ProgressEvent")}}</td>
   <td><em>Mozilla Specific</em></td>
   <td>Upload is in progress (see {{Event("progress")}}).</td>
  </tr>
  <tr>
   <td>
    <p>{{Event("ussdreceived")}}</p>
   </td>
   <td></td>
   <td><em>Firefox OS specific</em></td>
   <td>A new <abbr title="Unstructured Supplementary Service Data">USSD</abbr> message is received</td>
  </tr>
  <tr>
   <td>{{Event("voicechange")}}</td>
   <td></td>
   <td><em>Firefox OS specific</em></td>
   <td>The {{DOMxRef("MozMobileConnection.voice")}} object changes values.</td>
  </tr>
  <tr>
   <td>{{Event("msContentZoom")}}</td>
   <td></td>
   <td><em>Microsoft specific</em></td>
   <td></td>
  </tr>
  <tr>
   <td>{{Event("MSManipulationStateChanged")}}</td>
   <td></td>
   <td><em>Microsoft specific</em></td>
   <td></td>
  </tr>
  <tr>
   <td>{{Event("MSPointerHover")}} {{Deprecated_Inline}}</td>
   <td></td>
   <td><em>Microsoft specific</em></td>
   <td></td>
  </tr>
 </tbody>
</table>
</div>

<h2 id="Mozilla-specific_events">Mozilla-specific events</h2>

<div class="note">
<p><strong>Note:</strong> those events are never exposed to web content and can only be used in chrome content context.</p>
</div>

<h3 id="XUL_events">XUL events</h3>

<div style="overflow: auto;">
<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">Event Name</th>
   <th scope="col">Event Type</th>
   <th scope="col">Specification</th>
   <th scope="col">Fired when...</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{Event("broadcast")}}</td>
   <td></td>
   <td><a href="/en-US/docs/XUL/Tutorial/Broadcasters_and_Observers#Broadcast_event">XUL</a></td>
   <td>An <code>observer</code> noticed a change to the attributes of a watched broadcaster.</td>
  </tr>
  <tr>
   <td>{{Event("CheckboxStateChange")}}</td>
   <td></td>
   <td>XUL</td>
   <td>The state of a <code>checkbox</code> has been changed either by a user action or by a script (useful for accessibility).</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/close_event">close</a></td>
   <td></td>
   <td>XUL</td>
   <td>The close button of the window has been clicked.</td>
  </tr>
  <tr>
   <td>{{Event("command")}}</td>
   <td></td>
   <td>XUL</td>
   <td>An element has been activated.</td>
  </tr>
  <tr>
   <td>{{Event("commandupdate")}}</td>
   <td></td>
   <td>XUL</td>
   <td>A command update occurred on a <code>commandset</code> element.</td>
  </tr>
  <tr>
   <td>{{Event("DOMMenuItemActive")}}</td>
   <td></td>
   <td>XUL</td>
   <td>A menu or menuitem has been hovered or highlighted.</td>
  </tr>
  <tr>
   <td>{{Event("DOMMenuItemInactive")}}</td>
   <td></td>
   <td><em>XUL</em></td>
   <td>A menu or menuitem is no longer hovered or highlighted.</td>
  </tr>
  <tr>
   <td>{{Event("popuphidden")}}</td>
   <td><code>PopupEvent</code></td>
   <td><a href="/en-US/docs/XUL/PopupGuide/PopupEvents"><em>XUL</em></a></td>
   <td>A menupopup, panel or tooltip has been hidden.</td>
  </tr>
  <tr>
   <td>{{Event("popuphiding")}}</td>
   <td><code>PopupEvent</code></td>
   <td><a href="/en-US/docs/XUL/PopupGuide/PopupEvents"><em>XUL</em></a></td>
   <td>A menupopup, panel or tooltip is about to be hidden.</td>
  </tr>
  <tr>
   <td>{{Event("popupshowing")}}</td>
   <td><code>PopupEvent</code></td>
   <td><a href="/en-US/docs/XUL/PopupGuide/PopupEvents"><em>XUL</em></a></td>
   <td>A menupopup, panel or tooltip is about to become visible.</td>
  </tr>
  <tr>
   <td>{{Event("popupshown")}}</td>
   <td><code>PopupEvent</code></td>
   <td><a href="/en-US/docs/XUL/PopupGuide/PopupEvents"><em>XUL</em></a></td>
   <td>A menupopup, panel or tooltip has become visible.</td>
  </tr>
  <tr>
   <td>{{Event("RadioStateChange")}}</td>
   <td></td>
   <td>XUL</td>
   <td>The state of a <code>radio</code> has been changed either by a user action or by a script (useful for accessibility).</td>
  </tr>
  <tr>
   <td>{{Event("ValueChange")}}</td>
   <td></td>
   <td>XUL</td>
   <td>The value of an element has changed (a progress bar for example, useful for accessibility).</td>
  </tr>
 </tbody>
</table>
</div>

<h3 id="Add-on-specific_events">Add-on-specific events</h3>

<div style="overflow: auto;">
<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">Event Name</th>
   <th scope="col">Event Type</th>
   <th scope="col">Specification</th>
   <th scope="col">Fired when...</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozSwipeGesture">MozSwipeGesture</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A touch point is swiped across the touch surface</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozMagnifyGestureStart">MozMagnifyGestureStart</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>Two touch points start to move away from each other.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozMagnifyGestureUpdate">MozMagnifyGestureUpdate</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>Two touch points move away from each other (after a MozMagnifyGestureStart).</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozMagnifyGesture">MozMagnifyGesture</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>Two touch points moved away from each other (after a sequence of MozMagnifyGestureUpdate).</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozRotateGestureStart">MozRotateGestureStart</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>Two touch points start to rotate around a point.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozRotateGestureUpdate">MozRotateGestureUpdate</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>Two touch points rotate around a point (after a MozRotateGestureStart).</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozRotateGesture">MozRotateGesture</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>Two touch points rotate around a point (after a sequence of MozRotateGestureUpdate).</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozTapGesture">MozTapGesture</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>Two touch points are tapped on the touch surface.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozPressTapGesture">MozPressTapGesture</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A "press-tap" gesture happened on the touch surface (first finger down, second finger down, second finger up, first finger up).</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozEdgeUIGesture">MozEdgeUIGesture</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A touch point is swiped across the touch surface to invoke the edge UI (Win8 only).</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozAfterPaint">MozAfterPaint</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>Content has been repainted.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/DOMPopupBlocked">DOMPopupBlocked</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A popup has been blocked</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/DOMWindowCreated">DOMWindowCreated</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A window has been created.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/DOMWindowClose">DOMWindowClose</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A window is about to be closed.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/DOMTitleChanged">DOMTitleChanged</a></td>
   <td></td>
   <td><em>Addons specifc</em></td>
   <td>The title of a window has changed.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/DOMLinkAdded">DOMLinkAdded</a></td>
   <td></td>
   <td><em>Addons specifc</em></td>
   <td>A link has been added a document.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/DOMLinkRemoved">DOMLinkRemoved</a></td>
   <td></td>
   <td><em>Addons specifc</em></td>
   <td>A link has been removed inside from a document.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/DOMMetaAdded">DOMMetaAdded</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A <code>meta</code> element has been added to a document.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/DOMMetaRemoved">DOMMetaRemoved</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A <code>meta</code> element has been removed from a document.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/DOMWillOpenModalDialog">DOMWillOpenModalDialog</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A modal dialog is about to open.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/DOMModalDialogClosed">DOMModalDialogClosed</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A modal dialog has been closed.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/DOMAutoComplete">DOMAutoComplete</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>The content of an element has been auto-completed.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/DOMFrameContentLoaded">DOMFrameContentLoaded</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>The frame has finished loading (but not its dependent resources).</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/AlertActive">AlertActive</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A <code><a href="/en-US/docs/XUL/notification">notification</a></code> element is shown.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/AlertClose">AlertClose</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A <code><a href="/en-US/docs/XUL/notification">notification</a></code> element is closed.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/fullscreen">fullscreen</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>Browser fullscreen mode has been entered or left.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/sizemodechange">sizemodechange</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>Window has entered/left fullscreen mode, or has been minimized/unminimized.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/MozEnteredDomFullscreen">MozEnteredDomFullscreen</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td><a href="/en-US/docs/DOM/Using_full-screen_mode">DOM fullscreen</a> mode has been entered.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/SSWindowClosing">SSWindowClosing</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>The session store will stop tracking this window.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/SSTabClosing">SSTabClosing</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>The session store will stop tracking this tab.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/SSTabRestoring">SSTabRestoring</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A tab is about to be restored.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/SSTabRestored">SSTabRestored</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A tab has been restored.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/SSWindowStateReady">SSWindowStateReady</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A window state has switched to "ready".</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/SSWindowStateBusy">SSWindowStateBusy</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A window state has switched to "busy".</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/TabOpen">TabOpen</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A tab has been opened.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/TabClose">TabClose</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A tab has been closed.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/TabSelect">TabSelect</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A tab has been selected.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/TabShow">TabShow</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A tab has been shown.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/TabHide">TabHide</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A tab has been hidden.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/TabPinned">TabPinned</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A tab has been pinned.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/TabUnpinned">TabUnpinned</a></td>
   <td></td>
   <td><em>Addons specific</em></td>
   <td>A tab has been unpinned.</td>
  </tr>
 </tbody>
</table>
</div>

<h3 id="Developer_tool-specific_events">Developer tool-specific events</h3>

<div style="overflow: auto;">
<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">Event Name</th>
   <th scope="col">Event Type</th>
   <th scope="col">Specification</th>
   <th scope="col">Fired when...</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/CssRuleViewRefreshed">CssRuleViewRefreshed</a></td>
   <td></td>
   <td><em>devtools specific</em></td>
   <td>The "Rules" view of the style inspector has been updated.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/CssRuleViewChanged">CssRuleViewChanged</a></td>
   <td></td>
   <td><em>devtools specific</em></td>
   <td>The "Rules" view of the style inspector has been changed.</td>
  </tr>
  <tr>
   <td><a href="/en-US/docs/Web/Reference/Events/CssRuleViewCSSLinkClicked">CssRuleViewCSSLinkClicked</a></td>
   <td></td>
   <td><em>devtools specific</em></td>
   <td>A link to a CSS file has been clicked in the "Rules" view of the style inspector.</td>
  </tr>
 </tbody>
</table>
</div>

<h2 id="See_also">See also</h2>

<ul>
 <li>{{DOMxRef("Event")}}</li>
 <li><a href="/en-US/docs/Web/Guide/DOM/Events">Event developer guide</a></li>
</ul>