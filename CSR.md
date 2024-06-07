Certificate Signing Request(인증서 서명 요청)의 약자로, [[인증서]]를 발급받기 위해 필요한 정보를 담고 있는 인증서 신청 형식 데이터이다.
## CSR에 포함된 정보
### 도메인 정보 
| 이름                                                                                      | 설명                                                                                                                                                                                                                           |
| --------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Common Name (CN)<br><br>(e.g. *.example.com  <br>www.example.com  <br>mail.example.com) | The fully qualified domain name (FQDN) of your server.                                                                                                                                                                       |
| Organization (O)                                                                        | The legal name of your organization. Do not abbreviate and include any suffixes, such as Inc., Corp., or LLC.<br><br>For EV and OV SSL Certificates, this information is verified by the CA and included in the certificate. |
| Organizational Unit (OU)                                                                | The division of your organization handling the certificate.                                                                                                                                                                  |
| City/Locality (L)                                                                       | The city where your organization is located. This shouldn’t be abbreviated.                                                                                                                                                  |
| State/County/Region (S)                                                                 | The state/region where your organization is located. This shouldn't be abbreviated.                                                                                                                                          |
| Country (C)                                                                             | Two-letter country code where organization is located.                                                                                                                                                                       |
| Email Address                                                                           | Email address used to contact your organization.                                                                                                                                                                             |
### 공개키
서버에서 생성한 개인키-공개키 쌍 중 공개키를 포함해야 한다.
### 키 타입과 길이
일반적인 키 길이는 RSA 2048이지만 몇몇 CA에서는 더 큰 키 길이(RSA 4096+)나 ECC 키를 지원한다.
## 참고
https://www.globalsign.com/en/blog/what-is-a-certificate-signing-request-csr

#network #security 