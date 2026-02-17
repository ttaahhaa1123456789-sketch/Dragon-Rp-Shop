<!DOCTYPE html>
<html lang="fa">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>{Dragon Role play}</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:tahoma;
  scroll-behavior:smooth;
}

body {
  color: #fff;
  background:
    radial-gradient(circle at top, rgba(255, 140, 0, 0.25), transparent 40%),
    radial-gradient(circle at bottom, rgba(255, 90, 0, 0.2), transparent 40%),
    linear-gradient(135deg, #0b0602, #140900, #0b0602);
  background-attachment: fixed;
  overflow-x: hidden;
}

/* ===== Preloader ===== */
#preloader{
  position:fixed;
  width:100%;
  height:100%;
  background:#fff;
  display:flex;
  justify-content:center;
  align-items:center;
  z-index:9999;
}

.loader{
  width:60px;
  height:60px;
  border:6px solid #1E90FF;
  border-top:6px solid transparent;
  border-radius:50%;
  animation:spin 1s linear infinite;
}

@keyframes spin{
  100%{transform:rotate(360deg);}
}

/* ===== Navbar ===== */
.navbar{
  position:fixed;
  top:0;
  width:100%;
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:10px 20px;
  background: rgba(255,255,255,0.95);
  z-index:1000;
  border-radius: 0 0 15px 15px;
}

.menu-toggle{
  display:none;
  flex-direction:column;
  gap:5px;
  cursor:pointer;
}

.menu-toggle div{
  width:30px;
  height:4px;
  background:#1E90FF;
  border-radius:2px;
}

.navbar ul{
  display:flex;
  gap:20px;
  list-style:none;
}

.navbar a{
  color:#d77400;
  text-decoration:none;
  font-weight:bold;
  padding:8px 15px;
  border-radius:8px;
  transition:.3s;
}

.navbar a:hover{
  background:#1E90FF;
  color:white;
}

@media(max-width:900px){
  .menu-toggle{display:flex;}
  .navbar ul{
    display:none;
    flex-direction:column;
    background: rgba(255,255,255,0.95);
    position:absolute;
    top:60px;
    right:20px;
    padding:10px 20px;
    border-radius:8px;
  }
  .navbar ul.show{display:flex;}
}

/* ===== Hero ===== */
.hero{
  height:100vh;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  text-align:center;
}

.logo{
  color:#0effff;
  font-size:50px;
  font-weight:bold;
  text-shadow: 0 0 10px #1E90FF;
}

.btn{
  margin-top:20px;
  padding:15px 35px;
  background:#1E90FF;
  color:white;
  border-radius:15px;
  font-weight:bold;
  font-size:18px;
  box-shadow:0 0 20px #1E90FF;
}

/* ===== Sections ===== */
.section{
  padding:80px 20px;
  text-align:center;
}

/* ===== Cards ===== */
.cards{
  display:flex;
  flex-wrap:wrap;
  justify-content:center;
  gap:20px;
  margin-top:40px;
}

.card{
  padding:25px;
  border-radius:10px;
  width:250px;
  font-weight:bold;
  box-shadow: 0 0 15px rgba(0,0,0,0.1);
}

.card.owner{background:#af2d00;}
.card.scripter{background:#af2d00;}

/* ===== Gallery ===== */
.gallery-scroll{
  display:flex;
  overflow-x:auto;
  gap:20px;
  padding:20px 0;
}

.gallery-card{
  width:300px;
  border-radius:12px;
  overflow:hidden;
  box-shadow:0 0 15px rgba(0,0,0,.3);
}

.gallery-card img{width:100%;}

/* ===== Server IP ===== */
#server-ip{
  padding:25px 40px;
  background:rgba(255,140,0,.15);
  border-radius:18px;
  display:inline-block;
  box-shadow:0 0 20px rgba(255,140,0,.7);
}

footer{
  background:#FFD580;
  padding:20px;
  text-align:center;
  font-weight:bold;
  color:#1E90FF;
}
</style>
</head>

<body>

<div id="preloader">
  <div class="loader"></div>
</div>

<nav class="navbar">
  <div class="menu-toggle" id="menu-toggle">
    <div></div><div></div><div></div>
  </div>
  <ul id="nav-links">
    <li><a href="#home">خانه</a></li>
    <li><a href="#features">ویژگی‌ها</a></li>
    <li><a href="#team">مدیریت</a></li>
    <li><a href="#gallery">گالری</a></li>
    <li><a href="#server-ip">IP سرور</a></li>
    <li><a href="https://ttaahhaa1123456789-sketch.github.io/Dragon-Rp-Shop/" target="_blank">شاپ</a></li>
    <li><a href="https://ttaahhaa1123456789-sketch.github.io/Froum-DragonRp/" target="_blank">انجمن</a></li>
  </ul>
</nav>

<section id="home" class="hero">
  <h1 class="logo">DRAGON ROLEPLAY</h1>
  <h2><span id="typing"></span></h2>
  <a href="mp://127.0.0.1:7777" class="btn">🎮 Connect To Server</a>
</section>

<section id="features" class="section">
  <h2>ویژگی‌های سرور</h2>
  <div class="cards">
    <div class="card" style="background:#1E90FF;">🚓 سیستم پلیس حرفه‌ای</div>
    <div class="card" style="background:#32CD32;">🏢 گتو و مافیا</div>
    <div class="card" style="background:#FFD700;">💰 اقتصاد واقعی</div>
    <div class="card" style="background:#FF69B4;">🏎 ماشین‌های سفارشی</div>
  </div>
</section>

<section id="team" class="section">
  <h2>تیم مدیریت</h2>
  <div class="cards">
    <div class="card owner">👑 Owner: Mr_Taha</div>
    <div class="card scripter">🛡 Scripter: Kurdx</div>
  </div>
</section>

<section id="gallery" class="section">
  <h2>گالری سرور</h2>
  <div class="gallery-scroll">
    <div class="gallery-card"><img src="https://via.placeholder.com/400x250"></div>
    <div class="gallery-card"><img src="https://via.placeholder.com/400x250"></div>
    <div class="gallery-card"><img src="https://via.placeholder.com/400x250"></div>
  </div>
</section>

<center>
<section id="server-ip">
  <h2>IP سرور</h2>
  <span>127.0.0.1:7777</span>
</section>
</center>

<footer>
  Tavsot Tim Dragon Rp | @DraGon_RolePlay | @Mashin_Mazndarn
</footer>

<script>
window.addEventListener("load",()=>{document.getElementById("preloader").style.display="none"});

const menuToggle=document.getElementById('menu-toggle');
const navLinks=document.getElementById('nav-links');
menuToggle.onclick=()=>navLinks.classList.toggle('show');

const text="به بهترین سرور،دراگون رول پلی خوش آمدید";
let i=0;
(function typing(){
  if(i<text.length){
    document.getElementById("typing").innerHTML+=text.charAt(i++);
    setTimeout(typing,60);
  }
})();
</script>

</body>
</html>
