# 생활코딩

### CSS

- CSS 등장 이전의 상황
    
    ```html
    <!doctype html>
    <html>
    <head>
      <title>WEB - CSS</title>
      <meta charset="utf-8">
      <style>
          a{
              color:blue;
          }
      </style>
    </head>
    <body>
        <h1><a href="index.html">WEB</a></h1>
        <ol>
          <li><a href="1.html">HTML</a></li>
          <li><a href="2.html">CSS</a></li>
          <li><a href="3.html">Javascript</a></li>
        </ol>
    <!--<body>
      <h1><a href="index.html"><font color="red">WEB</font></a></h1>
      <ol>
        <li><a href="1.html"><font color="red">HTML</font></a></li>
        <li><a href="2.html"><font color="red">CSS</font></a></li>
        <li><a href="3.html"><font color="red">JavaScript</font></a></li>
      </ol>
    -->
      <h2>CSS</h2>
      <p>
        Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document written in a markup language.[1] Although most often used to set the visual style of web pages and user interfaces written in HTML and XHTML, the language can be applied to any XML document, including plain XML, SVG and XUL, and is applicable to rendering in speech, or on other media. Along with HTML and JavaScript, CSS is a cornerstone technology used by most websites to create visually engaging webpages, user interfaces for web applications, and user interfaces for many mobile applications.
      </p>
      </body>
      </html>
      </html>
    ```
    
    ---
    
    코딩을 잘하는 기본적인 방법 
    
    - 중복 코드의 제거
    → 중복된 코드가 있냐없냐에 따라 규모가 커지면 차이가 커진다.
    → font tag를 예로들어 일괄적으로 바꿔버리면 작성자의 의도와 다르게 바꾸면 안되는 것 또한 바뀔 수도있다. 하지만 중복을 제거한 공통분모를 가진 코드를 바꾸는 것은 공통분모를 가지고 있기 때문에 앞선 실수가 적어진다.
    
