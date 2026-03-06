# CUMPLE-ROSARIO
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Invitación 🎉</title>

<style>

body{
font-family:"Times New Roman", Times, serif;
margin:0;
background:linear-gradient(135deg,#ff758c,#ff7eb3);
color:white;
text-align:center;
}

.container{
padding:40px;
max-width:700px;
margin:auto;
}

.card{
background:rgba(0,0,0,0.35);
padding:30px;
border-radius:20px;
box-shadow:0 10px 30px rgba(0,0,0,0.3);
}

h1{
font-size:42px;
letter-spacing:2px;
}

p{
font-size:20px;
}

#contador{
font-size:28px;
margin:20px 0;
font-weight:bold;
}

iframe{
border-radius:15px;
margin-top:20px;
}

.btn{
display:inline-block;
margin-top:20px;
padding:15px 30px;
font-size:20px;
background:#25D366;
color:white;
text-decoration:none;
border-radius:50px;
transition:0.3s;
}

.btn:hover{
background:#1ebe5d;
}

</style>
</head>

<body>

<div class="container">
<div class="card">

<h1>🎉 Invitación 🎉</h1>

<p>Rosario te invita a celebrar</p>

<p><b>Fecha:</b> 3 Abril 2026</p>
<p><b>Hora:</b> 20:00 hs</p>
<p><b>Lugar:</b> Mi casa</p>
<p><b>Dirección:</b> Gervasio Posadas 254, Beccar</p>

<div id="contador"></div>

<h2>📍 Ubicación</h2>

<iframe
width="100%"
height="300"
src="https://www.google.com/maps?q=Gervasio%20Posadas%20254%20Beccar&output=embed">
</iframe>

<a class="btn"
href="https://wa.me/5491112345678?text=Hola%20Rosario%20confirmo%20mi%20asistencia%20🎉"
target="_blank">

Confirmar por WhatsApp 💬

</a>

</div>
</div>

<script>

var fechaEvento = new Date("Apr 3, 2026 20:00:00").getTime();

var x = setInterval(function(){

var ahora = new Date().getTime();
var distancia = fechaEvento - ahora;

var dias = Math.floor(distancia / (1000*60*60*24));
var horas = Math.floor((distancia % (1000*60*60*24)) / (1000*60*60));
var minutos = Math.floor((distancia % (1000*60*60)) / (1000*60));

document.getElementById("contador").innerHTML =
"⏳ Faltan " + dias + " días " + horas + "h " + minutos + "m";

},1000);

</script>

</body>
</html>
