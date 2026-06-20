<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Cartão que Vira</title>

<style>
body{
  margin:0;
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  background:#f2f2f2;
}

.card{
  width:350px;
  height:250px;
  position:relative;
  transform-style:preserve-3d;
  transition:transform 0.8s;
  cursor:pointer;
}

.card.flip{
  transform:rotateY(180deg);
}

.face{
  position:absolute;
  width:100%;
  height:100%;
  backface-visibility:hidden;
  border-radius:20px;
  overflow:hidden;
}

.face img{
  width:100%;
  height:100%;
  object-fit:cover;
}

.back{
  transform:rotateY(180deg);
}
</style>
</head>

<body>

<div class="card" id="card">
  <div class="face">
    <img src="frente.jpg">
  </div>

  <div class="face back">
    <img src="verso.jpg">
  </div>
</div>

<script>
document.getElementById('card').onclick = function() {this.classList.toggle('flip');}
</script>

</body>
</html>
 <img width="1050" height="600" alt="image" src="https://github.com/user-attachments/assets/48e733c0-3716-41ca-9d68-1faa2a310204" />
<img width="525" height="300" alt="image" src="https://github.com/user-attachments/assets/5fbc6598-e80e-441a-a7e8-05f8df01cf25" />
