<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Valentine 💖</title>

<style>
  body {
    height: 100vh;
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(135deg, #ff9a9e, #fad0c4);
    font-family: 'Poppins', sans-serif;
    overflow: hidden;
  }

  .card {
    background: white;
    padding: 30px;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 10px 30px rgba(0,0,0,0.2);
    animation: pop 1s ease;
  }

  @keyframes pop {
    from { transform: scale(0.5); opacity: 0; }
    to { transform: scale(1); opacity: 1; }
  }

  h1 {
    color: #ff4d6d;
    margin-bottom: 20px;
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
    background: #ccc;
    position: absolute;
  }
</style>
</head>

<body>

<div class="card">
  <h1>Will you be my Valentine? 💘</h1>
  <button id="yes">Yes 💖</button>
  <button id="no">No 🙈</button>
</div>

<script>
  const noBtn = document.getElementById("no");

  noBtn.addEventListener("mouseover", moveNo);
  noBtn.addEventListener("touchstart", moveNo);

  function moveNo() {
    const x = Math.random() * (window.innerWidth - 120);
    const y = Math.random() * (window.innerHeight - 60);
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
  }

  document.getElementById("yes").onclick = () => {
    window.location.href =
      "https://wa.me/?text=Yes%20baby%20💖%20I%27ll%20be%20your%20Valentine%20😍";
  };
</script>

</body>
</html># HOZA
TO YOU
