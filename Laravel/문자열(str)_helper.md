* Helper laravel.com/docs/11.x/helpers 참고

* Controller 코드
  
|코드|결과|
|---|---|
|//하단 코드와 결과는 동일<br>//$rs = Str::after('Hello my World','my');<br>$rs = Str::of('Hello my World')->after('my');<br>echo $rs;|World|
|//하단 코드와 결과는 동일<br>//$rs = Str::before('Hello my World','my');<br>$rs = Str::of('Hello my World')->before('my');<br>echo $rs;|Hello|
|//하단 코드와 결과는 동일<br>//$rs = Str::afterLast('010-1234-5678','-');<br>$rs = Str::of('010-1234-5678')->afterLast('-');<br>echo $rs;|5678|
|//하단 코드와 결과는 동일<br>//$rs = Str::replace('5678','1234','010-1234-5678');<br>$rs = Str::of('010-1234-5678')->replace('5678','1234');<br>echo $rs;|010-1234-1234|
|//하단 코드와 결과는 동일<br>//$rs = Str::repeat("+",5);<br>$rs = Str::of('+')->repeat(5);<br>echo $rs;|+++++|
|$rs = Str::random(7);<br>echo $rs;|aKffuF1(문자열 7개)|
|//하단 코드와 결과는 동일<br>//$rs = Str::remove('aa','abaabccaa');<br>$rs = Str::of('abaabccaa')->remove('aa');<br>echo $rs;|abbcc|
|//containsAll : 동일한 단어가 있는지 확인, 대소문자 구분, 일치 시 1(True) / 불일치 시 공백 return<br>$rs = Str::of('Hello Laravel World')->containsAll(['Laravel','World']);<br>echo $rs;|abbcc|
