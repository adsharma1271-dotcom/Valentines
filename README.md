# Valentines
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Be My Valentine 💖</title>
  <style>
    body {
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      font-family: 'Comic Sans MS', cursive;
      text-align: center;
      height: 100vh;
      margin: 0;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .box {
      background: white;
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
      max-width: 350px;
    }

    h1 {
      color: #ff4d6d;
    }

    button {
      padding: 12px 25px;
      font-size: 18px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      margin: 10px;
    }

    #yes {
      background: #ff4d6d;
      color: white;
    }

    #no {
      background: #adb5bd;
      color: white;
      position: relative;
    }

    video {
      width: 100%;
      border-radius: 15px;
      margin-top: 15px;
    }
  </style>
</head>
<body>

<div class="box" id="content">
  <h1>Will you be my Valentine? 💘</h1>
  <button id="yes" onclick="showLove()">Yes 💖</button>
  <button id="no" onmouseover="moveNo()">No 🙄</button>
</div>

<script>
  function showLove() {
    document.getElementById("content").innerHTML = `
      <h1>YAYYY 🥹💞</h1>
      <p>I knew it 😌💖</p>
      <video autoplay loop controls>
        <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4">
      </video>
      <p>Happy Valentine’s Day, my love 🌹</p>
    `;
  }

  function moveNo() {
    const noBtn = document.getElementById("no");
    noBtn.style.left = Math.random() * 200 - 100 + "px";
    noBtn.style.top = Math.random() * 200 - 100 + "px";
  }
</script>

</body>
</html>