- CSS의 등장
    
    [https://www.youtube.com/watch?v=L41Zjl7XANI](https://www.youtube.com/watch?v=L41Zjl7XANI)
    
    ```html
    <!doctype html>
    <html>
    <head>
      <title>WEB - CSS</title>
      <meta charset="utf-8">
      <style>
          a {
              color:black;
          }
      </style>
    </head>
    <body>
        <h1><a href="index.html">WEB</a></h1>
        <ol>
          <li><a href="1.html">HTML</a></li>
          <li><a href="2.html" style="color:red; text-decoration:underline">CSS</a></li>
          <li><a href="3.html">Javascript</a></li>
        </ol>
    <!--<body>
      <h1><a href="index.html"><font color="red">WEB</font></a></h1>
      <ol>
        <li><a href="1.html"><font color="red">HTML</font></a></li>
        <li><a href="2.html"><font color="red">CSS</font></a></li>
        <li><a href="3.html"><font color="red">JavaScript</font></a></li>
      </ol>
    -->
      <h2>CSS</h2>
      <p>
        Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document written in a markup language.[1] Although most often used to set the visual style of web pages and user interfaces written in HTML and XHTML, the language can be applied to any XML document, including plain XML, SVG and XUL, and is applicable to rendering in speech, or on other media. Along with HTML and JavaScript, CSS is a cornerstone technology used by most websites to create visually engaging webpages, user interfaces for web applications, and user interfaces for many mobile applications.
      </p>
      </body>
      </html>
      </html>
    ```
    
    CSS가 도입된 이유
    
    1. HTML이 정보에 전념하게 하기 위해서 HTML로부터 디자인의 기능을 뺏어온것이 CSS이다.
    2. CSS를 통해서 웹페이지를 디자인하는 것이 HTML로 디자인하는 것 보다 효율적이기 때문
    
- CSS의 기본문법
    
    [https://www.youtube.com/watch?v=h0AlL9YI6bM&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=4](https://www.youtube.com/watch?v=h0AlL9YI6bM&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=4)
    
    ```html
    <!doctype html>
    <html>
    <head>
      <title>WEB - CSS</title>
      <meta charset="utf-8">
      <style>
          a {
              color:black;
              text-decoration: none;
          }
      </style>
    </head>
    <body>
        <h1><a href="index.html">WEB</a></h1>
        <ol>
          <li><a href="1.html">HTML</a></li>
          <li><a href="2.html" style="color:red; text-decoration:underline">CSS</a></li>
          <li><a href="3.html">Javascript</a></li>
        </ol>
    <!--<body>
      <h1><a href="index.html"><font color="red">WEB</font></a></h1>
      <ol>
        <li><a href="1.html"><font color="red">HTML</font></a></li>
        <li><a href="2.html"><font color="red">CSS</font></a></li>
        <li><a href="3.html"><font color="red">JavaScript</font></a></li>
      </ol>
    -->
      <h2>CSS</h2>
      <p>
        Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document written in a markup language.[1] Although most often used to set the visual style of web pages and user interfaces written in HTML and XHTML, the language can be applied to any XML document, including plain XML, SVG and XUL, and is applicable to rendering in speech, or on other media. Along with HTML and JavaScript, CSS is a cornerstone technology used by most websites to create visually engaging webpages, user interfaces for web applications, and user interfaces for many mobile applications.
      </p>
      </body>
      </html>
      </html>
    ```
    
    Web browser 에게 어디서 어디까지가 CSS인지 알려줘야 한다.
    
    - <style> tag가 그 역할을 한다.
    - 문법의 끝을 구분해주는 구분자로 ; (세미클론)을 사용한다.
    
    Web page에 CSS를 넣는 방법으로는
    
    1. <style> tag를 사용
    2. HTML의 style 속성을 사용
    
    CSS에서는 선택자(Selector)를 사용한다. 그리고 선택자를 통해 효과(Declaration)를 준다.
    
    HTML의 style 속성을 사용할 때는 선택자가 필요가 없다.
    
- 혁명적 변화
    
    [https://www.youtube.com/watch?v=nC2-nJEXL2U&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=5](https://www.youtube.com/watch?v=nC2-nJEXL2U&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=5)
    
- CSS 속성을 스스로 알아내기
    
    [https://www.youtube.com/watch?v=WcED6Ia1IY4&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=6](https://www.youtube.com/watch?v=WcED6Ia1IY4&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=6)
    
    ```html
    <!doctype html>
    <html>
    <head>
      <title>WEB - CSS</title>
      <meta charset="utf-8">
      <style>
          a {
              color:black;
              text-decoration: none;
          }
      </style>
    </head>
    <body>
        <h1><a href="index.html">WEB</a></h1>
        <ol>
          <li><a href="1.html">HTML</a></li>
          <li><a href="2.html" style="color:red; text-decoration:underline">CSS</a></li>
          <li><a href="3.html">Javascript</a></li>
        </ol>
    <!--<body>
      <h1><a href="index.html"><font color="red">WEB</font></a></h1>
      <ol>
        <li><a href="1.html"><font color="red">HTML</font></a></li>
        <li><a href="2.html"><font color="red">CSS</font></a></li>
        <li><a href="3.html"><font color="red">JavaScript</font></a></li>
      </ol>
    -->
      <h2>CSS</h2>
      <p>
        Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document written in a markup language.[1] Although most often used to set the visual style of web pages and user interfaces written in HTML and XHTML, the language can be applied to any XML document, including plain XML, SVG and XUL, and is applicable to rendering in speech, or on other media. Along with HTML and JavaScript, CSS is a cornerstone technology used by most websites to create visually engaging webpages, user interfaces for web applications, and user interfaces for many mobile applications.
      </p>
      </body>
    </html>
    ```
    
    기본적인 CSS 구조를 알았으니 검색을 할 수 있게 됐다.
    (검색하는 습관을 기르자!!!)
    
    - css text size property
        - font-size
    - css text center property
- CSS 선택자의 기본
    
    [https://www.youtube.com/watch?v=8-rCMmamtDE&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=7](https://www.youtube.com/watch?v=8-rCMmamtDE&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=7)
    
    ```html
    <!doctype html>
    <html>
    <head>
      <title>WEB - CSS</title>
      <meta charset="utf-8">
      <style>
          a {
              color: black;
              text-decoration: none;
          }
          .saw {
              color: gray;
          }
          h1 {
              font-size: 45px;
              text-align: center;
          }
      </style>
    </head>
    <body>
        <h1><a href="index.html">WEB</a></h1>
        <ol>
          <li><a href="1.html" class="saw">HTML</a></li>
          <li><a href="2.html" class="saw">CSS</a></li>
          <li><a href="3.html">Javascript</a></li>
        </ol>
    <!--<body>
      <h1><a href="index.html"><font color="red">WEB</font></a></h1>
      <ol>
        <li><a href="1.html"><font color="red">HTML</font></a></li>
        <li><a href="2.html"><font color="red">CSS</font></a></li>
        <li><a href="3.html"><font color="red">JavaScript</font></a></li>
      </ol>
    -->
      <h2>CSS</h2>
      <p>
        Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document written in a markup language.[1] Although most often used to set the visual style of web pages and user interfaces written in HTML and XHTML, the language can be applied to any XML document, including plain XML, SVG and XUL, and is applicable to rendering in speech, or on other media. Along with HTML and JavaScript, CSS is a cornerstone technology used by most websites to create visually engaging webpages, user interfaces for web applications, and user interfaces for many mobile applications.
      </p>
      </body>
    </html>
    ```
    
    1. a tag를 기본적으로 검은색
    2. 방문한적 있는 것은 회색
    3. 방문하고 있는 것은 빨간색 
    
    1. saw Html tag에 선택자를 붙여 CSS를 적용하고 싶다?
    
    그냥 saw 를 선택자로 하면 ?
    
    → saw 라는 모든 이름의 태그를 선택하는 선택자
    
    → 이때 앞에 . 을 붙이게 되면 class가 saw인 태그를 가르키는 선택자가 된다.
    
    보다 가까이에 있는 명령이 큰 명령을 갖는다.
    
    따라서 tag 선택자 → class 선택자 . → id 선택자 # 순으로 강한 순서이다.
    
    전부 class 선택자라면 마지막에 등장하는 선택자가 우선 순위를 가진다.
    
    id 선택자는 PK 이다.
    
    CSS Selector 를 검색해보면 다양한 자료가 나온다!
    → 검색하는 힘을 기르자!!!!!!!
    
- 박스 모델
    
    [https://www.youtube.com/watch?v=MLjCVUspcDo&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=8](https://www.youtube.com/watch?v=MLjCVUspcDo&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=8)
    
    ```html
    <html>
        <head>
            <meta charset="utf-8">
            <title></title>
            <style>
                /*
                block level element
                */
                h1, a{
                    border-width: 5px;
                    border-color: red;
                    border-style: solid;
                    display: inline;
                }
                /*
                inline element
                */
                /*a {
                    border-width: 5px;
                    border-color: red;
                    border-style: solid;
                }*/
            </style>
        </head>
        <body>
            <h1>김재근</h1> 
            나는 <a href="https://github.com/geuun">김재근</a>이다!!!!!!!
            코딩 잘하고싶다아아아아아아아아아!!!!!!!!
        </body>
    </html>
    ```
    
    - border : 테두리
    - border - width : 테두리 두께
    - border - color : 테두리 컬러
    - border - style : 테두리의 스타일
    ex) 단선인지 실선인지
    - block level element : 화면 전체를 쓰는 태그
    - inline element :  자기 자신의 크기만큼 갖는 태그
    - display : 속성 
    ex) inline, block
    - display : none; 태그를 안 보이게 할 수 있음.
    - padding : 콘텐츠와 테두리 사이의 여백
    - margin : 테두리와 테두리사이의 간격
    
- 박스 모델 써먹기

    [박스 모델 써먹기](https://www.youtube.com/watch?v=4ir8XAf7wxI&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=9)

- 그리드 소개
    
    [그리드 소개](https://www.youtube.com/watch?v=M1eQFIBY2vI&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=10)

    디자인을 위해서 아무 의미가 없는 태그를 사용해야할 때가 필요하다
    
    그것이 <div> , <span> 태그이다.
    
    최신 기술을 사용해도 될지 안될지는 데이터에 근거해서 판단할 필요가 있다.
    
    [그리드 소개](https://caniuse.com/)
    
- 그리드 써먹기
    
    [그리드 써먹기](https://www.youtube.com/watch?v=AL8RSY8rADY&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=11&t=17s)
    
- 미디어 쿼리 소개
    
    [미디어 쿼리 소개](https://www.youtube.com/watch?v=aA4xunvDWU8&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=12)
    
    웹은 수많은 기기의 형태에서도 작동해야한다.
    →다양한 환경에서 적응할 수 있는 반응형 웹이 등장했다.
    
    반응형 디자인
    → 화면에 크기에 따라서 웹페이지의 각 요소들이 반응해서 동작하는 디자인
    
    미디어 쿼리는 CSS를 통해서 반응형 웹을 구현하는 방법이다.
    
- 미디어 쿼리 써먹기
    
    [미디어 쿼리 써먹기](https://www.youtube.com/watch?v=qe3nSIg2k3Y&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=13)
    
- CSS 코드의 재사용
    
    [CSS 코드의 재사용](https://www.youtube.com/watch?v=djBrHjeitUo&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=14)
    
    ```html
    <!doctype html>
    <html>
    <head>
      <title>WEB - CSS</title>
      <meta charset="utf-8">
      <link rel="stylesheet" href="style.css">
    </head>
      <body>
        <h1><a href="index.html">WEB</a></h1>
        <div id="grid">
          <ol>
            <li><a href="1.html">HTML</a></li>
            <li><a href="2.html">CSS</a></li>
            <li><a href="3.html">Javascript</a></li>
          </ol>
          <div id="article">
          <h2>CSS</h2>
            <p>
              Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document written in a markup language.[1] Although most often used to set the visual style of web pages and user interfaces written in HTML and XHTML, the language can be applied to any XML document, including plain XML, SVG and XUL, and is applicable to rendering in speech, or on other media. Along with HTML and JavaScript, CSS is a cornerstone technology used by most websites to create visually engaging webpages, user interfaces for web applications, and user interfaces for many mobile applications.
            </p>
          </div>
        </div>  
      </body>
    </html>
    ```
    
    모든 페이지에 대해 CSS를 적용해야된다면 너무 비효율적이지 않는가?
    그리고 코딩을 잘하는 방법에 있어서 반복을 줄이는게 그 하나의 방법인데 계속해서 반복 작업을 해야할까?
    
    반복 작업을 줄이기 위해 고안된 태그가 link 태그이다.
    
    네트워크적인 측에서는 웹페이지 안에 CSS를 넣는것이 효율적이다
    
    하지만 캐싱이라는 개념 때문에 그렇지 않다.
    
    캐싱이란 저장하다는 뜻으로 한번 다운로드 받았다면 파일이 바뀌기 전까지는 클라이언트 컴퓨터에 저장해놨다가 요청하면 저장된 결과를 가져와서 (네트워크를 사용을 안하기 때문에) 속도를 높일 수 있다.
    
    따라서 캐싱을 통해 웹페이지를 훨씬 더 빠르게 보여 줄 수 있으며 트래픽을 줄일 수 있는 효과를 얻을 수 있다.
    
- 수업을 마치며
    
    [수업을 마치며](https://www.youtube.com/watch?v=42Bps7nCx8I&list=PLuHgQVnccGMAnWgUYiAW2cTzSBywFO75B&index=15)
    
    CSS에서 가장 중요한 요소는 선택자와 속성이다.
    
    속성을 많이 알 수록 표현력이 풍부해지고,
    선택자를 많이 알 수록 속성을 더 정확하게 선택해서 표현할 수 있다.