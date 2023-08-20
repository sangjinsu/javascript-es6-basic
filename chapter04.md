# Spread, Rest

## Spread

- [...iterable]
- 이터러블 오브젝트를 하나씩 전개
- 오브젝트가 이터러블 오브젝트는 아니지만 전개 가능 
- Array Spread
  - spread 대상 배열을 작성한 위치에 엘리먼트 단위로 분리 
- String Spread 
  - spread 대상 문자열을 작성한 위치에 문자 단위로 전개 
- Object Spread
  - spread 대상 Object 를 작성한 위치에 프로퍼티 단위로 전개 
  - 프로퍼티 이름이 같으면 값 대체
- push(...spread)
  - push() 파라미터에 spread 대상 작성 

## Rest

- 호출하는 함수의 파라미터에 spread 대상 작성 
- 파라미터 배열을 엘리먼트 단위로 전개 
- 전개한 순서대로 파라미터 값으로 넘겨 줌 
- 호출받는 함수의 파라미터에 순서대로 매핑됨