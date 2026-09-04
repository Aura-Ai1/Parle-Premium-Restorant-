<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>PARLE — Haute Gastronomie</title>
<meta name="description" content="PARLE — Gastronomi, tasarım ve deneyimin buluştuğu seçkin restoran.">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;500;600;700&family=Manrope:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>
:root{
    --black:#050505;
    --dark:#0b0b0b;
    --gold:#c9a66b;
    --gold2:#f0d29a;
    --white:#f7f3eb;
    --muted:#aaa49a;
    --line:rgba(201,166,107,.22);
    --glass:rgba(10,10,10,.62);
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    background:var(--black);
    color:var(--white);
    font-family:Manrope,sans-serif;
    overflow-x:hidden;
}

body.loading{
    overflow:hidden;
}

a{
    color:inherit;
    text-decoration:none;
}

button,
input,
select,
textarea{
    font:inherit;
}

button{
    cursor:pointer;
}

/* =========================
   PRELOADER
========================= */

.loader{
    position:fixed;
    inset:0;
    z-index:9999;
    background:#030303;
    display:flex;
    align-items:center;
    justify-content:center;
    flex-direction:column;
    transition:1s ease;
}

.loader.hide{
    opacity:0;
    visibility:hidden;
    pointer-events:none;
}

.loader-logo{
    font-family:Cinzel,serif;
    font-size:clamp(48px,9vw,110px);
    letter-spacing:.28em;
    color:var(--gold2);
    margin-left:.28em;
}

.loader-line{
    width:180px;
    height:1px;
    background:rgba(201,166,107,.2);
    margin-top:28px;
    overflow:hidden;
}

.loader-line span{
    display:block;
    width:0;
    height:100%;
    background:var(--gold);
    animation:load 1.8s ease forwards;
}

@keyframes load{
    to{width:100%}
}

/* =========================
   NAVBAR
========================= */

.nav{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    z-index:1000;
    padding:24px 5vw;
    display:flex;
    align-items:center;
    justify-content:space-between;
    transition:.5s;
}

.nav.scrolled{
    padding:15px 5vw;
    background:rgba(5,5,5,.82);
    backdrop-filter:blur(18px);
    border-bottom:1px solid rgba(201,166,107,.12);
}

.logo{
    font-family:Cinzel,serif;
    font-size:24px;
    letter-spacing:.28em;
    margin-left:.28em;
    color:var(--gold2);
}

.nav-links{
    display:flex;
    gap:35px;
    list-style:none;
}

.nav-links a{
    position:relative;
    font-size:12px;
    text-transform:uppercase;
    letter-spacing:.2em;
    color:#ddd;
}

.nav-links a::after{
    content:"";
    position:absolute;
    left:0;
    bottom:-8px;
    width:0;
    height:1px;
    background:var(--gold);
    transition:.35s;
}

.nav-links a:hover::after{
    width:100%;
}

.nav-btn{
    border:1px solid var(--gold);
    background:transparent;
    color:var(--gold2);
    padding:12px 21px;
    text-transform:uppercase;
    letter-spacing:.15em;
    font-size:10px;
    transition:.3s;
}

.nav-btn:hover{
    background:var(--gold);
    color:#080808;
}

.menu-toggle{
    display:none;
    width:42px;
    height:42px;
    border:1px solid var(--line);
    background:transparent;
    color:white;
}

/* =========================
   CINEMATIC ENTRANCE
========================= */

.entrance{
    height:100svh;
    min-height:700px;
    position:relative;
    overflow:hidden;
    background:#020202;
}

.entrance-video{
    position:absolute;
    inset:0;
    width:100%;
    height:100%;
    object-fit:cover;
    opacity:.58;
    transform:scale(1.08);
    animation:cameraApproach 12s ease-out forwards;
}

.entrance::after{
    content:"";
    position:absolute;
    inset:0;
    background:
        linear-gradient(to bottom,rgba(0,0,0,.55),transparent 35%,rgba(0,0,0,.88)),
        radial-gradient(circle at center,transparent 15%,rgba(0,0,0,.72) 100%);
    z-index:1;
}

@keyframes cameraApproach{
    from{
        transform:scale(1.08);
    }
    to{
        transform:scale(1.25);
    }
}

.entrance-content{
    position:absolute;
    z-index:3;
    inset:0;
    display:flex;
    flex-direction:column;
    align-items:center;
    justify-content:center;
    text-align:center;
    pointer-events:none;
}

.eyebrow{
    font-size:10px;
    letter-spacing:.45em;
    text-transform:uppercase;
    color:var(--gold2);
    margin-bottom:22px;
}

.hero-logo{
    font-family:Cinzel,serif;
    font-size:clamp(70px,14vw,190px);
    font-weight:400;
    letter-spacing:.22em;
    margin-left:.22em;
    line-height:.8;
    text-shadow:0 15px 50px rgba(0,0,0,.8);
}

