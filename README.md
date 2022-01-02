# HTML 중첩되는 태그
다른 태그(들)을 포함하거나 다른 태그에 포함되어 사용되는 태그

### 목록 태그
어떤 요소들을 포함하는 목록을 나타낼 때 사용
```
ul > li
ol > li
```

---
```
<ul> : unordered(순서가 없는) list
```
속성: type
역할: 항목 앞의 표시자 모양
값: disc(기본), square, circle...
---
```
<ol> : ordered(순서가 있는) list
```
속성: type  ||  start
역할: 항목 앞의 표시자 형태  ||  시작할 번호
값: 1, A, a, I, i...  ||  정수 숫자값 (type과 관계없이)

---
```
<li> : list item - 목록의 요소
```
> 다른 태그들(또 다른 목록 등)을 포함할 수 있음.
---
### 테이블 태그
```
table > tr > th, td
table > caption
```
```
<table> : table - 표
```
```
<tr> : table row - 표의 한 열
```
```
<th> : table header - 각 열, 행의 머리
```
속성: colspan  || rowspan
역할:  가로로 n개 칸 병함  || 세로로 n개 칸 병함
값: 칸 개수 숫자값
>  다른 태그들을 포함할 수 있음.

```
<caption> : 표의 제목
```




