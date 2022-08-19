3주차

확실히 Sping 보단 SpringBoot가 설정하기 편한것 같습니다. 다만 DAO와 DTO, Config등이 어떤 일을 하는 패키지들인지 이해하지 못해 찾아보았습니다. 또한 mybastis를 연결한 이후엔 실행 자체가 되지 않아 혼란이 왔습니다.

Description: Field uMapper in com.example.SpringTest.service.StatisticServiceImpl required a bean of type 'com.example.SpringTest.dao.StatisticMapper' that could not be found.

The injection point has the following annotations: - @org.springframework.beans.factory.annotation.Autowired(required=true)

Action: Consider defining a bean of type 'com.example.SpringTest.dao.StatisticMapper' in your configuration.

이런 에러가 나왔는데 모든 패키지와 java파일들이 있는데 왜 찾지 못하는지 이해하지 못했습니다. 오타 또한 없어서 찾아보았는데 메인 클래스에

@SpringBootApplication(scanBasePackages = {"com.example.SpringTest.dao.StatisticMapper"})

이것을 넣으니 해결 되었습니다.

다만

Whitelabel Error Page This application has no explicit mapping for /error, so you are seeing this as a fallback.

Thu Aug 11 17:34:08 KST 2022 There was an unexpected error (type=Not Found, status=404). No message available

이 에러가 나타나서 해결 중입니다.

검색해본 결과 html파일 없어서 그렇다, controller 패키지가 없어서 그렇다는 이야기가 있어 해보았는데 여전히 해결되지 않았습니다.


4주차

원래는 API를 개발해야하는데 아직 환경 설정을 완성하지 못해 진행하지 못했습니다.
처음에는 그냥 404에러가 나서 검색해보니 
@SpringBootApplication(scanBasePackages = {"com.example.SpringTest.dao.StatisticMapper"})
이걸 넣으면 된다 해서 넣었는데 이후에는 Whitelable이 나와서 어찌해야할지 모르겠습니다.
인터넷에 나와있는 부분은 대부분 비슷하고 따라도 해보았는데 전혀 효과가 없었습니다.

또한 mybastis가 없다는 이야기도 나왔는데 설정을 했는데 없다고 해서 검색해서 pom.xml에 해당 내용을 다시 추가한 적이 있는데 이 또한 방법은 아니었습니다.

Several ports (8005, 8080) required by Tomcat v9.0 Server at localhost are already in use. The server may already be running in another process, or a system process may be using the port. To start this server you will need to stop the other process or change the port number(s).
이 에러 메세지도 많이 나왔었는데 이건 CMD에 들어가서 포트 번호를 검색한후 프로세스를 종료했더니 되었습니다.

어떠한 문제인진 모르겠는데 서버에서 해당 파일을 찾지 못하는 문제도 있습니다. 저는 넣었는데 말이죠..
