# HTTP 란?

http는 서버와 클라이언트가 인터넷 상에서 데이터를 주고받기 위한 프로토콜(protocol)이다.
http는 어떤 종류의 데이터도 전송할 수 있도록 설계되어 있다.

## HTTP 작동 방식

http는 서버/클라이언트 모델을 따르기 때문에
클라이언트가 서버에 요청을 보내면 서버는 클라이언트에 응답한다.

http는 stateless (무상태) 방식을 따른다.
이 떄 stateless(무상태) 방식이란 서버가 여러 클라이언트들을 구별할 수 없다는 것이다.

## 리퀘스트 메소드

- `GET` : URI로 지정한 정보를 도출한다. 파일의 경우 해당 파일의 내용을 되돌려 보내며 CHI 프로그램의 경우에는 해당 프로그램의 출력 데이터를 그대로 반송한다.
- `POST` : 폼에 입력한 데이터를 송신하는 경우에 사용하는 것으로, 클라이언트에서 서버로 데이터를 송신한다.
- `HEAD` : `GET`과 비슷하지만, HTTP 메시지의 헤어만 반송하고 데이터 내용은 돌려보내지 않는다. 파일 최종 갱신 일시와 같은 속성 정보를 조사할 때 사용한다.
- `OPTION` : 통신 옵션을 조사할 때 사용한다.
- `DELETE` : URI로 지정한 서버의 파일을 삭제한다.

## HTTP Status Code

- `1xx` : Information responses
- `2xx` : Successful responses
- `3xx` : Redirection messages
- `4xx` : Client error responses
- `5xx` : Server error responses