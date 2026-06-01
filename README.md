<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>JIANG WEI Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@200;300;400;600;700&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{

font-family:'Inter',sans-serif;
background:#050505;
color:white;
overflow-x:hidden;

}

/* 背景动态光 */

.bg{

position:fixed;
width:100%;
height:100%;
top:0;
left:0;
z-index:-2;

background:
radial-gradient(circle at 20% 30%,rgba(255,255,255,.12),transparent 40%),
radial-gradient(circle at 80% 70%,rgba(120,120,255,.12),transparent 40%),
#050505;

animation:move 10s ease-in-out infinite alternate;

}

@keyframes move{

0%{
transform:scale(1);
}

100%{
transform:scale(1.2);
}

}

/* noise */

body::after{

content:'';

position:fixed;

top:0;
left:0;

width:100%;
height:100%;

background-image:url('https://grainy-gradients.vercel.app/noise.svg');

opacity:.03;

pointer-events:none;

z-index:-1;

}

/* hero */

.hero{

height:100vh;

display:flex;

justify-content:center;

align-items:center;

padding:80px;

}

.content{

max-width:1200px;

width:100%;

}

.cn{

font-size:18px;

opacity:0;

animation:fadeUp 1.8s ease forwards;

animation-delay:.6s;

letter-spacing:4px;

color:#9e9e9e;

margin-bottom:30px;

}

h1{

font-size:110px;

font-weight:700;

line-height:0.9;

letter-spacing:-6px;

opacity:0;

animation:fadeUp 1.5s ease forwards;

}

h2{

font-size:28px;

font-weight:300;

margin-top:20px;

letter-spacing:10px;

color:#8f8f8f;

opacity:0;

animation:fadeUp 1.6s ease forwards;

animation-delay:.2s;

}

.tagline{

margin-top:40px;

font-size:20px;

font-weight:300;

max-width:600px;

line-height:1.9;

color:#bfbfbf;

opacity:0;

animation:fadeUp 2s ease forwards;

animation-delay:1s;

}

.highlight{

color:white;

font-weight:600;

}

/* scroll */

.scroll{

position:absolute;

bottom:50px;

left:50%;

transform:translateX(-50%);

font-size:13px;

letter-spacing:5px;

opacity:.4;

animation:float 2s infinite;

}

@keyframes float{

0%{
transform:translate(-50%,0);
}

50%{
transform:translate(-50%,10px);
}

100%{
transform:translate(-50%,0);
}

}

@keyframes fadeUp{

from{

opacity:0;

transform:translateY(60px);

}

to{

opacity:1;

transform:translateY(0);

}

}

/* section */

.section{

padding:160px 10%;

display:flex;

justify-content:space-between;

align-items:flex-start;

gap:100px;

}

.section-title{

font-size:16px;

letter-spacing:5px;

color:#7a7a7a;

}

.section-text{

font-size:42px;

line-height:1.5;

max-width:900px;

font-weight:300;

}

.section-text span{

font-weight:600;

}

/* responsive */

@media(max-width:900px){

h1{

font-size:64px;

}

.section{

flex-direction:column;
}

.section-text{

font-size:28px;

}

}

</style>
</head>
<body>

<div class="bg"></div>

<section class="hero">

<div class="content">

<div class="cn">

个人创作 / 视觉设计 / 绘画表达

</div>

<h1>

姜惟

</h1>

<h2>

JIANG WEI

</h2>

<div class="tagline">

Personal Creative Portfolio.

Exploring the intersection of

<span class="highlight">

drawing, visual storytelling and experimental design.

</span>

以视觉记录情绪、想法与未完成的世界。

</div>

</div>

<div class="scroll">

SCROLL

</div>

</section>

<section class="section">

<div class="section-title">

ABOUT

</div>

<div class="section-text">

我专注于

<span>画画、创作与视觉设计。</span>

喜欢在极简结构中保留情绪感，

让图像、排版与光影形成一种安静但具有张力的表达。

</div>

</section>

<section class="section">

<div class="section-title">

PHILOSOPHY

</div>

<div class="section-text">

Minimal.

Dark.

Emotional.

Creating visual experiences that feel

<span>

cinematic, silent and alive.

</span>

</div>

</section>

</body>
</html>
