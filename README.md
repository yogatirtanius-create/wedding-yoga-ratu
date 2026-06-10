# wedding-yoga-ratu
Wedding Yoga &amp; Ratu
wedding-yoga-ratu/
│
├── index.html
├── style.css
├── script.js
│
└── assets/
    ├── cover.jpg          ← gunakan gambar undangan yang Anda kirim
    ├── bride-groom.jpg    ← foto pasangan terbaik
    ├── gallery1.jpg
    ├── gallery2.jpg
    ├── gallery3.jpg
    └── music.mp3
    <!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Wedding Invitation | Yoga & Ratu</title>

<link rel="stylesheet" href="style.css">

<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;600;700&family=Great+Vibes&display=swap" rel="stylesheet">
</head>

<body>

<audio id="music" loop>
    <source src="assets/music.mp3" type="audio/mpeg">
</audio>

<section class="cover" id="cover">
    <div class="overlay">
        <h3>The Wedding Of</h3>

        <h1>Yoga & Ratu</h1>

        <p>21 Juli 2026</p>

        <div id="guest">
            Kepada Yth.
            <br>
            Bapak/Ibu/Saudara/i
        </div>

        <button onclick="openInvitation()">
            Buka Undangan
        </button>
    </div>
</section>

<section class="hero">

    <img src="assets/bride-groom.jpg" class="hero-photo">

    <h2>Pemberkatan & Resepsi Pernikahan</h2>

    <p class="verse">
        “Demikianlah mereka bukan lagi dua,
        melainkan satu.
        Karena itu, apa yang telah dipersatukan Allah,
        tidak boleh diceraikan manusia.”
        <br>
        (Matius 19:6)
    </p>

</section>

<section class="countdown">

    <h2>Menuju Hari Bahagia</h2>

    <div class="timer">
        <div><span id="days">0</span><small>Hari</small></div>
        <div><span id="hours">0</span><small>Jam</small></div>
        <div><span id="minutes">0</span><small>Menit</small></div>
        <div><span id="seconds">0</span><small>Detik</small></div>
    </div>

</section>

<section class="couple">

    <h2>Mempelai</h2>

    <div class="name">
        Yoga Tirtanius
    </div>

    <p>
        Putra dari Bapak Edy Yohanes
        <br>
        & Ibu Betsyeba Vitri Andayani
    </p>

    <div class="and">&</div>

    <div class="name">
        Sari Ratu Magdalena Bone
    </div>

    <p>
        Putri dari Bapak Lodovikus Arnoldus Bone
        <br>
        & Ibu Syelley Dwi Handayani
    </p>

</section>

<section class="event">

<div class="card">

<h3>Ibadah Pemberkatan Kudus</h3>

<p>Selasa, 21 Juli 2026</p>
<p>08.30 WIB - Selesai</p>

<p>
Gereja GPdI Megang Sakti
<br>
Kabupaten Musi Rawas
</p>

</div>

<div class="card">

<h3>Resepsi Pernikahan</h3>

<p>Selasa, 21 Juli 2026</p>
<p>11.00 WIB - Selesai</p>

<p>
Aula Gereja GPdI Megang Sakti
<br>
Kabupaten Musi Rawas
</p>

</div>

</section>

<section class="gallery">

<h2>Galeri</h2>

<div class="gallery-grid">

<img src="assets/gallery1.jpg">
<img src="assets/gallery2.jpg">
<img src="assets/gallery3.jpg">

</div>

</section>

<section class="maps">

<h2>Lokasi Acara</h2>

<iframe
src="https://maps.google.com/maps?q=Megang%20Sakti&t=&z=13&ie=UTF8&iwloc=&output=embed">
</iframe>

</section>

<section class="rsvp">

<h2>Konfirmasi Kehadiran</h2>

<a
class="btn"
href="https://wa.me/6281234567890?text=Shalom,%20saya%20akan%20hadir">
RSVP WhatsApp
</a>

</section>

<footer>

<h2>Yoga & Ratu</h2>

<p>
Terima kasih atas doa dan kehadiran Anda.
</p>

</footer>

<script src="script.js"></script>

</body>
</html>
style.css
*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:'Cormorant Garamond',serif;
background:#f9f3ea;
color:#4b3c2f;
text-align:center;
}

.cover{
height:100vh;
background:url('assets/cover.jpg') center/cover;
display:flex;
justify-content:center;
align-items:center;
}

.overlay{
background:rgba(255,255,255,.75);
padding:40px;
border-radius:20px;
}

h1{
font-family:'Great Vibes',cursive;
font-size:70px;
color:#b88b2f;
}

h2{
font-size:38px;
margin-bottom:20px;
}

.hero,
.countdown,
.couple,
.gallery,
.maps,
.rsvp{
padding:80px 20px;
}

.hero-photo{
width:300px;
border-radius:20px;
margin-bottom:30px;
}

.verse{
max-width:700px;
margin:auto;
font-style:italic;
}

.timer{
display:flex;
justify-content:center;
gap:20px;
}

.timer div{
background:white;
padding:20px;
border-radius:15px;
min-width:100px;
}

.timer span{
display:block;
font-size:40px;
font-weight:bold;
color:#b88b2f;
}

.name{
font-family:'Great Vibes';
font-size:55px;
color:#b88b2f;
}

.and{
font-size:40px;
margin:20px 0;
}

.event{
display:flex;
gap:20px;
padding:80px 20px;
justify-content:center;
flex-wrap:wrap;
}

.card{
background:white;
padding:30px;
border-radius:20px;
max-width:400px;
box-shadow:0 4px 15px rgba(0,0,0,.1);
}

.gallery-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:15px;
}

.gallery-grid img{
width:100%;
border-radius:15px;
}

iframe{
width:100%;
height:350px;
border:none;
border-radius:15px;
}

.btn{
display:inline-block;
padding:15px 35px;
background:#b88b2f;
color:white;
text-decoration:none;
border-radius:50px;
}

button{
padding:15px 30px;
background:#b88b2f;
color:white;
border:none;
border-radius:50px;
cursor:pointer;
margin-top:20px;
}

footer{
padding:60px;
background:#e9dcc5;
}

@media(max-width:768px){

h1{
font-size:55px;
}

.name{
font-size:45px;
}

.timer{
flex-wrap:wrap;
}

}
script.js
function openInvitation(){

document.getElementById('cover').style.display='none';

document.getElementById('music').play();

window.scrollTo({
top:0,
behavior:'smooth'
});

}

const params = new URLSearchParams(window.location.search);

const guest = params.get("to");

if(guest){

document.getElementById("guest").innerHTML=
`Kepada Yth.<br>${guest}`;

}

const weddingDate =
new Date("2026-07-21T08:30:00").getTime();

setInterval(()=>{

const now = new Date().getTime();

const distance = weddingDate - now;

document.getElementById("days").innerHTML =
Math.floor(distance/(1000*60*60*24));

document.getElementById("hours").innerHTML =
Math.floor((distance%(1000*60*60*24))/(1000*60*60));

document.getElementById("minutes").innerHTML =
Math.floor((distance%(1000*60*60))/(1000*60));

document.getElementById("seconds").innerHTML =
Math.floor((distance%(1000*60))/1000);

},1000);