.hero-sub{
    margin-top:32px;
    color:#ddd;
    font-size:13px;
    letter-spacing:.3em;
    text-transform:uppercase;
}

.hero-actions{
    margin-top:40px;
    display:flex;
    gap:12px;
    pointer-events:auto;
}

.primary-btn{
    padding:16px 28px;
    border:1px solid var(--gold);
    background:var(--gold);
    color:#080808;
    font-size:10px;
    letter-spacing:.18em;
    text-transform:uppercase;
    transition:.3s;
}

.primary-btn:hover{
    background:transparent;
    color:var(--gold2);
}

.secondary-btn{
    padding:16px 28px;
    border:1px solid rgba(255,255,255,.3);
    background:rgba(0,0,0,.25);
    backdrop-filter:blur(10px);
    color:white;
    font-size:10px;
    letter-spacing:.18em;
    text-transform:uppercase;
}

.scroll-indicator{
    position:absolute;
    bottom:35px;
    left:50%;
    transform:translateX(-50%);
    z-index:4;
    display:flex;
    flex-direction:column;
    align-items:center;
    gap:12px;
    color:#aaa;
    font-size:9px;
    letter-spacing:.25em;
    text-transform:uppercase;
}

.scroll-line{
    width:1px;
    height:55px;
    background:linear-gradient(var(--gold),transparent);
}

/* =========================
   INTRO
========================= */

.intro{
    min-height:70vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:120px 8vw;
    position:relative;
}

.intro::before{
    content:"";
    position:absolute;
    width:500px;
    height:500px;
    border-radius:50%;
    background:rgba(201,166,107,.05);
    filter:blur(80px);
}

.section-label{
    color:var(--gold);
    font-size:10px;
    letter-spacing:.4em;
    text-transform:uppercase;
    margin-bottom:25px;
}

.intro h2{
    font-family:Cinzel,serif;
    font-weight:400;
    font-size:clamp(35px,5vw,75px);
    line-height:1.15;
    max-width:1000px;
    position:relative;
}

.intro p{
    max-width:650px;
    margin:30px auto 0;
    color:var(--muted);
    line-height:2;
    font-size:14px;
    position:relative;
}

/* =========================
   FOOD EXPERIENCE
========================= */

.food-section{
    padding:100px 5vw 150px;
    background:#080808;
}

.section-head{
    display:flex;
    align-items:end;
    justify-content:space-between;
    gap:30px;
    margin-bottom:55px;
}

.section-title{
    font-family:Cinzel,serif;
    font-size:clamp(35px,5vw,70px);
    font-weight:400;
}

.section-description{
    max-width:420px;
    color:var(--muted);
    line-height:1.8;
    font-size:13px;
}

.food-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:20px;
}

.food-card{
    position:relative;
    height:570px;
    overflow:hidden;
    background:#111;
    cursor:pointer;
}

.food-card:nth-child(2){
    transform:translateY(55px);
}

.food-card img{
    width:100%;
    height:100%;
    object-fit:cover;
    transition:1s cubic-bezier(.2,.7,.2,1);
    filter:saturate(.8);
}

.food-card::after{
    content:"";
    position:absolute;
    inset:0;
    background:linear-gradient(transparent 35%,rgba(0,0,0,.9));
}

.food-card:hover img{
    transform:scale(1.08);
    filter:saturate(1);
}

.food-info{
    position:absolute;
    z-index:2;
    bottom:28px;
    left:28px;
    right:28px;
}

.food-category{
    color:var(--gold);
    font-size:9px;
    letter-spacing:.3em;
    text-transform:uppercase;
}

.food-name{
    font-family:Cinzel,serif;
    font-size:28px;
    margin-top:8px;
}

.food-desc{
    color:#bbb;
    font-size:12px;
    line-height:1.6;
    margin-top:8px;
}

.food-price{
    margin-top:18px;
    color:var(--gold2);
    font-size:13px;
}

/* =========================
   STORY
========================= */

.story{
    display:grid;
    grid-template-columns:1fr 1fr;
    min-height:700px;
}

.story-image{
    min-height:600px;
    overflow:hidden;
}

.story-image img{
    width:100%;
    height:100%;
    object-fit:cover;
}

.story-content{
    padding:100px 9vw;
    display:flex;
    justify-content:center;
    flex-direction:column;
    background:#0c0c0c;
}

.story-content h2{
    font-family:Cinzel,serif;
    font-size:clamp(38px,4vw,65px);
    font-weight:400;
    line-height:1.15;
}

.story-content p{
    color:var(--muted);
    line-height:2;
    margin:28px 0;
    font-size:14px;
}

