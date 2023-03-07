# 인터넷은 어떻게 작동될까요?
--------------------------------------------
## 인터넷

### 전세계의 컴퓨터가 연결된 _네트워크_, 즉 _컴퓨터 통신망_. 컴퓨터들은 TCP/IP 통신 프로토콜을 이용해 정보를 주고받는다.
### TCP/IP

#### TCP/IP는 인터넷 네트워크의 대표적인 표준 프로토콜이다.   
- 프로토콜 : 컴퓨터 간의 정보를 원활하게 교환하기 위해 만들어진 규칙의 집합.
--------------------------------------------
## 네트워크

### 통신망. 컴퓨터가 연결되어 정보를 주고 받는 경로.
--------------------------------------------
## 네트워크의 종류

> ### PAN ( Personal Area Network ) : 가장 작은 규모의 네트워크
> > ### LAN ( Local Area Network ) : 근거리 영역 네트워크
> > > ### MAN (Metropolitan Area Network) : 대도시 영역 네트워크
> > > > ### WAN (Wide Ares Network) : 광대역 네트워크
> > > > >  ### 여러 종류의 정보서비스가 부가된 부가가치 통신망.
> > > > > >### ISDN (Integrated Services Digital Network) : 종합정보 통신망, 통합서비스 디지털 통신망.   
--------------------------------------------
## 네트워크 - **라우터, 모뎀**
### 연결할 컴퓨터가 많아 질수록, 네트워크의 규모가 커지고 복잡해진다.
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FzU56d%2Fbtq4wuDRaCR%2FWAYXa1vUczZ8j9nfbuI9c1%2Fimg.png" width="450px" height="450px" title="px(픽셀) 크기 설정" alt="네트워크1"></img><br/>

### 위 사진을 보면 알 수 있듯 컴퓨터가 많아지면 연결할 케이블의 개수도 늘어난다. 컴퓨터가 더 많아지면 연결해야 하는 케이블 수도 더 늘어날 것이고, 더 복잡해질 것이다.   

### >_so_ 이러한 문제를 해결하기 위해 네트워크의 각 컴퓨터는 _라우터_ 라고하는 특수한 소형 컴퓨터에 연결된다. _라우터_ 는 각 _컴퓨터 간의 메시지를 받고 전달하는 역할_ 을 한다.   
---------------------------------------------
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FP66vP%2Fbtq4wt56tLJ%2FDbQLIW3l8G35GU0eBprAs1%2Fimg.png" width="450px" height="450px" title="px(픽셀) 크기 설정" alt="네트워크2"></img><br/>

### 그렇다면 _라우터_ 끼리 연결 하게 되면 어떤 일이 발생할까?   
> 위와 같이 어떤 라우터가 연결하는 컴퓨터들이, 다른 _라우터_ 가 연결하는 컴퓨터들에도 연결을 할 수 있게 된다.
연결 할 수 있는 컴퓨터 수에 있어서 확장이 가능하다는 소리이다.   
### _그러나_, 아주 먼 지역(ex)다른 나라)에 있는 컴퓨터와 내 컴퓨터를 케이블로 연결 하는 것은 상식적으로 할 수 없는 일이기 때문에, 또 _문제점_ 이 생긴다.
 
>_so_ 거리가 먼 지역의 네트워크 연결 문제를 해결하기 위해, _모뎀_ 이라는 특수 장비를 연결한다.
### _모뎀_ 은 네트워크의 정보를 전 세계에 연결된 전화 기반의 시설에서 처리하는 장비이다.
----------------------------------------------
## 네트워크 - **ISP** 
### _ISP_ 는 _인터넷 서비스 제공 업체(Internet Service Provider)_ 의 약자이다. 네트워크를 ISP에 연결하면, ISP는 연결되는 라우터들을 관리하고, 다른 ISP들의 라우터에도 접근이 가능하게 해준다. 쉽게 말해서, 네트워크끼리 소통이 가능하게 해주고, 관리해주는 역할이다.

### 아래는 그렇게 만들어진 **전체 네트워크 인프라** 이다.   

![Alt text](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-7.png "네트워크3")

-----------------------------------------------------
