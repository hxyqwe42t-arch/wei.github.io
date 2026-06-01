<!DOCTYPE html>
<html lang="zh">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>姜惟 | Personal Website</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
scroll-behavior:smooth;
}

body{
background:#050505;
color:#fff;
overflow-x:hidden;
}

body::before{
content:"";
position:fixed;
inset:0;
background:
radial-gradient(
circle at var(--x) var(--y),
rgba(255,255,255,.12),
transparent 28%
);
pointer-events:none;
}

nav{
position:fixed;
top:0;
width:100%;
display:flex;
justify-content:space-between;
padding:30px 60px;
z-index:999;
backdrop-filter:blur(12px);
}

.logo{
font-size:22px;
letter-spacing:5px;
font-weight:700;
}

nav ul{
display:flex;
gap:35px;
list-style:none;
}

nav a{
text-decoration:none;
color:white;
opacity:.7;
transition:.3s;
}

nav a:hover{
opacity:1;
}

.hero{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
}

.name{
font-size:1rem;
letter-spacing:8px;
color:#8f8f8f;
margin-bottom:15px;
}

.hero h1{

font-size:7rem;
line-height:1;
letter-spacing:10px;
text-transform:uppercase;

background:linear-gradient(
90deg,
#ffffff,
#888,
#ffffff
);

-webkit-background-clip:text;
-webkit-text-fill-color:transparent;

animation:fadeUp 1s ease;
}

.hero p{
margin-top:25px;
font-size:1.1rem;
color:#aaa;
max-width:720px;
line-height:1.8;
}

.btn{

margin-top:45px;
padding:16px 38px;

background:transparent;
border:1px solid #fff;

color:white;

cursor:pointer;
transition:.35s;
}

.btn:hover{

background:white;
color:black;
transform:translateY(-4px);

}

section{
padding:140px 10%;
}

.section-title{
font-size:3rem;
margin-bottom:70px;
}

.cards{

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(280px,1fr));

gap:30px;
}

.card{

background:#111;
padding:40px;
border:1px solid #222;
border-radius:22px;

transition:.4s;
}

.card:hover{

transform:translateY(-10px);
border-color:#777;

box-shadow:
0 0 30px rgba(255,255,255,.08);

}

.card h3{

margin-bottom:18px;
letter-spacing:3px;

}

.card p{
color:#b9b9b9;
line-height:1.7;
}

footer{

padding:70px;
text-align:center;
color:#666;

}

@keyframes fadeUp{

from{
opacity:0;
transform:translateY(50px);
}

to{
opacity:1;
transform:translateY(0);
}

}

@media(max-width:768px){

.hero h1{
font-size:3.5rem;
}

nav{
padding:25px;
}

nav ul{
display:none;
}

}

</style>
</head>

<body>

<nav>

<div class="logo">
姜惟
</div>

<ul>

<li><a href="#about">ABOUT</a></li>
<li><a href="#work">WORK</a></li>
<li><a href="#contact">CONTACT</a></li>

</ul>

</nav>

<section class="hero">

<div class="name">
JIANG WEI
</div>

<h1>
ASK<br>THE<br>SPIDER
</h1>

<p>

你好，我是姜惟。

插画、设计、创意表达、视觉实验。

我喜欢把想法做成画面，把情绪藏进颜色、线条和网页里。

这里不是普通主页。

这是我的个人宇宙。

</p>

<button class="btn">
ENTER MY WORLD
</button>

</section>

<section id="about">

<h2 class="section-title">
ABOUT ME
</h2>

<div class="cards">

<div class="card">

<h3>ILLUSTRATION</h3>

<p>
喜欢画画、角色设计、氛围感视觉。
把脑子里的世界一点点拖出来落地。
</p>

</div>

<div class="card">

<h3>DESIGN</h3>

<p>
极简、暗色、未来感、实验风格。
让视觉看起来像深夜偷偷长出来的东西。
</p>

</div>

<div class="card">

<h3>CREATION</h3>

<p>
网站、视觉、创意表达。
持续制造一些无法被简单定义的作品。
</p>

</div>

</div>

</section>

<section id="work">

<h2 class="section-title">
PROJECTS
</h2>

<div class="cards">

<div class="card">

<h3>VOID</h3>

<p>
个人视觉实验项目。
</p>

</div>

<div class="card">

<h3>NEON DREAM</h3>

<p>
未来感网页概念设计。
</p>

</div>

<div class="card">

<h3>JIANG WEI LAB</h3>

<p>
插画 / UI / 创意探索空间。
</p>

</div>

</div>

</section>

<footer id="contact">

© 2026 姜惟 Personal Website

</footer>

<script>

document.addEventListener("mousemove",(e)=>{

document.body.style.setProperty(
"--x",
e.clientX+"px"
);

document.body.style.setProperty(
"--y",
e.clientY+"px"
);

})

</script>

</body>
</html>