.signature{
    color:var(--gold2);
    font-family:Cinzel,serif;
    font-size:22px;
}

/* =========================
   MENU
========================= */

.menu-section{
    padding:140px 6vw;
}

.filters{
    display:flex;
    flex-wrap:wrap;
    gap:10px;
    margin:45px 0;
}

.filter{
    background:transparent;
    border:1px solid rgba(255,255,255,.13);
    color:#aaa;
    padding:11px 18px;
    font-size:10px;
    text-transform:uppercase;
    letter-spacing:.15em;
    transition:.3s;
}

.filter.active,
.filter:hover{
    border-color:var(--gold);
    color:var(--gold2);
}

.menu-list{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:0 70px;
}

.menu-item{
    padding:28px 0;
    border-bottom:1px solid rgba(255,255,255,.1);
    display:grid;
    grid-template-columns:1fr auto;
    gap:20px;
}

.menu-item h3{
    font-family:Cinzel,serif;
    font-weight:400;
    font-size:20px;
}

.menu-item p{
    color:#858585;
    font-size:12px;
    margin-top:8px;
    line-height:1.6;
}

.menu-price{
    color:var(--gold2);
    font-size:13px;
}

/* =========================
   RESERVATION
========================= */

.reservation{
    position:relative;
    padding:140px 7vw;
    background:
        linear-gradient(rgba(0,0,0,.75),rgba(0,0,0,.88)),
        url("https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?auto=format&fit=crop&w=2200&q=85")
        center/cover fixed;
}

.reservation-box{
    max-width:900px;
    margin:auto;
    border:1px solid var(--line);
    background:rgba(5,5,5,.7);
    backdrop-filter:blur(20px);
    padding:60px;
}

.reservation-box h2{
    font-family:Cinzel,serif;
    font-size:50px;
    font-weight:400;
    text-align:center;
}

.reservation-box>p{
    text-align:center;
    color:#999;
    font-size:13px;
    margin:15px auto 45px;
    max-width:550px;
}

.form-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:18px;
}

.field{
    display:flex;
    flex-direction:column;
    gap:8px;
}

.field.full{
    grid-column:1/-1;
}

.field label{
    color:var(--gold);
    font-size:9px;
    text-transform:uppercase;
    letter-spacing:.2em;
}

.field input,
.field select,
.field textarea{
    width:100%;
    border:1px solid rgba(255,255,255,.13);
    background:rgba(255,255,255,.035);
    color:white;
    padding:15px;
    outline:none;
    transition:.3s;
}

.field select option{
    background:#111;
}

.field textarea{
    min-height:110px;
    resize:vertical;
}

.field input:focus,
.field select:focus,
.field textarea:focus{
    border-color:var(--gold);
}

.submit{
    margin-top:25px;
    width:100%;
    padding:17px;
    border:1px solid var(--gold);
    background:var(--gold);
    color:#050505;
    text-transform:uppercase;
    letter-spacing:.2em;
    font-size:10px;
    transition:.3s;
}

.submit:hover{
    background:transparent;
    color:var(--gold2);
}

/* =========================
   GALLERY
========================= */

.gallery{
    padding:120px 5vw;
}

.gallery-grid{
    display:grid;
    grid-template-columns:1.3fr .7fr .7fr;
    grid-template-rows:280px 280px;
    gap:14px;
}

.gallery-item{
    overflow:hidden;
    position:relative;
}

.gallery-item:first-child{
    grid-row:1/3;
}

.gallery-item img{
    width:100%;
    height:100%;
    object-fit:cover;
    transition:.8s;
}

.gallery-item:hover img{
    transform:scale(1.06);
}

/* =========================
   FOOTER
========================= */

footer{
    padding:70px 6vw 30px;
    background:#030303;
    border-top:1px solid rgba(255,255,255,.08);
}

.footer-top{
    display:flex;
    justify-content:space-between;
    gap:40px;
    padding-bottom:60px;
}

.footer-logo{
    font-family:Cinzel,serif;
    font-size:40px;
    letter-spacing:.25em;
    margin-left:.25em;
    color:var(--gold2);
}

.footer-info{
    color:#888;
    font-size:12px;
    line-height:2;
}

.footer-bottom{
    padding-top:25px;
    border-top:1px solid rgba(255,255,255,.08);
    display:flex;
    justify-content:space-between;
    gap:20px;
    color:#666;
    font-size:10px;
}

.burox{
    color:var(--gold);
    letter-spacing:.08em;
}

/* =========================
   MODAL
========================= */

.modal{
    position:fixed;
    inset:0;
    z-index:3000;
    background:rgba(0,0,0,.8);
    backdrop-filter:blur(14px);
    display:flex;
    align-items:center;
    justify-content:center;
    padding:20px;
    opacity:0;
    visibility:hidden;
    transition:.4s;
}

