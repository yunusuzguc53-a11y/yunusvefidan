# yunusvefidan
.
<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<title>Sana Küçük Bir Sürprizim Var 💗</title>

<style>

body{
margin:0;
font-family:Arial, sans-serif;
background:linear-gradient(135deg,#ff9ecb,#ffc0da,#ffd6ea);
color:white;
text-align:center;
overflow-x:hidden;
}

.container{
padding:60px 20px;
}

h1{
font-size:55px;
}

.card{
background:rgba(255,255,255,0.2);
backdrop-filter:blur(10px);
border-radius:20px;
padding:30px;
max-width:600px;
margin:auto;
}

button{
margin-top:20px;
background:#ff2f8e;
border:none;
padding:15px 35px;
font-size:18px;
border-radius:30px;
color:white;
cursor:pointer;
}

button:hover{
transform:scale(1.1);
}

.hidden{
display:none;
}

img{
width:250px;
border-radius:20px;
margin-top:20px;
box-shadow:0 10px 25px rgba(0,0,0,0.2);
}

/* uçan kalpler */

.heart{
position:fixed;
bottom:-10px;
font-size:25px;
animation:fly 6s linear infinite;
}

@keyframes fly{
0%{transform:translateY(0);opacity:1}
100%{transform:translateY(-100vh);opacity:0}
}

</style>
</head>

<body>

<audio autoplay loop>
<source src="muzik.mp3" type="audio/mpeg">
</audio>

<div class="container">

<h1>💗 Sana Bir Sürprizim Var 💗</h1>

<div class="card">

<p>
Hayatıma girdiğin günden beri her şey daha güzel.  
Gülüşün kalbimi ısıtıyor, varlığın bana huzur veriyor.
</p>

<p>
Sen sadece sevgilim değilsin…  
Aynı zamanda en güzel hikâyemin başrolüsün. ❤️
</p>

<img src="foto.jpg">

<br>

<button onclick="mesaj()">Mesajımı Aç 💌</button>

<div id="surpriz" class="hidden">

<p>
Eğer bir gün dünyadan bir şey isteyecek olsaydım  
o da seninle sonsuza kadar birlikte olmak olurdu.
</p>

<p>
Çünkü sen benim en güzel tesadüfümsün. 💞
</p>

<h2>Seni Çok Seviyorum ❤️</h2>

</div>

</div>

</div>

<script>

function mesaj(){
document.getElementById("surpriz").style.display="block";
}

/* kalp animasyonu */

setInterval(function(){
let heart=document.createElement("div");
heart.className="heart";
heart.innerHTML="💖";
heart.style.left=Math.random()*100+"vw";
heart.style.fontSize=(Math.random()*20+20)+"px";
document.body.appendChild(heart);

setTimeout(()=>{
heart.remove();
},6000);

},300);

</script>

</body>
</html>
