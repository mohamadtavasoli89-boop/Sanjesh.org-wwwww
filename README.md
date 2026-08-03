<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>سازمان سنجش آموزش کشور</title>

<style>
body{
margin:0;
font-family:tahoma;
background:#f4f4f4;
}

.login{
display:flex;
justify-content:center;
align-items:center;
height:100vh;
}

.box{
background:white;
padding:30px;
border-radius:15px;
box-shadow:0 0 15px rgba(0,0,0,.2);
width:320px;
text-align:center;
}

img{
width:120px;
margin-bottom:15px;
}

input{
width:100%;
padding:12px;
margin-top:15px;
font-size:18px;
}

button{
width:100%;
padding:12px;
margin-top:15px;
background:#0066cc;
color:white;
border:none;
font-size:18px;
border-radius:8px;
}

#dashboard{
display:none;
padding:20px;
}

.card{
background:white;
padding:20px;
margin:15px;
border-radius:12px;
box-shadow:0 0 10px rgba(0,0,0,.15);
}
</style>
</head>

<body>

<div class="login" id="login">

<div class="box">

<img src="https://upload.wikimedia.org/wikipedia/fa/5/5f/Logo_SANJESH.svg">

<h2>سازمان سنجش آموزش کشور</h2>

<input id="code" placeholder="کد ملی">

<button onclick="login()">ورود</button>

<p id="msg" style="color:red;"></p>

</div>

</div>

<div id="dashboard">

<h1>داشبورد</h1>

<div class="card">
اینجا بعداً PDF قرار می‌دهیم.
</div>

<div class="card">
اینجا بعداً عکس قرار می‌دهیم.
</div>

</div>

<script>

const password="1234567890";

function login(){

if(document.getElementById("code").value==password){

document.getElementById("login").style.display="none";

document.getElementById("dashboard").style.display="block";

}else{

document.getElementById("msg").innerHTML="کد ملی اشتباه است";

}

}

</script>

</body>
</html>