.modal.open{
    opacity:1;
    visibility:visible;
}

.modal-box{
    width:min(850px,100%);
    max-height:90vh;
    overflow:auto;
    background:#0c0c0c;
    border:1px solid var(--line);
    position:relative;
    display:grid;
    grid-template-columns:1fr 1fr;
    transform:translateY(30px);
    transition:.4s;
}

.modal.open .modal-box{
    transform:translateY(0);
}

.modal-img{
    width:100%;
    height:100%;
    min-height:500px;
    object-fit:cover;
}

.modal-content{
    padding:50px;
}

.modal-content h2{
    font-family:Cinzel,serif;
    font-size:38px;
    font-weight:400;
    margin:15px 0;
}

.modal-content p{
    color:#999;
    line-height:1.9;
    font-size:13px;
}

.modal-price{
    color:var(--gold2);
    margin-top:25px;
}

.close{
    position:absolute;
    top:15px;
    right:15px;
    z-index:3;
    width:40px;
    height:40px;
    border:1px solid rgba(255,255,255,.2);
    background:rgba(0,0,0,.6);
    color:white;
}

/* =========================
   TOAST
========================= */

.toast{
    position:fixed;
    right:25px;
    bottom:25px;
    z-index:5000;
    background:#101010;
    border:1px solid var(--line);
    padding:18px 22px;
    max-width:350px;
    transform:translateY(150px);
    opacity:0;
    transition:.5s;
}

.toast.show{
    transform:translateY(0);
    opacity:1;
}

.toast strong{
    display:block;
    color:var(--gold2);
    margin-bottom:5px;
    font-size:13px;
}

.toast span{
    color:#999;
    font-size:11px;
}

/* =========================
   REVEAL
========================= */

.reveal{
    opacity:0;
    transform:translateY(40px);
    transition:1s cubic-bezier(.2,.7,.2,1);
}

.reveal.visible{
    opacity:1;
    transform:none;
}

/* =========================
   RESPONSIVE
========================= */

@media(max-width:900px){

    .nav-links,
    .nav .nav-btn{
        display:none;
    }

    .menu-toggle{
        display:block;
    }

    .nav.mobile-open{
        background:#050505;
    }

    .nav.mobile-open .nav-links{
        display:flex;
        position:absolute;
        top:75px;
        left:0;
        right:0;
        padding:30px;
        background:#050505;
        flex-direction:column;
        gap:25px;
        border-bottom:1px solid var(--line);
    }

    .food-grid{
        grid-template-columns:1fr;
    }

    .food-card{
        height:500px;
    }

    .food-card:nth-child(2){
        transform:none;
    }

    .story{
        grid-template-columns:1fr;
    }

    .story-image{
        height:500px;
        min-height:0;
    }

    .menu-list{
        grid-template-columns:1fr;
    }

    .reservation-box{
        padding:35px 22px;
    }

    .form-grid{
        grid-template-columns:1fr;
    }

    .field.full{
        grid-column:auto;
    }

    .gallery-grid{
        grid-template-columns:1fr 1fr;
        grid-template-rows:250px 250px 250px;
    }

    .gallery-item:first-child{
        grid-row:auto;
        grid-column:1/-1;
    }

    .footer-top,
    .footer-bottom{
        flex-direction:column;
    }

    .modal-box{
        grid-template-columns:1fr;
    }

    .modal-img{
        min-height:280px;
        max-height:350px;
    }
}

@media(max-width:500px){

    .nav{
        padding:18px 20px;
    }

    .logo{
        font-size:19px;
    }

    .hero-logo{
        font-size:62px;
    }

    .hero-sub{
        font-size:9px;
        letter-spacing:.2em;
        padding:0 20px;
    }

    .hero-actions{
        flex-direction:column;
        width:220px;
    }

    .intro{
        padding:90px 25px;
    }

    .food-section,
    .menu-section,
    .gallery{
        padding-left:20px;
        padding-right:20px;
    }

    .section-head{
        display:block;
    }

    .section-description{
        margin-top:20px;
    }

    .gallery-grid{
        display:grid;
        grid-template-columns:1fr;
        grid-template-rows:300px 220px 220px 220px;
    }

    .gallery-item:first-child{
        grid-column:auto;
    }

    .reservation{
        padding:80px 15px;
    }

    .reservation-box h2{
        font-size:35px;
    }
}
</style>
</head>

<body class="loading">

<!-- PRELOADER -->
<div class="loader" id="loader">
    <div class="loader-logo">PARLE</div>
    <div class="loader-line">
        <span></span>
    </div>
</div>

