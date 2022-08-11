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
