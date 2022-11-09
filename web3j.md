# web3j
````
              _      _____ _ 
             | |    |____ (_)
__      _____| |__      / /_ 
\ \ /\ / / _ \ '_ \     \ \ |
 \ V  V /  __/ |_) |.___/ / |
  \_/\_/ \___|_.__/ \____/| |
                         _/ |
                        |__/ 
by Web3Labs
Version: 1.4.2
Build timestamp: 2022-10-21 08:18:21.49 UTC
````

## Install web3j on Ubuntu
아래 명령(ubuntu)으로 web3j 설치.  
````
curl -L get.web3j.io | sh && source ~/.web3j/source.sh
````


## truffle ABI(json file) to Java
빌드된 contract ABI 파일(json)을 Java 애플리케이션에서 호출 하기 위한 Java Class 파일 생성 방법.  
````
web3j generate truffle \
    --truffle-json=<truffle에서 생성된 json파일 경로> \
    --outputDir=<생성된 java파일 경로> \
    --package=<java 패키지명>
````
