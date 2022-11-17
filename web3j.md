# web3j

참고 : https://docs.web3j.io/4.8.7/  

Web3j is a highly modular, reactive, type safe Java and Android library for working with Smart Contracts and integrating with clients (nodes) on the Ethereum network:  
(구글 번역 : Web3j는 스마트 계약과 함께 작업하고 Ethereum 네트워크의 클라이언트(노드)와 통합하기 위한 고도의 모듈식 반응형 유형 안전 Java 및 Android 라이브러리입니다.)  


## Install web3j CLI
아래 명령으로 web3j cli를 설치 할 수 있다.
````
curl -L get.web3j.io | sh && source ~/.web3j/source.sh
````

web3j CLI 버전 확인  
````
web3j -version
````

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




## truffle ABI(json file) to Java
빌드된 contract ABI 파일(json)을 Java 애플리케이션에서 호출 하기 위한 Java Class 파일 생성 방법.  
````
web3j generate truffle \
    --truffle-json=<truffle에서 생성된 json파일 경로> \
    --outputDir=<생성할 java파일 경로> \
    --package=<생성할 java 패키지명>
````
