# 마크업 언어란?

### HTML(HyperText Markup Language)

**프로그래밍 언어**: 기계가 무엇을 어떻게 할지 지시를 내리는 것

**마크업 언어:** 특정 형식과 문법대로 어떤 요소나 절차를 배치하는 것

HyperText: 링크등 을 통해 다른 곳으로 이동 할수 있는 텍스트

### **WYSWYG (What Tou See What You Get)**

코드로 페이지를 만든것이 아닌 결과물에서 보일 모습 그대로 GUI로 작업하는 것

과거 웹사이트는 정적이었으나 현재는 웹이 발달하면서웹 페이지 하나에 수많은 웹페이지와 동적 요소 및  수많은 변수들이 있기 때문에 WYSWYG방식으로 만드는 데 한계

---

# HTML 구조

**<!DOCTYPE html>**

html5버전의 html형식을 가진 문서라고 명시하는 것

**<html lang="en">**

요소의 시작

**</html>**

```jsx
<html>
	<head>
	</head>
	<body>
	</body>
</html>
```

해당요소의 끝

### localhost

서버, 내 컴퓨터 를 가르키는 주소

### Port

서버가 웹사이트의 리소스를 개발할때 내보내는 여러개의 문 중 하나 

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Website</title>
</head>
<body>
    <h1>Welcom</h1>
    <p>hello world!!</p>
</body>
</html>
```

## 페이지 정보를 나타내는 태그

- **<html lang="en">**
    
    페이지의 언어를 해당 언어로 인식, 웹 페이지의 음성지원 언어 결정
    
    **Accessibility (**접근성)과 관련, 시각적으로 컨텐츠를 인식하지 않는 분들도 사용하는데 큰 지장이 없도록 설계
    
- **메타태그**
    1. **<meta charset="UTF-8">**
    가변길이 Unicode 문자 인코딩 방식
    컴퓨터 모든 정보는 숫자로 특정 규칙을 따라 문자로 변환하는 인코딩 필요 
    - **ASCII사용,**  ASCII은 알파벳만 지원함 따라서 각 나라의 여러 문자를 표시할 수 있는 여러 형식 생김
    - 영어+한글 = **euc-kr** 사용 but, 다른 문자를 표시하게되는 경우 문제 발생
    - 전세계의 모든 문자를 담은 **Unicode** 문자표 등장(인코딩 형식X)
    2. **<meta name="viewport" content="width=device-width, initial-scale=1.0">
    - content="width=device-width:**  페이지가 기기의 너비와 같게
    - **initial-scale=1.0** : 페이지에 처음 들어왔을때 페이지를 몇배줌으로 나타낼지
    ****반응형 페이지 제작에 필요
    **반응형**: 스크린 크기에 따라 컨텐츠 크기 반응
    **적응형**: pc와 모바일의 웹을 따로 작업
    3. **<meta http-equiv="X-UA-Compatible" content="IE=edge">**
    익스플로러때문에 만들어진 태그 (웹 호환성)
    **IE=edge: 최신 버전으로 웹 페이지를 읽어라**
    4. **<meta name="description" content=" "/>**
    검색엔진에서 검색된 결과의 설명
    5. **오픈그래프
    <meta property="og:title" content=" title"> 
    <meta property="og:url" content=URL">
    <meta property="og:image" content=" .png"> 
    <meta property="og:description" content=" desctiption"/>**
    다른 서비스에 링크를 보낼때 보이는 **오픈그래프**
    콘텐츠의 요약내용이 **SNS에 게시되는데 최적화된 데이터를 가지고 갈 수 있도록 설정**
    6. <link rel="stylesheet" href=" [.css](https://pm.pstatic.net/dist/css/nmain.20211230.css)"> 
    <link rel="stylesheet" href= [.css](https://ssl.pstatic.net/sstatic/search/pc/css/sp_autocomplete_210318.css)"> 
    <link rel="shortcut icon" type="image/x-icon" href="[/favicon.ico?1](https://www.naver.com/favicon.ico?1)"/> 
    **링크태그 페이지 외부의 정보와 페이지를 연결**할때 사용

---

## 제목, 부(...)제목 태그

### `<h1>` ~ `<h6>`

- 번호별로 크기가 달라짐 (높을수록 하위 제목)
- 줄바꿈 적용

---

## 줄바꿈 태그

### `<br>` vs. `<p>`

### `<br>` : break

- 닫는 태그 필요 없음, 위치 무관
- 여러번 사용 → 여러 줄
- 단순 시각적인 줄 바꿈 `(엔터)`

### `<p>` : paragraph

- 정보 부여: 한 문단, 정보 덩어리임을 나타냄
- **CSS가 적용될 단위**로 사용
- 단순 줄 바꿈이 아닌, **문단 구분**을 위한 태그

---

## 강조 태그

### `<b>` vs. `<strong>`

### `<b>` : bold

- **시각적 강조** (단순히 진하게)

### `<strong>`

- **정보적 강조** (컴퓨터에게 **중요한 정보**임을 알림)
ex, 스크린 리더가 강하게 발음

---

## 기울임 태그

### `<i>` vs. `<em>`

### `<i>` : italic

- 단순히 기울임

### `<em>` : emphasize

- 정보적 강조 (컴퓨터에게 **중요한 정보**임을 알림)
ex, 스크린 리더가 강하게 발음

---

## 기타 태그

### `<small>`

- 글씨를 작게

### `<cite>` : citation

- 저작물의 출처 표기 (**제목**을 표시할 것)

---

## 페이지 작성시 권장사항

1. h1는 페이지당 하나
2. 순서를 건너뛰지 말 것 (예: `<h1>` 다음에는 `<h2>`)
3. ~~시각적 효과~~를 위해 사용하지 말 것 (**디자인은 CSS로**)
4. 정보의 구조를 나타내는 용도로 사용할 것

---