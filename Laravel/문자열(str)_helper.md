* Helper laravel.com/docs/11.x/helpers 참고

Controller 코드

//$rs = Str::after('Hello my World','my');
$rs = Str::of('Hello my World')->after('my');
echo "<br>결과1 : ".$rs."<br><br>"; // 결과 : World

//$rs = Str::before('Hello my World','my');
$rs = Str::of('Hello my World')->before('my');
echo "<br>결과2 : ".$rs."<br><br>"; // 결과 : Hello

//$rs = Str::afterLast('010-1234-5678','-');
$rs = Str::of('010-1234-5678')->afterLast('-');
echo "<br>결과3 : ".$rs."<br><br>"; // 결과 : 5678

//$rs = Str::replace('5678','1234','010-1234-5678');
$rs = Str::of('010-1234-5678')->replace('5678','1234');
echo "<br>결과4 : ".$rs."<br><br>"; // 결과 : 010-1234-1234
        
//$rs = Str::repeat("+",5);
$rs = Str::of('+')->repeat(5);
echo "<br>결과5 : ".$rs."<br><br>"; // 결과 : +++++

$rs = Str::random(7);
echo "<br>결과6 : ".$rs."<br><br>"; // 결과 : aKffuF1(문자열 7개)

//$rs = Str::remove('aa','abaabccaa');
$rs = Str::of('abaabccaa')->remove('aa');
echo "<br>결과7 : ".$rs."<br><br>"; // 결과 : abbcc

//containsAll : 동일한 단어가 있는지 확인, 대소문자 구분, 일치 시 1(True) / 불일치 시 공백 return
$rs = Str::of('Hello Laravel World')->containsAll(['Laravel','World']);
echo "<br>결과8 : ".$rs."<br><br>"; // 결과 : abbcc
