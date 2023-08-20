# Iteration

- 반복문의 반복 개념과 차이가 있음
- 이터레이션을 위한 프로토콜 필요
    - 프로토콜에 따라 이터레이션 수행

### 이터레이션 프로토콜

- 이터레이션 할 수 있는 구조의 오브젝트여야 함
- 이터레이션 프로토콜 구분
    - Iterable
    - Iterator

### 이터러블 프로토콜

- 오브젝트가 반복할 수 있는 구조
- Symbol.iterator 를 갖고 있어야 함
- Array, Argument, String, TypedArray, Map, Set, DOM NodeList

### 이터러블 오브젝트

- 이터러블 프로토콜을 갖고 있는 오브젝트
- 반복 구조, Symbol.iterator()
- 스펙에서는 @@iterator() 로 표기
- 자체 오브젝트에는 없지만 이터러블 오브젝트 상속 가능
    - prototype chain (__proto__) 에 있으면 가능 

### 이터레이터 프로토콜

- 값을 순서대로 생성하는 방법
- 이터레이터 오브젝트 
  - Symbol.iterator() 를 호출하면 이터레이터 오브젝트를 생성하여 반환
  - 이터레이터 오브젝트에 next()가 있음 생성한 오브젝트를 이터레이터라고도 부름
- 이터레이터 오브젝트 구조 
  - {value:any, done: bool}
  - done 이 true, value 가 undefined 이면 모두 처리한 상태

