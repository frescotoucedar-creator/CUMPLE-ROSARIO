# CUMPLE-ROSARIO
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Invitación - Rosario</title>

<style>

body{
font-family:"Times New Roman", Times, serif;
margin:0;
background:#111;
color:#f5f5f5;
text-align:center;
}

.container{
max-width:700px;
margin:auto;
padding:20px;
}

.card{
background:#1b1b1b;
padding:30px 20px;
border-radius:15px;
border:1px solid #d4af37;
box-shadow:0 10px 40px rgba(0,0,0,0.6);
}

.foto{
width:100%;
border-radius:10px;
margin-bottom:20px;
}

h1{
font-size:38px;
color:#d4af37;
letter-spacing:3px;
}

h2{
color:#d4af37;
margin-top:30px;
}

p{
font-size:18px;
margin:6px 0;
}

#contador{
font-size:22px;
margin:20px 0;
color:#d4af37;
}

iframe{
width:100%;
height:250px;
border-radius:12px;
border:none;
margin-top:15px;
}

.btn{
display:block;
margin:15px auto;
padding:14px;
font-size:18px;
background:#d4af37;
color:#111;
text-decoration:none;
border-radius:40px;
font-weight:bold;
width:80%;
max-width:320px;
}

.btn:hover{
background:#f1cc5a;
}

.btn-wpp{
background:#25D366;
color:white;
}

.btn-wpp:hover{
background:#1ebe5d;
}

</style>
</head>

<body>

<div class="container">
<div class="card">

<img src="foto.jpg" class="foto">

<h1>Invitación</h1>

<p>Rosario te invita a celebrar</p>

<p><b>Fecha:</b> 3 de Abril de 2026</p>
<p><b>Hora:</b> 20:00 hs</p>

<p><b>Lugar:</b> Mi casa</p>
<p>Gervasio Posadas 254, Beccar</p>

<div id="contador"></div>

<h2>Ubicación</h2>

<iframe
src="https://www.google.com/maps?q=Gervasio%20Posadas%20254%20Beccar&output=embed">
</iframe>

<a class="btn"
href="https://www.google.com/maps/search/?api=1&query=Gervasio+Posadas+254+Beccar"
target="_blank">

Abrir en Google Maps

</a>

<a class="btn btn-wpp"
href="https://wa.me/5491123879284?text=Hola%20Rosario%20confirmo%20mi%20asistencia%20🎉"
target="_blank">

Confirmar por WhatsApp

</a>

</div>
</div>

<script>

var fechaEvento = new Date("Apr 3, 2026 20:00:00").getTime();

setInterval(function(){

var ahora = new Date().getTime();
var distancia = fechaEvento - ahora;

var dias = Math.floor(distancia/(1000*60*60*24));
var horas = Math.floor((distancia%(1000*60*60*24))/(1000*60*60));
var minutos = Math.floor((distancia%(1000*60*60))/(1000*60));

document.getElementById("contador").innerHTML =
"Faltan " + dias + " días " + horas + "h " + minutos + "m";

},1000);

</script>

</body>
</html>
