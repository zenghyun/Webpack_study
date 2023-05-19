# 웹팩의 주요 속성 4가지

## mode 
Webpack에서 기본적으로 제공하는 타입이 3개가 있다.
production, development, none 

<br>

## entry
webpack으로 변환할 파일의 주소 

<br>

## output
결과를 출력하기위한 경로와 파일이름을 지정하는 곳 

<br>

## css-loader
css 파일을 webpack에서 인식할 수 있게 만든다. 

<br>

## style-loader 
style-loader는 webpack안에 들어가있는 style 코드를 header안에 inline 코드로 바꿔준다. 

style-loader는 css-loader보다 앞에 있어야 하고 loader는 항상 오른쪽에서 왼쪽으로 적용이 된다. 

<br>

```javascript
 module: {
    rules: [
      {
        test: /\.scss$/,
        use: ['style-loader', 'css-loader' 'sass-loader']
      }
    ]
  },
```

<br>

1. sass 파일을 css 파일로 바꾼다.

2. css 파일을 webpack에서 인식할 수 있게 만든다.

3. webpack안에 들어가있는 style 코드를 header안에 inline 코드로 바꿔준다.

<br>

## plugin 

plugin은 웹팩의 기본적인 동작에 추가적인 기능을 제공하는 속성이다. 