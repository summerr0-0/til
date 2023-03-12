### 도커 시작

`dockerd &`	

혹은

`systemctl start docker`

### 도커 상태 확인

`ps -ef | grep docker `  혹은

 `systemctl status docker`

### 도커 컨테이너 생성

`docker create <옵션> <--name 컨테이너명> <이미지명>`

-   옵션
    -   -d 백그라운드 모드로 수행
    -   -p 호스트와 컨테이너의 포트 연결
    -   -v 호스트와 컨테이너의 디렉토리 연결
    -   -name 컨테이너 이름 설정
    -   -u 실행할 사용자 지정

### 도커 컨테이너 보기

-   모든 컨테이너 보기  
    `sudo docker ps -a`
    
-   실행중인 컨테이너 보기  
    `sudo docker ps`
    

### 컨테이너 수행하기

`sudo docker start [컨테이너]`

### 컨테이너 접속

`sudo docker attach [컨테이너]`

`docker exec -it [컨테이너] /bin/bash`

### 컨테이너 빠져나오기

-   컨테이너 종료하면서 빠져나오기  
    `exit` 혹은 `Ctrl + D`
    
-   컨테이너 유지하면서 빠져나오기  
    `Ctrl + P` 입력 후 `Ctrl + Q` 입력

### 컨테이너 종료

`docker stop [컨테이너]`

### 컨테이너 삭제하기

-   하나만 삭제하기  
    `sudo docker rm [컨테이너]`

### 현재 이미지 확인

`docker images`

### 이미지 삭제

`docker rmi [이미지]`

### 컨테이너 이미지 같이 삭제

`docker rmi -f [이미지]`

### 도커 에러 확인

`docker logs [컨테이너]`  
로 들어가서 로그를 확인해본다