http는 무엇일까요?
=================
**HTTP (Hyper Text Transfer Protocol)**, 하이퍼텍스트 전송 프로토콜
------------------------------------------
### 서버와 클라이언트(사용자)가 서로 데이터를 주고받기 위해 사용되는 프로토콜(통신 규약)
### 1989년 Tim Berners Lee(팀 버너스리)가 처음 설계,<br> 초기 단계에서 발전을 거듭해 현재는 HTML 문서와 같은 정보들을 가져오는 데 사용.
### 월드 와이드 웹(World-Wide Web 일명 : www) 기반에서<br>전 세계적으로 정보 공유를 하는데 큰 역할을 했다.<br>인터넷 주소를 지정할때 http://www.--와 같이 시작하는 것은    www.--이라는 인터넷 주소가 가진 데이터 정보 등의 교환을 http의 통신 규약대로 처리하라는 것을 의미한다.
### 사용자가 브라우저를 통해(클라이언트) 어떤 서비스를 요청(request)시, 서버에서는 해당 요청사항에 맞는 결과를 찾아서 사용자에게 응답(response)한다.
![Alt text](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FOuorH%2FbtrmRu6tol9%2Fb6TfAxPy5Z2KK83dDs3Bs1%2Fimg.png "client-server")
-----------------------------------------------------
HTTP의 특징
--------------
### 1.*클라이언트-서버* 모델을 따른다.
### 2.기본적으로 TCP/IP를 이용하는 응용 프로토콜. 사용 포트 번호는 기본적으로 80. -TCP/IP는 인터넷 네트워크의 대표적인 표준 프로토콜.
### 3.비연결형 지향 : 클라이언트가 서버에게 리소스를 요청한 후 응답을 받으면 연결을 끊는다. 이 특징을 보완하기 위해 Cookie와 같은 기술이 등장. (무상태, Stateless라고 부름)
### 4.무상태성: 각각의 요청은 독립적이다.---------------------------------------------------- 
클라이언트-서버 모델
-------------------   
 ## 클라이언트 -----메시지-----> 서버를 요청 (request)이라고 하며,<br> 서버 -----메시지-----> 클라이언트를 응답(responses)라고 부른다.   


> ## *클라이언트(사용자 에이전트)* :
 ### 사용자를 대신하여 동작하는 모든 도구.<br> 브라우저(웹 정보를 화면에 표시해 주는 응용프로그램 ex 크롬 익스플로러)는 항상 클라이언트의 역할을 한다.<br>   브라우저는 절대로 서버가 될 수 없다.<br> 웹페이지를 예로 들면, 브라우저는 페이지에 나타날 HTML 문서를 요청한다 >> 스크립트/이미지/비디오/CSS 등등을 가져온다 >> 이 리소스들을 혼합해 웹페이지에 표시한다.
> ## *서버(웹서버)* :
 ### 통신 채널 반대편에는 클라이언트의 요청을 받아 이 요청에 대한 정보를 제공하는 서버가 존재. 요청에 대한 답이 HTTP 메시지(HTTP message). 

### 또 이 요청과 응답 사이에는 여러 개체들이 있는데, 그 중 프록시는 게이트웨이 또는 캐시 역할을 한다.


> ## 프록시 :
 ### 웹브라우저와 서버 사이에 수많은 HTTP 메시지들이 왔다갔다 함. 애플리케이션 계층에서 동작하는 것들을 일반적으로 프록시라고 말한다. 프록시는 눈에 보이거나 그렇지 않을 수도 있으며 다양한 기능들을 수행한다.
 * ### 캐싱 (HTTP로 문서 캐시되는 방식 제어.)

 * ### 필터링 (바이러스 백신 스캔, 유해 컨텐츠 차단 기능)

 * ### 로드 밸런싱 (여러 서버들이 서로 다른 요청을 처리하도록 허용)

 * ### 인증 (다양한 리소스에 대한 접근 제어.)

 * ### 로깅 (이력 정보를 저장)
-----------------------------------------------
HTTP 메시지
-----------
* ### 크롬에서 오른쪽 마우스를 눌러 검사(Ctrl+Shift+C)로 들어간뒤 Network로 들어가면 해당 페이지의 HTTP 메시지 정보를 확인할 수 있다. 

## *HTTP 메시지*는 요청 메시지(Request message)와 응답 메시지(Response message)로 분류된다. (클라이언트에서 온 메시지/서버에서 온 메시지의 차이)

![Alt text](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FVHNV8%2FbtqDn0wi4jm%2F34tZOYkLKDBBaLhcKGvpQK%2Fimg.png)

![Alt text](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FpqNm0%2FbtqDn2AB40b%2F54ILC6POhg9KKth15ovIM0%2Fimg.png)

## *General* 은 메시지에 대한 일반적인 정보를 제공한다. (요청/응답 전체에 적용)
 * ### *Request Method* :  클라이언트가 수행하고자 하는 동작 정의 (GET, POST, PUT, DELETE, OPTIONS, HEAD). 일반적으로 GET(클라이언트가 리소스를 가져옴)이나 POST(HTML 폼의 데이터를 전송)를 사용함.

 * ### Statue Code : 200 정상

## *Response Headers*는 *response message*만 취급.

 * ### date : 메시지 작성 일자
 * ### cache-control : 캐시 사용 제어. (no-cache:캐시 쌓지 않는다 / max-age=seconds:seconds값보다 오래된 응답은 보내지 않는다 / public : 어떤 캐시든 쌓는다 등등)
 * ### content-type : 응답되는 컨텐츠의 유형
 * ### content-length : 응답되는 컨텐츠의 길이
 * ### last-modified : 응답되는 컨텐츠가 마지막으로 수정된 일시
 * ### server : HTTP 서버의 정보

## *Request Headers*는 *request message*만 취급.

 * ### authority : 도메인 이름 및 옵션 포트로 이뤄진 URL. (옵션 포트 앞에는 ':'가 붙는다)
 * ### accept-language : 클라이언트가 요청하는 언어
 * ### user-agent : 클라이언트 프로그램 (웹 브라우저)을 표시함.

#### 참고 사이트
 - <https://is-this-it.tistory.com/41>
 - <https://bomango.tistory.com/5>