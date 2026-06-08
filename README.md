<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Profile</title>

<style>
body{
margin:0;
font-family:Arial;
background:#111;
color:white;
overflow-x:hidden;
}

.bg-wrap{
position:absolute;
top:0;left:0;
width:100%;
height:220px;
overflow:hidden;
z-index:-1;
}
.bg-wrap img{
width:100%;
height:100%;
object-fit:cover;
filter:brightness(.7);
}
.bg-fade{
position:absolute;
bottom:0;
width:100%;
height:100px;
background:linear-gradient(to bottom,transparent,#111);
}

.header{
text-align:center;
padding:25px;
}
.profile-img{
width:110px;
height:110px;
border-radius:50%;
border:3px solid #00c300;
object-fit:cover;
box-shadow:0 0 15px #00c30055;
}
.name{
font-size:22px;
margin-top:12px;
font-weight:bold;
}

.content{
padding:10px;
}

.post{
background:#1a1a1a;
border-radius:16px;
margin:18px auto;
padding:12px;
max-width:360px;
box-shadow:0 4px 15px rgba(0,0,0,.35);
}

.slider{
display:flex;
overflow-x:auto;
gap:10px;
scroll-snap-type:x mandatory;
scroll-behavior:smooth;
}
.slider::-webkit-scrollbar{
display:none;
}
.slider img{
width:100%;
border-radius:12px;
flex-shrink:0;
scroll-snap-align:center;
}

.caption{
margin-top:10px;
font-size:14px;
}

.actions{
display:flex;
gap:18px;
margin-top:10px;
font-size:20px;
}

.action{
cursor:pointer;
transition:.2s;
user-select:none;
}
.action:hover{
transform:scale(1.15);
}

.like.active{
color:red;
}
.repost.active{
color:#00c300;
}

.stats{
font-size:13px;
color:#aaa;
margin-top:6px;
}

.comment{
font-size:13px;
margin-top:8px;
padding:8px;
background:#222;
border-radius:10px;
}

.comment-name{
font-weight:bold;
color:white;
}

.comment-text{
color:#bbb;
margin-left:5px;
}
</style>
</head>
<body>

<div class="bg-wrap">
<img src="https://i.pinimg.com/originals/7d/07/a2/7d07a255678962d30d8717dcf5dbd266.gif">
<div class="bg-fade"></div>
</div>

<div class="header">
<img class="profile-img" src="https://i.postimg.cc/MHMYx07M/TA-2026-04-04-14-18-57.png">
<div class="name">ลีออนรักเมีย</div>
</div>

<div class="content">

<div class="post">
<div class="slider">
<img src="https://i.postimg.cc/HLVrxHS6/ad6031d9d390662fd70b3ddc1df32d64.jpg">
<img src="https://i.postimg.cc/dVm0V3mN/ff2eba32.png">
</div>

<div class="caption">เมียสวยมีชัยไปกว่าครึ่ง</div>

<div class="actions">
<span class="action like" onclick="toggle(this)">❤</span>
<span class="action">💬</span>
<span class="action repost" onclick="toggle(this)">🔁</span>
</div>

<div class="stats">❤️ <span>12.4K</span> · 💬 3.1K · 🔁 <span>1.2K</span></div>

<div class="comment">
<span class="comment-name">ฝันร้ายแรงค์แกรน</span>
<span class="comment-text">โคตรสวยหมายถึงเมียพี่</span>
</div>

<div class="comment">
<span class="comment-name">แว่นอย่าทิ้งเค้า</span>
<span class="comment-text">ฟิลกู๊ล</span>
</div>
</div>

</div>

<script>
function toggle(el){
el.classList.toggle("active");
}
</script>

</body>
</html>
