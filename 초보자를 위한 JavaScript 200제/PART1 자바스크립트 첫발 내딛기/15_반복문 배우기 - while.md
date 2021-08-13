# 반복문 배우기 - while
```
while (조건식) {
  반복하게 될 문장
}
```
```
do {
  반복하게 될 문장
} while (조건식)
```
```
var hometown = [
	{name: '진', city: '과천'},
	{name: '남준', place: '일산', city: '고양'},
	{name: '호석', place: '광주', city: '전라도'},
	{name: '지민', place: '부산', city: '경상도'}
];

var isHometown = function(h, name) {
	console.log(`함수가 실행되었습니다. ${h.city} 도시에서 ${name} 을 찾습니다.`);
	
	if (h.name === name) {
		console.log(`${h.name} 의 고향은 ${h.city} ${h.place} 입니다.`);
		return true;
	}	
	return false;
}

var h;
while (h = hometown.shift()) {
	if (!h.name || !h.place || !h.city) continue;
	
	var result = isHometown(h, '호석');
	if (result) break;
}

var i = 0;
var names = ['남준', '정국', '윤기', '호섭'];
var cities = ['경기', '부산', '대구', '광주'];
do {
	hometown[i] = {name: names[i], city: cities[i]};
	i++;
} while (i < 4);

console.log(hometown);
/*
함수가 실행되었습니다. 고양 도시에서 호석 을 찾습니다.
함수가 실행되었습니다. 전라도 도시에서 호석 을 찾습니다.
호석 의 고향은 전라도 광주 입니다.
[
  { name: '남준', city: '경기' },
  { name: '정국', city: '부산' },
  { name: '윤기', city: '대구' },
  { name: '호섭', city: '광주' }
]
*/
```
