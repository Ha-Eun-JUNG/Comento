1주차

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

(07.25)
<톰캣>


