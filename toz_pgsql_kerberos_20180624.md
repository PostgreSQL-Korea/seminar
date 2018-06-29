# 2018.06.24 토즈 대학로점 세미나

## Kerberos 세미나

### Kerberos 통신구조
![Kerberos 통신구조](kerberos_structure.gif)

### Kerbeos 용어 설명
* Principal: Kerberos에 접속하는 사용자, 컴퓨터, 서비스를 공급하는 서비스 서버들을 가리키며 자격증명이라고 부르기도 한다. Kerberos Principal이 공식 용어이다.
* Instance: 서비스 Principal 및 Special Principal를 가리킨다.
* Realm: 커베로스 설치 시 제공하는 유일한 Realm 제어 호스트 또는 사용자가 속한 도메인 또는 그룹이며, 일반적으로 대문자인 도메인을 사용하며 도메인은 DNS서버에서 찾을 수 있어야 한다.
* KDC: KDC(Key Distribution Center)는 3부분으로 구성된다. 첫번째는 모든 Principal의 데이터베이스, 두번째는 인증서버, 세번째는 티켓 부여 서버다. 각 Realm에는 하나의 KDC가 있어야 한다.
* TGT: TGT(Ticket Granting Ticket) AS(인증서버. Authenticate Server)에서 발행한 TGT는 User와 KDC에만 알려진 User 비밀번호로 암호화된다.
* TGS: 요청시 고객에게 서비스 티켓을 발급한다.
* 티켓: 두 사람의 신원을 확인할 때 사용하며 1개의 Princiapl은 사용자이고 다른 Principal은 사용자가 요청한 Service이다. 티켓은 인증된 세션 동안 보안 통신에 사용하는 암호화 키를 설정한다.
* 키탭: KDC의 주 데이터베이스를 덤프한 파일이며, 서비스 또는 호스트의 암호화 키를 포함한다.

### 커베로스 구성
커베로스는...
