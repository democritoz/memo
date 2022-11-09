# git 명령어 

## git remote

### add
git 원격 저장소 추가  
```
git remote add <name> <url>
```
예)  
```
git remote add origin https://github.com/democritoz/memo.git
```



## ubuntu에서 SSH로 github 연결 방법

1) ubuntu에서 ssh-keygen 명령을 실행
  ```
  ssh-keygen
  ```  

2) ~/.ssh/ 디렉토리에 아래 2개 파일이 생성됨.  
  id_rsa.pub 파일이 공개키 파일이다.  
  ```
  id_rsa
  id_rsa.pub
  ```  

3) ssh-keygen으로 생성된 공개키 파일 내용을 github에 등록.  
github의 아래 메뉴로 이동해서 공개키를 등록 하면 된다.
```
Github -> Settings -> SSH and GPG Kyes -> New SSH Key 
```

4) ssh 접속 테스트  
ubuntu에서 아래 명령으로 github에 접속 되는지 확인.
````
ssh -T git@github.com
