# Destructuring

## Destructuring, Array 분할 할당

- 배열의 엘리먼트를 분할하여 할당
    - 인덱스에 해당하는 변수에 할당
    - 매치되는 인덱스에 변수가 없으면 값을 할당하지 않음
- spread 와 같이 사용
    ```javascript
    let one, two, rest 
    [one, two, rest] = [1,2,3,4,5,6,7,8,9]
    ```

## Object 분할 할당, 파라미터 분할 할당

- Object 프로퍼티를 분할하여 할당 
  ```javascript
  const {one, two} = {one: 1, two: 2}
  ```
- Object 구조에 맞추어 값 할당
  ```javascript
  let five, six 
  ({one: five, two: six} = {one: 5, two: 6})
  ```
- spread 분할 할당 
  ```javascript
  const {one, ...rest} = {one: 1, two: 2, three: 3, four: 4, five: 5}
  ```

## Object 오퍼레이션, 프로퍼티 이름 조합

- 같은 프로퍼티 이름 사용할시에는 뒤에 작성한 프로퍼티 값으로 대체
- 
