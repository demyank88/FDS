###### Front-end Development School

# DAY 28

### DOM Level 0.

* a가 name을 가지고 있으면 
* a가 href를 가지고 있으면 link, id를 사용하는 것을 권장
* form에서는 반드시 name을 사용해야 함

* form에서 placeholder로 label을 절대로 대체 할 수 없음.
* label을 쓰고 안보이게 해야됨

* name을 쓰는 경우는 form 뿐이다...
  * name을 써야 데이터 전송이 가능하다.
  * name이 있으면 document에서 바로 접근도 가능함.
    * **지금은 name을 쓰지 않음**
    * 지금 쓰는게 `getElementsByTagName` 같은 방식 - DOM Level. 1
      * 초창기 웹은 단락을 무시했었음...
    * 이름에 하이픈이 있으면 객체로 접근할 수 없음
    * `['name']`써서 접근할 수 있음. 

```js
// 과거의 코드는 사라져야 한다.
if(document.all) {
  // IE
} else {
  // NN
}

if(document.layers) {
  // NN
} else {
  // IE
}
//발견하면 지우자...
```

### 중급 DOM
* 1997년 CSS가 불완전한 상태로 등장한 시기
* 해당 요소의 CSS 속성을 조작할 수 있는 API를 제공한 것이 중급 DOM 
* CSS와 중급 DOM이 현대 웹 디자인의 시초...

#### DOM Level 1
* 1998년... 표준화 착수
* js는 요소이름이나 ID로 만 접근이 가능했었음... 하지만 문서 내에 ID는 하나만 써야됨.
  * class가 느리다? 클래스 관련 인터페이스가 나오기 전에는 많이 느렸음.
  * class 네임으로 접속하는 인터페이스가 나오지만 IE 6,7,8에서 안됨....... IE....
  * class 탐색 방식은 모든 요소에 한번씩 물어봐야 하는 형태였음. 그래서 느림.

#### DOM Level 2
* IE 가 세상을 점령해서 표준을 무시하기 시작함
* 이때 진보된 이벤트 모델이 나이고 시작함.
  * 커스템 이벤트 모델을 만들 수 있는 시대의 시작... 정식으로 표준이 된것은 작년...
  * 이미 jQuery에서는 커스템 이벤트 모델이 되고 있었음.


### 문서 객체 모델

#### DOM 프로퍼티
* 객체가 소유한 프로퍼티
  * 객체가 변수를 소유하면 프로퍼티가 됨.

* 노드 인터페이스
  * 노드에 접근하고 변경하고 조작하는~

* document.---


