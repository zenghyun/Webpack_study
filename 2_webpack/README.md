# Webpack 

[Webpack이란?]()


## 웹팩 설정 파일 설명 
📌 webpack.config.js

```javascript
var path = require('path');

module.exports = {
  mode: 'none',
  entry: './src/index.js',
  output: {
    filename: 'main.js',
    path: path.resolve(__dirname, 'dist')
  }
};
```

<br>

### webpack
코드를 묶고 변환하기 위한 특정 기능을 플러그인 하도록 해준다.
```
npm install webpack
```

<br>

### webpack-cli
프로젝트에서 웹팩 명령어를 실행하려면 webpack-cli가 필요하다.
```
npm install webpack-cli
```
