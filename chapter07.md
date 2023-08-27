# for-of 문

## for-of

- 배열을 반복하면서 엘리먼트를 하나씩 전개
- 문자열은 하나씩 반복하면서 전개
- NodeList 를 반복하면서 엘리먼트를 하나씩 전개

## for-in, for-of 차이

### for-in

- 열거 가능한 프로퍼티가 대상
- key, value 형태는 디폴트가 enumerable: true
- Object.defineProperty() 는 디폴트가 enumerable: false

### for-of

- 이터러블 오브젝트가 대상
- Object는 전개되지 않음
- prototype의 프로퍼티도 전개되지 않음

## for-of Object

- Object는 이터러블 오브젝트가 아니므로 for-of 사용 불가
- Object 를 for-offh 전개 가능한 방법
    - Object.keys() 로 프로퍼티 이름을 배열로 만들고
    - 만든 배열을 for-of 로 전개 