<!-- NAVIGATION -->
<header class="nav" id="nav">

    <a href="#top" class="logo">PARLE</a>

    <ul class="nav-links">
        <li><a href="#experience">Deneyim</a></li>
        <li><a href="#menu">Menü</a></li>
        <li><a href="#story">Hikâye</a></li>
        <li><a href="#gallery">Galeri</a></li>
    </ul>

    <a href="#reservation" class="nav-btn">
        Rezervasyon
    </a>

    <button class="menu-toggle" id="menuToggle">
        ☰
    </button>

</header>


<!-- =========================
     CINEMATIC ENTRANCE
========================= -->

<section class="entrance" id="top">

    <!--
        BURAYA KENDİ RESTORAN GİRİŞ VİDEONU KOY:
        restaurant-entrance.mp4

        Video akışı:
        Üstten görünüm → restorana yaklaşma → kapıya giriş
    -->

    <video
        class="entrance-video"
        autoplay
        muted
        loop
        playsinline
        poster="https://images.unsplash.com/photo-1515003197210-e0cd71810b5f?auto=format&fit=crop&w=2200&q=85">

        <source src="restaurant-entrance.mp4" type="video/mp4">
    </video>

    <div class="entrance-content">

        <div class="eyebrow">
            HAUTE GASTRONOMIE
        </div>

        <h1 class="hero-logo">
            PARLE
        </h1>

        <div class="hero-sub">
            Gastronomi · Tasarım · Sohbet
        </div>

        <div class="hero-actions">

            <a href="#experience" class="primary-btn">
                Deneyimi Başlat
            </a>

            <a href="#reservation" class="secondary-btn">
                Masa Ayırt
            </a>

        </div>

    </div>

    <div class="scroll-indicator">
        Keşfet
        <div class="scroll-line"></div>
    </div>

</section>


<!-- INTRO -->

<section class="intro reveal" id="experience">

    <div>

        <div class="section-label">
            PARLE EXPERIENCE
        </div>

        <h2>
            Bir restorandan fazlası.
            <br>
            Bir atmosfer.
        </h2>

        <p>
            PARLE'de her detay; tabağın sunumundan ışığın masaya
            düşüşüne kadar tek bir deneyimin parçasıdır.
            Mutfağın yaratıcılığı, modern tasarım ve kusursuz
            servis aynı masada buluşur.
        </p>

    </div>

</section>


<!-- FOOD CARDS -->

<section class="food-section">

    <div class="section-head reveal">

        <div>
            <div class="section-label">
                SIGNATURE
            </div>

            <h2 class="section-title">
                İmza Tabaklar
            </h2>
        </div>

        <p class="section-description">
            Şefin seçkisi. Mevsimsel ürünler, modern teknikler
            ve PARLE'nin kendine özgü sunum anlayışı.
        </p>

    </div>


    <div class="food-grid">

        <article
            class="food-card reveal"
            data-title="Közlenmiş Dana"
            data-category="ANA YEMEK"
            data-price="₺1.950"
            data-desc="Yavaş pişirilmiş dana, kök sebzeler, yoğun demi-glace ve aromatik otlarla tamamlanan PARLE imza tabağı."
            data-image="https://images.unsplash.com/photo-1544025162-d76694265947?auto=format&fit=crop&w=1200&q=85">

            <img loading="lazy"
                 src="https://images.unsplash.com/photo-1544025162-d76694265947?auto=format&fit=crop&w=1200&q=85"
                 alt="PARLE imza dana tabağı">

            <div class="food-info">
                <div class="food-category">ANA YEMEK</div>
                <div class="food-name">Közlenmiş Dana</div>
                <div class="food-desc">
                    Kök sebzeler · Aromatik otlar · Demi-glace
                </div>
                <div class="food-price">₺1.950</div>
            </div>

        </article>


        <article
            class="food-card reveal"
            data-title="Deniz Esintisi"
            data-category="DENİZ"
            data-price="₺1.750"
            data-desc="Günün deniz ürünü, narenciye dokunuşları, hafif sebze garnitürü ve taze otlarla servis edilir."
            data-image="https://images.unsplash.com/photo-1544943910-4c1dc44aab44?auto=format&fit=crop&w=1200&q=85">

            <img loading="lazy"
                 src="https://images.unsplash.com/photo-1544943910-4c1dc44aab44?auto=format&fit=crop&w=1200&q=85"
                 alt="Deniz ürünü tabağı">

            <div class="food-info">
                <div class="food-category">DENİZ</div>
                <div class="food-name">Deniz Esintisi</div>
                <div class="food-desc">
                    Günün seçimi · Narenciye · Taze otlar
                </div>
                <div class="food-price">₺1.750</div>
            </div>

        </article>


        <article
            class="food-card reveal"
            data-title="PARLE Tatlı"
            data-category="TATLI"
            data-price="₺690"
            data-desc="Çikolata, kahve ve vanilyanın dengeli birleşimiyle hazırlanan modern PARLE tatlısı."
            data-image="https://images.unsplash.com/photo-1551024506-0bccd828d307?auto=format&fit=crop&w=1200&q=85">

            <img loading="lazy"
                 src="https://images.unsplash.com/photo-1551024506-0bccd828d307?auto=format&fit=crop&w=1200&q=85"
                 alt="PARLE tatlısı">

            <div class="food-info">
                <div class="food-category">TATLI</div>
                <div class="food-name">PARLE Tatlı</div>
                <div class="food-desc">
                    Çikolata · Kahve · Vanilya
                </div>
                <div class="food-price">₺690</div>
            </div>

        </article>

    </div>

