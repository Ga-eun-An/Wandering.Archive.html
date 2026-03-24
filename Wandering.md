<!DOCTYPE html>

<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link href="https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@300;400;700&display=swap" rel="stylesheet">

<style>
img:hover {
  opacity: 0.8;
}

body{
  font-family: "Roboto Condensed", sans-serif;
  letter-spacing: -0.01em;
  margin: 40px;
}

* {cursor:none;}

.cursor {
  position: fixed;
  width: 60px;
  height: 60px;
  background: yellow;
  border-radius: 50%;
  pointer-events: none;
  transform: translate(-50%, -50%);
  z-index: 9999;
}
.cursor.click {
  transform: translate(-50%, -50%) scale(0.7);
}

h1{
  font-size: 40px;
  margin-bottom: 5px;
}
h2{
  font-size: 30px;
  margin-top: 0px;
  font-weight: 400;
}
</style>

</head>

<body>

<h1><a href="Wandering Archive.html">Wandering Archive / publications</a></h1>
<h2>A Random Archive by Gayeong An, Gaeun An</h2>

<img src="London.png" width="15%">
<img src="peachshadow.png" width="20%">
<img src="comte.png" width="20%">
<img src="IMG_9213.png" width="20%">
<img src="IMG_1139.png" width="20%">
<img src="먼로.png" width="13%">


<div class="ball"></div>
<div class="cursor"></div>

<script>
const cursor=document.querySelector(".cursor");

document.addEventListener("mousemove",(e)=>{
cursor.style.left=e.clientX+"px";
cursor.style.top=e.clientY+"px";
});

document.addEventListener("mousedown",()=>{
cursor.classList.add("click");
});

document.addEventListener("mouseup",()=>{
cursor.classList.remove("click");
});
</script>

</body>

</html>
