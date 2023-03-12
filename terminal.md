# 터미널

### 서버 환경

`top`

## 네트워크 보기
`sudo lsof -i :3000 `

## 설정
검색어 히스토리 
- history

현재경로
- pwd

cron 확인하기
- crontab -e

서버 용량 확인하기
- df -h

백그라운드에서 서버 실행하기
- `&`

pid 삭제하기
- kill -9 ‘pid번호’

#### 쉘 스크립트 열기
`sh 쉘명.sh`



#### search
- ps -ef | gprep ‘검색명’
- grep ‘검색멍’ 파일명.log | WC-c 단어 개수
- tail -500f 파일명 | grep 검색어
