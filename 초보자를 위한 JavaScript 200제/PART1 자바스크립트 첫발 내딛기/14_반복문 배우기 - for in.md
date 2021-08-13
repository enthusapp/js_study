# 반복문 배우기 - for in
```
for (속성명 in 반복할 대상) {

}
```
```
var store = { snack: 1000, flower: 5000, beverage: 2000 };

for (var item in store) {
  if (!store.hasOwnProperty(item)) continue;

  console.log(item + ' 는 가격이 ' + store[item] + ' 입니다.')
}
// snack은 가격이 1000 입니다.
// flower는 가격이 5000 입니다.
// beverage는 가격이 2000 입니다.
```
