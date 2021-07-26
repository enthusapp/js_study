# 반복문 배우기 - for
```
for (초기값; 조건식; 어떤 간격으로) {
  실행할 문장
}
```
```
for(i=0; i<10; i++) {
  console.log(i + '번째 반복 문장 입니다.');
}
/*
0번째 반복 문장입니다.
1번째 반복 문장입니다.
2번째 반복 문장입니다.
3번째 반복 문장입니다.
4번째 반복 문장입니다.
5번째 반복 문장입니다.
6번째 반복 문장입니다.
7번째 반복 문장입니다.
8번째 반복 문장입니다.
9번째 반복 문장입니다.
*/
```
```
var hometown = [
	{name: '남준', place: '일산', city: '고양'},
	{name: '진', place: '과천'},
	{name: '호석', place: '광주', city: '전라도'},
	{name: '지민', place: '부산', city: '경상도'}
];

for (var i = 0; i < hometown.length; i++) {
	var h = hometown[i];
	if (!h || !h.city) continue; // 다음 문장들은 무시되고 다음 반복

	console.log(i + ' 번째 실행입니다.');
	
	if (h.name === '호석') {
		console.log(h.name + '의 고향은 ' + h.city + ' ' + h.place + ' 입니다.');
		break; // 반복문 종료
	}
}
// 0 번째 실행입니다.
// 2 번째 실행입니다.
// 호석의 고향은 전라도 광주 입니다.
```
