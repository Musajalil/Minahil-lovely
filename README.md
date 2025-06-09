# Minahil-lovely
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>To My Love Minahil 💖</title>
  <style>
    body {
      margin: 0;
      background: linear-gradient(to bottom right, #ffe6f0, #ffe0ec);
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      color: #ff4081;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      overflow: hidden;
    }

    h1 {
      font-size: 3em;
      animation: glow 2s ease-in-out infinite alternate;
    }

    @keyframes glow {
      from {
        text-shadow: 0 0 10px #ff99c8, 0 0 20px #ff5eaa;
      }
      to {
        text-shadow: 0 0 20px #ff1493, 0 0 30px #ff1493;
      }
    }

    .message {
      font-size: 1.5em;
      text-align: center;
      max-width: 600px;
      margin: 20px;
      animation: fadeIn 2s ease-in;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .heart {
      position: absolute;
      width: 20px;
      height: 20px;
      background: #ff1493;
      transform: rotate(45deg);
      animation: float 6s linear infinite;
    }

    .heart::before,
    .heart::after {
      content: '';
      position: absolute;
      width: 20px;
      height: 20px;
      background: #ff1493;
      border-radius: 50%;
    }

    .heart::before {
      top: -10px;
      left: 0;
    }

    .heart::after {
      left: -10px;
      top: 0;
    }

    @keyframes float {
      0% {
        transform: translateY(0) rotate(45deg);
        opacity: 1;
      }
      100% {
        transform: translateY(-100vh) rotate(45deg);
        opacity: 0;
      }
    }
  </style>
</head>
<body>

  <h1>To My Beautiful Minahil 💗</h1>
  <div class="message">
    Every moment with you feels like a dream come true.<br>
    Your smile lights up my world brighter than the stars. 🌟<br><br>
    I am so lucky to have your love, your heart, your soul...<br>
    You're not just in my heart — you are my heart. ❤️<br><br>
    I love you endlessly, Minahil. Forever and always. 💞
  </div>

  <!-- Floating hearts -->
  <script>
    function createHeart() {
      const heart = document.createElement('div');
      heart.className = 'heart';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = (3 + Math.random() * 3) + 's';
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 6000);
    }

    setInterval(createHeart, 300);
  </script>

</body>
</html>