</section>


<!-- STORY -->

<section class="story" id="story">

    <div class="story-image reveal">

        <img
            loading="lazy"
            src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?auto=format&fit=crop&w=1600&q=85"
            alt="PARLE restoran atmosferi">

    </div>

    <div class="story-content reveal">

        <div class="section-label">
            OUR PHILOSOPHY
        </div>

        <h2>
            Sessiz bir
            <br>
            zarafet.
        </h2>

        <p>
            PARLE'nin mutfak anlayışı sadelikten güç alır.
            Gereksiz hiçbir şey tabağa girmez.
            Her malzeme bir amaca, her dokunuş bir hikâyeye hizmet eder.
        </p>

        <div class="signature">
            PARLE
        </div>

    </div>

</section>


<!-- MENU -->

<section class="menu-section" id="menu">

    <div class="section-label reveal">
        THE MENU
    </div>

    <h2 class="section-title reveal">
        Menü
    </h2>

    <div class="filters reveal">

        <button class="filter active" data-filter="all">
            Tümü
        </button>

        <button class="filter" data-filter="Başlangıç">
            Başlangıç
        </button>

        <button class="filter" data-filter="Ana Yemek">
            Ana Yemek
        </button>

        <button class="filter" data-filter="Deniz">
            Deniz
        </button>

        <button class="filter" data-filter="Tatlı">
            Tatlı
        </button>

    </div>


    <div class="menu-list">

        <div class="menu-item reveal" data-category="Başlangıç">
            <div>
                <h3>İnce Kesim</h3>
                <p>Mevsim yeşillikleri · Narenciye · Özel sos</p>
            </div>
            <div class="menu-price">₺780</div>
        </div>

        <div class="menu-item reveal" data-category="Başlangıç">
            <div>
                <h3>Bahçe</h3>
                <p>Köz sebzeler · Taze otlar · Fermente dokunuş</p>
            </div>
            <div class="menu-price">₺650</div>
        </div>

        <div class="menu-item reveal" data-category="Ana Yemek">
            <div>
                <h3>Közlenmiş Dana</h3>
                <p>Kök sebzeler · Demi-glace · Aromatik otlar</p>
            </div>
            <div class="menu-price">₺1.950</div>
        </div>

        <div class="menu-item reveal" data-category="Ana Yemek">
            <div>
                <h3>Şefin Tavuğu</h3>
                <p>Çıtır deri · Kremalı sebzeler · Baharatlı jus</p>
            </div>
            <div class="menu-price">₺1.250</div>
        </div>

        <div class="menu-item reveal" data-category="Deniz">
            <div>
                <h3>Deniz Esintisi</h3>
                <p>Günün seçimi · Narenciye · Taze otlar</p>
            </div>
            <div class="menu-price">₺1.750</div>
        </div>

        <div class="menu-item reveal" data-category="Deniz">
            <div>
                <h3>Deniz Bahçesi</h3>
                <p>Mevsim deniz ürünleri · Sebze · Hafif sos</p>
            </div>
            <div class="menu-price">₺1.690</div>
        </div>

        <div class="menu-item reveal" data-category="Tatlı">
            <div>
                <h3>PARLE Tatlı</h3>
                <p>Çikolata · Kahve · Vanilya</p>
            </div>
            <div class="menu-price">₺690</div>
        </div>

        <div class="menu-item reveal" data-category="Tatlı">
            <div>
                <h3>Bahçe Meyveleri</h3>
                <p>Mevsim meyveleri · Yoğurt kreması · Bal</p>
            </div>
            <div class="menu-price">₺590</div>
        </div>

    </div>

</section>


<!-- RESERVATION -->

