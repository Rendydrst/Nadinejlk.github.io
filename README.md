<html lang="en">

<head>
  <meta charset="UTF-8" />
<meta http-equiv="X-UA-Compatible" content="IE=edge" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link href="https://fonts.googleapis.com/css2?family=Ubuntu:wght@400;500;700&display=swap" rel="stylesheet" />
<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
<link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet" />
<link href="https://fonts.googleapis.com/icon?family=Material+Icons+Sharp" rel="stylesheet" />
<script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.4.4/dist/sweetalert2.all.min.js"></script>
<title>Nadine jelek</title>
<style>
html {
scroll-behavior: smooth;
}

* {
padding: 0;
margin: 0;
font-family: "Ubuntu";
color: rgb(56, 56, 56);
}

body {
background: wheat;
/* background-image: url("https://wallpaper.dog/large/10871886.png"); */
background-image: linear-gradient(#ff71c0, #b983ff, #5aaeff);
background-position: center;
background-size: cover;
overflow: hidden;
overflow: hidden;
}

.open {
background-image: linear-gradient(#ff71c0, #b983ff);
height: 100vh;
width: 100vw;
position: fixed;
top: 0;
display: flex;
flex-direction: column;
align-items: center;
align-content: center;
justify-content: center;
z-index: 1;
transition: 0.5s all ease;
}

.open h2 {
/* margin: 0 30px; */
margin-bottom: 20px;
color: rgb(56, 56, 56);
text-align: center;
max-width: 600px;
}

.open .card {
background: white;
padding: 30px;
border-radius: 10px;
box-shadow: 10px 10px 30px rgba(0, 0, 0, 0.123);
text-align: center;
}

.open .card h3 {
margin-top: 20px;
}

.open .card img {
height: 100px;
}

.atas {
height: 100vh;
display: flex;
flex-direction: column;
justify-content: center;
align-items: center;
}

.atas img {
height: 200px;
margin-bottom: 50px;
padding: 20px 30px;
background: white;
border-radius: 20px;
box-shadow: 10px 10px 30px rgba(0, 0, 0, 0.123);
}

.atas h2 {
font-size: 1.5em;
padding: 20px 30px;
background: white;
border-radius: 20px;
box-shadow: 10px 10px 30px rgba(0, 0, 0, 0.123);
}

p {
display: block;
text-align: center;
color: rgb(56, 56, 56);
background: white;
font-weight: bold;
font-size: 1.5em;
padding: 50px 30px;
margin: 40px 20px;
border-radius: 20px;
box-shadow: 10px 10px 30px rgba(0, 0, 0, 0.123);
}

p.wm {
margin-top: 70px;
margin-bottom: 0;
padding-top: 30px;
padding-bottom: 25px;
border-radius: 20px 20px 0 0;
font-weight: 500;
font-size: 1.1em;
color: red;
}

p.wm a {
color: red;
text-decoration: none;
}

.material-icons-sharp {
color: red;
font-size: 30px;
transform: translateY(5px);
animation: kenyal 2s ease infinite;
cursor: pointer;
}

@keyframes kenyal {
0% {
transform: scale(1) translateY(5px);
}

50% {
transform: scale(1.2) translateY(5px);
}

100% {
transform: scale(1) translateY(5px);
}
}
</style>
</head>

<body class="body">
<audio class="audio" src="https://www.mboxdrive.com/Selamat%20Ulang%20Tahun%20[Jamrud].mp3" autoplay type="audio"
loop=""></audio>
<div class="open">
<div class="card">
<h2>HALO YUPI</h2>
<img onclick="mulai()" src="e.jpg" alt="" srcset="" />
<h3>Pencet foto jeleknya kalo mau buka</h3>
</div>
</div>
<div class="atas" id="atas">
<img onclick="mulai()" src="i.jpg" alt="" />
<h2>Scroll kebawah bau</h2>
</div>

<p data-aos="zoom-in">
Ciee udah kepala 7
</p>
<p data-aos="zoom-in">
Apapun keputusan kamu ambil aku bakal support kok asal positif yaaa semangatt kuliahnyaa cantikk
</p>
<p data-aos="zoom-in">
Semoga kita bisa cepet ketemu yaa cantikk
</p>


<p data-aos="zoom-in">
Pencet aja love nya
<i onclick="tanya()" class="material-icons-sharp"> favorite </i>
</p>

<script>
var musik = "";
</script>
<script>
AOS.init({
once: true,
});
</script>
<script>
var audio = document.querySelector(".audio");
if (musik) {
audio.src = musik;
}

function mulai() {
audio.play();
document.querySelector(".open").style = "opacity: 0;";
document.querySelector(".body").style = "overflow-y: scroll;";
setTimeout(function () {
document.querySelector(".open").style.display = "none";
}, 1000);
}

function wa(isi) {
window.open(
"https://wa.me/62895325421825?text= jawaban mu? :  " +
isi);
}
async function tanya() {
var {
value: kado
} = await swal.fire({
title: "Kirim alamatmu okey",
input: "text",
showCancelButton: false,
});
if (kado) {
await swal.fire("Kirim jawabannya ke wa aku");
wa(kado);
} else {
await swal.fire("Harus dijawab wleee");
tanya();
}
}
</script>
<p class="wm">
<span><a href="https://www.gabut-it.com/">kalo ada apa apa jangan dipendem sendiri</a></span>
</p>
</body>

</html>
