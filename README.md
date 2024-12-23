<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>redirect</title>
</head>

<body>
<script>
//上面的不要碰
/*
這邊式要修改的部分
要改的部分 陣列形式
減少就拿掉 格式 [1,2,3,4] 拿掉3 就是 [1,2,4] 要加的話一樣[1,2,3,4,5] 
兩個 ' ' 中間放網址
改到一個都沒有的時候把這個index.html擋按砍掉
*/
var urls = ['[網址1](https://docs.google.com/forms/d/e/1FAIpQLScbqxl66jlP8gIs-j9TCjTEs8t_cvrsYLfBwOse0G58f6kd6Q/viewform?usp=header)',
'[網址2](https://docs.google.com/forms/d/e/1FAIpQLSfVbVU7YGv3XlRhF2xRp6CN7U0noKRmjXLBCVs0eivx6xfG5Q/viewform?usp=header)'];
//下面的不要碰
var min = 0;
var max = urls.length - 1;
if(max==0){
 window.location.href='https://www.google.com.tw';
 }
else{
 var random = Math.floor(Math.random() * (max - min + 1)) + min;
 window.location.href=urls[random];
 }
</script>
</body>
</html