<section class="reservation" id="reservation">

    <div class="reservation-box reveal">

        <div class="section-label">
            YOUR TABLE
        </div>

        <h2>
            Masanız hazır.
        </h2>

        <p>
            PARLE deneyiminiz için rezervasyon talebinizi oluşturun.
            Menü ve fiyat bilgileri işletme tarafından güncellenebilir.
        </p>

        <form id="reservationForm">

            <div class="form-grid">

                <div class="field">
                    <label>Ad Soyad</label>
                    <input id="name" type="text" placeholder="Adınız Soyadınız" required>
                </div>

                <div class="field">
                    <label>E-posta</label>
                    <input id="email" type="email" placeholder="ornek@mail.com" required>
                </div>

                <div class="field">
                    <label>Tarih</label>
                    <input id="date" type="date" required>
                </div>

                <div class="field">
                    <label>Saat</label>
                    <select id="time" required>
                        <option value="">Saat seçin</option>
                        <option>18:00</option>
                        <option>18:30</option>
                        <option>19:00</option>
                        <option>19:30</option>
                        <option>20:00</option>
                        <option>20:30</option>
                        <option>21:00</option>
                        <option>21:30</option>
                    </select>
                </div>

                <div class="field">
                    <label>Kişi Sayısı</label>
                    <select id="guests" required>
                        <option value="">Seçin</option>
                        <option>1 Kişi</option>
                        <option>2 Kişi</option>
                        <option>3 Kişi</option>
                        <option>4 Kişi</option>
                        <option>5 Kişi</option>
                        <option>6 Kişi</option>
                        <option>7+ Kişi</option>
                    </select>
                </div>

                <div class="field">
                    <label>Özel Gün</label>
                    <select>
                        <option>Seçim yok</option>
                        <option>Doğum günü</option>
                        <option>Yıl dönümü</option>
                        <option>İş yemeği</option>
                        <option>Özel kutlama</option>
                    </select>
                </div>

                <div class="field full">
                    <label>Not</label>
                    <textarea placeholder="Özel bir isteğiniz varsa buraya yazabilirsiniz."></textarea>
                </div>

            </div>

            <button class="submit" type="submit">
                Rezervasyon Talebi Gönder
            </button>

        </form>

    </div>

</section>


<!-- GALLERY -->

<section class="gallery" id="gallery">

    <div class="section-label reveal">
        PARLE MOMENTS
    </div>

    <h2 class="section-title reveal">
        Atmosfer
    </h2>

    <div class="gallery-grid">

        <div class="gallery-item reveal">
            <img loading="lazy"
                 src="https://images.unsplash.com/photo-1414235077428-338989a2e8c0?auto=format&fit=crop&w=1600&q=85"
                 alt="Restoran tabağı">
        </div>

        <div class="gallery-item reveal">
            <img loading="lazy"
                 src="https://images.unsplash.com/photo-1515003197210-e0cd71810b5f?auto=format&fit=crop&w=1000&q=85"
                 alt="Restoran iç mekanı">
        </div>

        <div class="gallery-item reveal">
            <img loading="lazy"
                 src="https://images.unsplash.com/photo-1550966871-3ed3cdb5ed0c?auto=format&fit=crop&w=1000&q=85"
                 alt="Masa düzeni">
        </div>

        <div class="gallery-item reveal">
            <img loading="lazy"
                 src="https://images.unsplash.com/photo-1559339352-11d035aa65de?auto=format&fit=crop&w=1000&q=85"
                 alt="Restoran atmosferi">
        </div>

        <div class="gallery-item reveal">
            <img loading="lazy"
                 src="https://images.unsplash.com/photo-1541544741938-0af808871cc0?auto=format&fit=crop&w=1000&q=85"
                 alt="Şef sunumu">
        </div>

    </div>

</section>


<!-- FOOTER -->

<footer>

    <div class="footer-top">

        <div>
            <div class="footer-logo">
                PARLE
            </div>

            <div class="footer-info" style="margin-top:20px;">
                Haute Gastronomie<br>
                Gastronomi · Tasarım · Sohbet
            </div>
        </div>

        <div class="footer-info">
            Rezervasyon<br>
            Masa talepleri için rezervasyon formunu kullanabilirsiniz.
        </div>

        <div class="footer-info">
            Çalışma Saatleri<br>
            Her gün · 18:00 — 23:00
        </div>

    </div>

    <div class="footer-bottom">

        <span>
            © 2026 PARLE. Tüm hakları saklıdır.
        </span>

        <span class="burox">
            BUROX tarafından yapılmıştır.
        </span>

    </div>

</footer>


<!-- FOOD MODAL -->

<div class="modal" id="foodModal">

    <div class="modal-box">

        <button class="close" id="closeModal">
            ×
        </button>

        <img class="modal-img" id="modalImg" src="" alt="">

        <div class="modal-content">

            <div class="section-label" id="modalCategory">
                ANA YEMEK
            </div>

            <h2 id="modalTitle">
                Közlenmiş Dana
            </h2>

            <p id="modalDesc">
                Açıklama
            </p>

            <div class="modal-price" id="modalPrice">
                ₺1.950
            </div>

        </div>

    </div>

</div>


<!-- TOAST -->

