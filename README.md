<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>石头剪刀布</title>
<head>
<style type="text/css">
body{background: gray}
.main{margin: 0 auto;text-align: center;}
.middle{height: 300px;text-align: center;}
.alert{height:500px;margin: 0 auto;}
</style>    
</head>
<body>
<div class="main">
	<div class="middle">
		<img id="shitou" 
		src="https://raw.githubusercontent.com/fufeiha/ife/master/2015_summer/asset/shitou.jpg">
		<img id="jiandao" 
		src="https://raw.githubusercontent.com/fufeiha/ife/master/2015_summer/asset/jiandao.jpg">
		<img id="bu" 
		src="https://raw.githubusercontent.com/fufeiha/ife/master/2015_summer/asset/bu.jpg">
	</div>
	<div class="alert">
		<img id="my-result">
	    <span id="result-text"></span>
	    <img id="computer-result">
	</div>
</div>	
	<script type="text/javascript">	
	var jiandao=
	document.getElementById("jiandao");
	jiandao.onclick=function(){
	    document.getElementById("my-result").src="https://raw.githubusercontent.com/fufeiha/ife/master/2015_summer/asset/jiandao.jpg";
	var computerResult=Math.random();
	if (computerResult<0.33){
        //jiandao
		document.getElementById("computer-result").src="https://raw.githubusercontent.com/fufeiha/ife/master/2015_summer/asset/jiandao.jpg";
        document.getElementById("result-text").innerHTML="平局！";
}
    else if (computerResult<0.67){
        //shitou
    	document.getElementById("computer-result").src="https://raw.githubusercontent.com/fufeiha/ife/master/2015_summer/asset/shitou.jpg";
	    document.getElementById("result-text").innerHTML="你输了！"
}
    else {
        //bu
    	document.getElementById("computer-result").src="https://raw.githubusercontent.com/fufeiha/ife/master/2015_summer/asset/bu.jpg";
	    document.getElementById("result-text").innerHTML="你赢了！"
}
}
</script>
</body>
</html>
