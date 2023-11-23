### 1. 컨테이너 기술이란 무엇입니까? (100자 이내로 요약)
- 컨네이너 기술은 애플리케이션 간에 운영체제(OS)를 공유하여 가볍게 사용 할 수 있는 기술입니다.
- 자체 파일 시스템, CPU 점유욜, 프로세스 공간을 컨테이너 형태로 가져 클라우드, OS 배포에 이식 할 수 있습니다.


### 2. 도커란 무엇입니까? (100자 이내로 요약)
- 도커(`Docker`)는 애플리케이션 개발, 배포, 실행하기 위한 개방형 플랫폼입니다.
- 컨테이너 애플리케이션을 배포하고 테스트가 용의합니다.

### 3. 도커 파일, 도커 이미지, 도커 컨테이너의 개념은 무엇이고, 서로 어떤 관계입니까?
- 도커 이미지는 컨테이너를 마들기 위한 지침이 포함된 읽기 전용 템플릿입니다.  
- 도커 컨테이너는 실행 가능한 이미지 인스턴스입니다.  
- 도커 파일은 도커 파일의 명령어를 순서대로 실행하는 역할을 합니다.  

1. 도커 파일 내부에 `FROM` 키워드에 새로운 이미지를 생성할 때 기반으로 사용할 이미지를 지정합니다.  
2. `ENTRYPOINT` 키워드로 컨테이너를 시작할 때 실행 할 명령어를 입력합니다.  
3.  도커 파일 작성이 완료가 되면 `docker build` 명령어를 실행합니다.  
4. 실행이 완료가 되면 도커 이미지가 생성이 됩니다.  
5. 새로 생성한 이미지로 `docker run` 명령어를 실행하여 컨테이너를 생성합니다.  
6. 컨테이너는 `ENTRYPOINT`에 지정 된 실행 명령어를 출력합니다.  
7. 출력이 완료가 되면 컨테이너는 종료가 됩니다.  