<div class="toast" id="toast">

    <strong>Talebiniz alındı.</strong>

    <span>
        Bu demo sürümünde rezervasyon veritabanına gönderilmez.
        Gerçek sistem için backend veya WhatsApp bağlantısı eklenebilir.
    </span>

</div>


<script>

/* =========================
   LOADER
========================= */

window.addEventListener("load", () => {

    setTimeout(() => {

        document.getElementById("loader").classList.add("hide");
        document.body.classList.remove("loading");

    }, 1800);

});


/* =========================
   NAVBAR
========================= */

const nav = document.getElementById("nav");

window.addEventListener("scroll", () => {

    if(window.scrollY > 60){
        nav.classList.add("scrolled");
    }else{
        nav.classList.remove("scrolled");
    }

});


/* =========================
   MOBILE MENU
========================= */

const menuToggle = document.getElementById("menuToggle");

menuToggle.addEventListener("click", () => {
    nav.classList.toggle("mobile-open");
});


document.querySelectorAll(".nav-links a").forEach(link => {

    link.addEventListener("click", () => {
        nav.classList.remove("mobile-open");
    });

});


/* =========================
   REVEAL ANIMATION
========================= */

const observer = new IntersectionObserver(
    entries => {

        entries.forEach(entry => {

            if(entry.isIntersecting){

                entry.target.classList.add("visible");

            }

        });

    },
    {
        threshold:.12
    }
);


document.querySelectorAll(".reveal").forEach(el => {
    observer.observe(el);
});


/* =========================
   FOOD MODAL
========================= */

const modal = document.getElementById("foodModal");
const closeModal = document.getElementById("closeModal");

const modalImg = document.getElementById("modalImg");
const modalTitle = document.getElementById("modalTitle");
const modalCategory = document.getElementById("modalCategory");
const modalPrice = document.getElementById("modalPrice");
const modalDesc = document.getElementById("modalDesc");


document.querySelectorAll(".food-card").forEach(card => {

    card.addEventListener("click", () => {

        modalImg.src = card.dataset.image;
        modalTitle.textContent = card.dataset.title;
        modalCategory.textContent = card.dataset.category;
        modalPrice.textContent = card.dataset.price;
        modalDesc.textContent = card.dataset.desc;

        modal.classList.add("open");

        document.body.classList.add("loading");

    });

});


function closeFoodModal(){

    modal.classList.remove("open");
    document.body.classList.remove("loading");

}


closeModal.addEventListener("click", closeFoodModal);


modal.addEventListener("click", e => {

    if(e.target === modal){
        closeFoodModal();
    }

});


/* ESC */

document.addEventListener("keydown", e => {

    if(e.key === "Escape"){

        closeFoodModal();

        nav.classList.remove("mobile-open");

    }

});


/* =========================
   MENU FILTER
========================= */

const filters = document.querySelectorAll(".filter");
const menuItems = document.querySelectorAll(".menu-item");


filters.forEach(filter => {

    filter.addEventListener("click", () => {

        filters.forEach(btn => btn.classList.remove("active"));

        filter.classList.add("active");

        const selected = filter.dataset.filter;

        menuItems.forEach(item => {

            if(
                selected === "all" ||
                item.dataset.category === selected
            ){

                item.style.display = "grid";

            }else{

                item.style.display = "none";

            }

        });

    });

});


/* =========================
   RESERVATION
========================= */

const dateInput = document.getElementById("date");

const today = new Date();
const localDate =
    today.getFullYear() +
    "-" +
    String(today.getMonth()+1).padStart(2,"0") +
    "-" +
    String(today.getDate()).padStart(2,"0");

dateInput.min = localDate;


const form = document.getElementById("reservationForm");
const toast = document.getElementById("toast");


form.addEventListener("submit", e => {

    e.preventDefault();

    const name =
        document.getElementById("name").value.trim();

    if(!name){
        return;
    }

    toast.classList.add("show");

    form.reset();

    dateInput.min = localDate;

    setTimeout(() => {

        toast.classList.remove("show");

    },6000);

});


/* =========================
   VIDEO FALLBACK
========================= */

const video = document.querySelector(".entrance-video");

video.addEventListener("error", () => {

    video.style.display = "none";

});


/* =========================
   PARALLAX EFFECT
========================= */

window.addEventListener("scroll", () => {

    const scrolled = window.scrollY;

    if(scrolled < window.innerHeight){

        video.style.transform =
            `scale(1.08) translateY(${scrolled * .08}px)`;

    }

});


/* =========================
   REDUCED MOTION
========================= */

if(
    window.matchMedia &&
    window.matchMedia("(prefers-reduced-motion: reduce)").matches
){

    document.querySelectorAll(".reveal").forEach(el => {
        el.style.transition = "none";
        el.classList.add("visible");
    });

}

</script>

</body>
</html>
