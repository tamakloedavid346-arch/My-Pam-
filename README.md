# My-Pam-
Vals
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Be My Valentine 💘</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Arial', sans-serif;
    }

    body {
      height: 100vh;
      background: url('background.jpg') no-repeat center center/cover;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .overlay {
      background: rgba(0, 0, 0, 0.55);
      padding: 30px 40px;
      border-radius: 15px;
      text-align: center;
      color: white;
    }

    h1 {
      margin-bottom: 25px;
      font-size: 2.2rem;
    }

    button {
      font-size: 1.1rem;
      padding: 10px 25px;
      margin: 10px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      transition: transform 0.2s;
    }

    .yes {
      background-color: #ff4d6d;
      color: white;
    }

    .no {
      background-color: #cccccc;
      color: black;
      position: relative;
    }

    button:hover {
      transform: scale(1.1);
    }
  </style>
</head>
<body>

  <div class="overlay">
    <h1>Will you be my Valentine? 💖</h1>
    <button class="yes" onclick="yesClicked()">Yes</button>
    <button class="no" onmouseover="moveNo()">No</button>
  </div>

  <script>
    function yesClicked() {
      alert("YAY!! 💕 I knew you'd say yes 😍");
    }

    function moveNo() {
      const button = document.querySelector('.no');
      const x = Math.random() * 200 - 100;
      const y = Math.random() * 200 - 100;
      button.style.transform = translate(${x}px, ${y}px);
    }
  </script>

</body>
</html>
