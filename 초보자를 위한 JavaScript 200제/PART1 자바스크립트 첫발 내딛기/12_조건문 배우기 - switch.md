# 조건문 배우기 - switch
```
switch (표현식1) {
  case 값1:
    명령문1
    break;
  case 값2:
    명령문2
    break;
  default:
    명령문3
}
```
```
var subject = '자바스크립트';
switch (subject) {
  case 'C언어':
    console.log('초보자를 위한 C++ 200제');
    break;
  case '자바스크립트':
    console.log('초보자를 위한 자바스크립트 200제');
    break;
  case '파이썬':
    console.log('초보자를 위한 파이썬 200제');
    break;
  default:
    console.log('이젠 초보자가 아닙니다');
    break;
}
// 초보자를 위한 자바스크립트 200제
```
