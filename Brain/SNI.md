Server Name Indication의 약자로 서버의 이름을 표시한다.
IP 주소와 도메인이 1:1로 대응되면 IP 주소에 따라 인증서를 발급하면 되지만 하나의 IP 주소에 여러 도메인이 존재한다면 IP 주소만으로 TLS 연결을 할 수 없다. 그래서 IP 주소의 어떤 도메인과 TLS 연결을 맺을지 명시하는 것이다.
## ESNI
TLS Handshake의 Client Hello 패킷에 SNI를 전송하는데 이를 암호화하지 않아 클라이언트가 접속하고자 하는 도메인이 스누핑으로 노출될 수 있다. 이 부분을 암호화 하여 클라이언트가 어떤 인증서를 요청하는지 알 수 없게 하는 방법이다.
## 참고
https://www.cloudflare.com/ko-kr/learning/ssl/what-is-sni/

#network #security 