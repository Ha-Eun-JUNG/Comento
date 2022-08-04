//1주차

<이클립스, 스프링>

JDK랑 이클립스는 이미 설치가 되어있는 상태여서 넘어갔습니다.
다만 스프링을 설치하는 과정에서

Cannot complete the provisioning operation.  Please change your selection and try again. See below for details.

Cannot complete the install because one or more required items could not be found.
  Software being installed: Spring IDE Integration, Flex and Web Services Extension (optional) 3.9.22.202204280911-RELEASE (org.springframework.ide.eclipse.integration.feature.feature.group 3.9.22.202204280911-RELEASE)
  Missing requirement: Spring IDE Configuration Graphical Editing 3.9.22.202204280911-RELEASE (org.springframework.ide.eclipse.config.graph 3.9.22.202204280911-RELEASE) requires 'osgi.bundle; org.eclipse.mylyn.commons.ui [3.7.0,4.0.0)' but it could not be found
  Cannot satisfy dependency:
    From: Spring IDE Core (required) 3.9.22.202204280911-RELEASE (org.springframework.ide.eclipse.feature.feature.group 3.9.22.202204280911-RELEASE)
    To: org.eclipse.equinox.p2.iu; org.springframework.ide.eclipse.config.graph [3.9.22.202204280911-RELEASE,3.9.22.202204280911-RELEASE]
  Cannot satisfy dependency:
    From: Spring IDE Integration, Flex and Web Services Extension (optional) 3.9.22.202204280911-RELEASE (org.springframework.ide.eclipse.integration.feature.feature.group 3.9.22.202204280911-RELEASE)
    To: org.eclipse.equinox.p2.iu; org.springframework.ide.eclipse.feature.feature.group 0.0.0
    
하나 이상의 필수 항목을 찾을 수 없기 때문에 설치를 완료할 수 없습니다.
  설치 중인 소프트웨어: Spring IDE 통합, Flex 및 웹 서비스 확장(선택 사항) 3.9.22.202204280911-RELEASE(org.springframework.ide.eclipse.integration.feature.feature.group 3.9.22.202204280911-RELEASE)
  누락된 요구 사항: Spring IDE 구성 그래픽 편집 3.9.22.202204280911-RELEASE(org.springframework.ide.eclipse.config.graph 3.9.22.202204280911-RELEASE)에는 'osgi.bundle; org.eclipse.mylyn.commons.ui [3.7.0,4.0.0)' 하지만 찾을 수 없습니다.
  종속성을 충족할 수 없음:
    보낸 사람: Spring IDE 코어(필수) 3.9.22.202204280911-RELEASE(org.springframework.ide.eclipse.feature.feature.group 3.9.22.202204280911-RELEASE)
    받는 사람: org.eclipse.equinox.p2.iu; org.springframework.ide.eclipse.config.graph [3.9.22.202204280911-RELEASE,3.9.22.202204280911-RELEASE]
  종속성을 충족할 수 없음:
    보낸 사람: Spring IDE 통합, Flex 및 웹 서비스 확장(선택 사항) 3.9.22.202204280911-RELEASE(org.springframework.ide.eclipse.integration.feature.feature.group 3.9.22.202204280911-RELEASE)
    받는 사람: org.eclipse.equinox.p2.iu; org.springframework.ide.eclipse.feature.feature.group 0.0.0

라는 에러가 떠서 확인해보니 이클립스 버전이 너무 최신이어서 그랬던것 같아 본래 설치되어있던 이클립스를 삭제하고 낮은 버전의 이클립스로 설치를 하였더니 해결되었습니다.
설치 후 한글이 깨지는 현상이 나타나 해결하였습니다.


<톰캣>
(작성했던 글이 삭제 되어 기억이 없습니다..ㅜ)
설치하는데 문제는 없었던것으로 기억합니다

<Hello World 출력>
Hello World를 출력하는데에 있어서 URL을 어떻게 해야하는지 몰라 조금 해맸습니다.
Project 이름은 SpringTest인데 Package 이름은 settingweb이어서 둘다 작성해보았습니다.
다음부턴 같게 해야할것 같습니다.

<MariaDB, MySQL WorkBench 설치>
각각 설치하는데 문제는 발생하지 않았습니다.
다만 INSERT하는 과정에서 오타가 발생해 에러가 났는데 오타 확인 잘 해야할것 같습니다.
또한 SELECT할때 INSERT 밑에 작성했는데 에러가 나서 아예 삭제하고 다시 작성했더니 됐습니다.
사소한 에러를 발생 시킨것 같습니다.

<스프링, MySQL, MYBastis 연동>
이게 가장 문제였습니다.
1번은 잘 따라갔는데 2번에서 막혔습니다

xmlns가 문제라고 해서 검색해서

변경했는데
에러는 뜨지 않는데 3번 파일이 안 만들어져 막혔습니다.
