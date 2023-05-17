## npm init -y 
기본 npm init을 눌렀을 때 물어보는 질문들을 다 생략하고 바로 생성해줌

<br>

## npm install
node_modules 설치 명령어 

<br>

## npm을 사용하는 이유, 장점  
- 장점 1: 라이브러리간의 의존관계 (특정 라이브러리가 다른 라이브러리의 영향을 받을 떄) package.json에 모아서 정리할 수 있다.

- 장점 2: 라이브러리 **공식문서(cdn)** 를 확인하고 설치하는 것이 아닌 터미널에서 바로 설치할 수 있다.

<br>

## npm uninstall
기존에 내가 설치한 라이브러리를 지움 

<br>

## npm install 설치 옵션 

<br>

### - npm 전역 설치 
```
npm install 설치할 라이브러리 --global or -g
```
이렇게 설치하면  
```
/usr/local/lib/node_modules  
```
이 경로에 설치됨 

시스템 레벨에 전역으로 설치하게 하는 것임  

<br>

### - npm 지역 설치 
<br>

NPM 지역 설치에 자주 사용되는 2가지 옵션은 다음과 같습니다.
```
npm install jquery --save-prod ( --save-prod는 생략해도 알아서 됨 )
npm install jquery --save-dev
```

위 명령어는 아래와 같이 각각 축약할 수 있습니다.
```
npm i jquery
npm i jquery -D
```

<br>

## dependencies와 devDependencies의 차이 
- dependencies 
  - 애플리케이션과 직관되어 있는, 화면에 영향을 미치는 라이브러리 같은 것을 설치한다.
  
  - ```
    npm install jquery or npm i jquery
- devDependencies 
  - webpack, js-compress, sass 등 개발을 할 때 도움을 주는 개발용 라이브러리를 설치한다.

  - ```
    npm install webpack --save -dev of npm i webpack -D

 - **devDependencies에 있는 라이브러리는 배포시 설치되지 않는다.**
   