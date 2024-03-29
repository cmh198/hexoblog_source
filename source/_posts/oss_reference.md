---
title: oss_reference
date: 2021-12-22 03:12:54
tags: oss
---

# 오픈소스 기말고사 cheat sheet

### VIM cheat sheet
[링크](https://vim.rtorr.com/lang/ko)

### 1. link, symbolic link 관련 문제
        - 중간고사에서 변형 문제
        - ln -s 
---
### 2. 어떤 명령을 수행하는 실행파일을 만듬 + permission 변경
        1. vi 편집기로 새 파일을 생성합니다.
	    2. 새 파일 내용 최 상단에 #!/bin/bash 라인을 추가합니다.
	    3. 원하는 명령어를 추가해줍니다.
	    4. 실행권한 부여하기 (chmod 777 test.sh)
        5. 실행 ./~.sh

---
### 3. bash 스크립트 -> loop를 사용해서 수식 계산
![수식처리법](/images/bashshell.png)

[참고 링크](https://zetawiki.com/wiki/Bash_%EC%88%AB%EC%9E%90_%EA%B3%84%EC%82%B0)
---
### 4.주요한 오픈소스 라이선스 2개 선택해서 이것과 이것 차이점~ 
        - 표 옆에 놓고 보고 쓰면됨
![오픈소스 라이선스 표](/images/license.png)

![라이센스 트리](/images/Licensetree.png)
### 5.오픈소스 써서 비즈니스를 하는 방법 설명 
	- 커뮤니티 버전으로 소스를 먼저 공개한 뒤 기술지원같은 추가적인 서비스는 유료 버전으로 따로 서비스를 두어 운영한다.
    - 무료 + 유료 결합 모델은 일단 제품을 무료로 다운로드 가능하게 하고 별도로 'PRO' UPGRADE 버전을 만들어 놓는다.
    제품의 핵심부분은 무료로 제공하면서, 다양한 애드온 기능을 프로 버전에서 제공한다.
    마치 모바일 앱이 설치는 무료지만 인앱 결제를 통해 수익을 창출하는 것과 같다.
    최근에 이러한 SW제품들이 많이 늘어나고 있는데 백신이나 통합 드라이버 설치기 등 Util 프로그램들이 실제로 이러한 경향을 많이 보인다.
### 6.퍼미션,그룹,유저에 대해 설명하라 
	- 바꾸는 법 설명 (슈퍼유저가 되었다고 생각하고) 어떤 명령어 쳐야 하는지
    - chmod 777 filename
    - chown <옵션> 소유자파일
    - chown 소유자 파일 -> 소유자 변경 
    - chown :그룹 파일 -> 그룹변경
    - chown 소유자:그룹 파일 -> 소유자 그룹 동시 변경
    - su {username}
    - 리눅스는 여러명의 사용자가 동시에 접속하여 사용하는 시스템이다.
    리눅스의 관리자는 그 여러명의 사용자 각각 접근할 수 있는 영역이나 파일등을 관리해야 할 필요성이 있으므로 각 계정에 따른 권한 관리를 알아야 한다.
    사용자가 사용하는 계정은 하나 이상의 그룹에 소속되어 있다.

    - /etc/passwd 파일 -> 현재 계정을 알아 볼 수 있다.
    - /etc/group 파일 -> 현재 그룹을 확인할 수 있다.

[그룹 관련 커맨드](https://3months.tistory.com/317)  
[유저 관련 커맨드](https://withcoding.com/101)  
[참조 링크1](https://www.manualfactory.net/13594)  
[참조 링크2](http://hansworld.co.kr/Instant_Backup/1261)
### 7.파일 이동하거나 복사하는 명령어들을 이렇게 해라 저렇게 해라라고 하면 그것을 하는 리눅스 명령어를 쓰면됨 그 명령어가 담긴 파일 저장
    - cp ... dir/ = 파일들을 dir에 복사
    - mv ... dir/ = 파일들을 dir에 이동

### 8.BIZ MODEL 7 Canvas (Segments)
    - 몇 개 회사를 집어주고 그 회사의 어떤 사업 (lg의 한 사업을 정해서) 7 canvas를 그리시오 미리 몇 개 해놓고 복붙ㄱㄱ
    - OSS BIZ 2- Business Canvas
    - Key partner - 같이 일하는 사람 iaas, Paas, open source
    - Key Activities - 하는 일 ex. Sw 개발, DevOps pipeline
    - Key Resources - 비즈니스에 투입하는 것 ex. Code base,Developers
    - Value Propositions - 어떤 가치 제공
    - Customer Relationships - 고객과 어떤 관계 ex. Online support
    - Channels - 고객에게 어떻게 제공 app, website, api..
    - Customer Segments - Business users
    - Cost structure(비용 구조) - 유지보수 인력,파트너 비용(IaaS)
    - Revenue streams -  거래에 의한 사용
    우버 예시
    - 주요 파트너:운전자들, 투자자, 결제업체, 지도 api 제공자, 로비스트
    - 주요 활동: 
    - 주요 자원: 네트워크, 디지털 플랫폼, 숙련된 운전자
    - 고객 관계:

![example1](/images/7canvas_example1.png)  
![example2](/images/7canvas_example2.png)  
![example3](/images/7canvas_example3.png)    
![example4](/images/kakaotaxi_7canvas.PNG)
![example5](/images/Starbucks.png)  
![example6](/images/instacart.jpeg)    
![example7](/images/netflix.png)    




