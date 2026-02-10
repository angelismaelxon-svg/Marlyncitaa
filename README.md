# Marlyncitaa
Tarjeta San Valentín 
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>San Valentín 💖</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background: linear-gradient(135deg, #ff758c, #ff7eb3);
      height: 100vh;
      margin: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
    }
    .card {
      background: white;
      padding: 35px;
      border-radius: 25px;
      box-shadow: 0 15px 40px rgba(0,0,0,0.3);
      width: 300px;
    }
    h1 {
      margin-bottom: 30px;
    }
    .yes {
      font-size: 36px;
      padding: 22px 55px;
      background: #ff2e63;
      color: white;
      border: none;
      border-radius: 18px;
      cursor: pointer;
      margin-bottom: 25px;
    }
    .no {
      font-size: 14px;
      padding: 6px 12px;
      background: #ccc;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      position: absolute;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>¿Quieres ser mi San Valentín? 💘</h1>
    <button class="yes" onclick="sayYes()">SÍ 💖</button>
  </div>

  <button class="no" id="no">no</button>

  <script>
    const noBtn = document.getElementById("no");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * (window.innerWidth - 100);
      const y = Math.random() * (window.innerHeight - 50);
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    });

    function sayYes() {
      window.location.href =
        "https://wa.me/?text=💖%20Acepto%20ser%20tu%20San%20Valentín%20😍";
    }
  </script>
</body>
</html>
