# shohadaa-mawfakia-
<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>شهداء قضاء الموفقية</title>

<style>

body{
font-family: Arial;
background:#111;
color:white;
margin:0;
text-align:center;
}

header{
background:#000;
padding:20px;
}

h1{
color:gold;
}

.search{
margin:20px;
}

input{
padding:10px;
width:250px;
}

.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
gap:20px;
padding:20px;
}

.card{
background:#222;
padding:10px;
border-radius:10px;
cursor:pointer;
}

.card img{
width:100%;
border-radius:10px;
}

.name{
margin-top:10px;
font-size:18px;
}

footer{
margin-top:40px;
opacity:0.5;
}

</style>

</head>

<body>

<header>

<h1>مضيف شهداء الموفقية</h1>

<div class="search">
<input type="text" id="search" placeholder="ابحث عن شهيد..." onkeyup="search()">
</div>

</header>

<div class="grid" id="martyrs">

<div class="card">
<img src="https://via.placeholder.com/200">
<div class="name">شهيد 1</div>
</div>

<div class="card">
<img src="https://via.placeholder.com/200">
<div class="name">شهيد 2</div>
</div>

<div class="card">
<img src="https://via.placeholder.com/200">
<div class="name">شهيد 3</div>
</div>

</div>

<footer>

<p>المبرمج: منتظر لفته البدري</p>

</footer>

<script>

function search(){

let input=document.getElementById("search").value.toLowerCase();
let cards=document.getElementsByClassName("card");

for(let i=0;i<cards.length;i++){

let name=cards[i].innerText.toLowerCase();

if(name.includes(input)){
cards[i].style.display="block";
}else{
cards[i].style.display="none";
}

}

}

</script>

</body>
</html>
