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

.face img{<img width="1050" height="600" alt="image" src="https://github.com/user-attachments/assets/f302b312-d49e-47dd-b40a-2730e856ac0e" />

  width:100%;
  height:100%;
  object-fit:cover;
}

.back{<img width="525" height="300" alt="image" src="https://github.com/user-attachments/assets/cb322a13-d631-4284-80ec-abd75f977d90" />

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
document.getElementById('card').onclick = function() {
  this.classList.toggle('flip');
}
</script>

</body>
</html>
