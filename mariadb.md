# Maria DB



## 사용자 계정 생성 방법
```
  create user '생성할 사용자ID"@'%' IDENTIFIED BY '계정 비밀번호'
```

## 사용자 권한 부여 방법
```
  grant all privileges on 데이터베이스.* to '사용자ID'@'%'
```

## 사용자 권한 부여 후 적용
```
  flush privileges
```
