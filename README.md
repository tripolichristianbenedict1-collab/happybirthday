<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Birthday Sister Raine 💗</title>

  <style>
    @import url('https://fonts.googleapis.com/css2?family=Pacifico&family=Poppins:wght@300;400;600;700&display=swap');

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: #0b0618;
      color: white;
      overflow-x: hidden;
    }

    /* Animated background */
    body::before {
      content: "";
      position: fixed;
      inset: 0;
      background:
        radial-gradient(circle at 20% 20%, #6b21a855, transparent 35%),
        radial-gradient(circle at 80% 70%, #db277755, transparent 35%);
      animation: backgroundMove 10s ease-in-out infinite alternate;
      z-index: -2;
    }

    @keyframes backgroundMove {
      from { transform: scale(1); }
      to { transform: scale(1.25); }
    }

    /* Navigation */
    nav {
      position: fixed;
      top: 15px;
      left: 5%;
      width: 90%;
      padding: 15px 25px;
      border: 1px solid #d8b4fe55;
      border-radius: 50px;
      background: #17102dcc;
      backdrop-filter: blur(12px);
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 100;
    }

    .logo {
      font-family: 'Pacifico', cursive;
      font-size: 20px;
      color: #f5b8ff;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
      font-size: 13px;
      transition: 0.3s;
    }

    nav a:hover {
      color: #f0abfc;
    }

    /* Hero section */
    .hero {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 100px 20px 50px;
    }

    .hero h1 {
      font-family: 'Pacifico', cursive;
      font-size: clamp(40px, 7vw, 80px);
      color: #f5c2ff;
      text-shadow: 0 0 20px #d946ef;
      animation: glow 2s ease-in-out infinite alternate;
    }

    .hero p {
      font-size: 18px;
      margin-top: 15px;
      color: #e9d5ff;
    }

    @keyframes glow {
      from { text-shadow: 0 0 10px #d946ef; }
      to { text-shadow: 0 0 35px #f0abfc; }
    }

    .btn {
      margin-top: 30px;
      padding: 14px 28px;
      border: none;
      border-radius: 30px;
      background: linear-gradient(135deg, #d946ef, #8b5cf6);
      color: white;
      font-size: 15px;
      font-weight: bold;
      cursor: pointer;
      box-shadow: 0 0 20px #c026d355;
      transition: 0.3s;
    }

    .btn:hover {
      transform: scale(1.08);
      box-shadow: 0 0 35px #e879f9;
    }

    /* Floating decorations */
    .floating {
      position: fixed;
      bottom: -50px;
      font-size: 25px;
      animation: floatUp linear infinite;
      pointer-events: none;
      z-index: -1;
    }

    @keyframes floatUp {
      0% {
        transform: translateY(0) rotate(0deg);
        opacity: 0;
      }
      15% { opacity: 1; }
      100% {
        transform: translateY(-110vh) rotate(360deg);
        opacity: 0;
      }
    }

    /* Sections */
    section {
      padding: 80px 20px;
      text-align: center;
    }

    .section-title {
      font-family: 'Pacifico', cursive;
      color: #f0abfc;
      font-size: 35px;
      margin-bottom: 35px;
    }

    .card {
      max-width: 750px;
      margin: auto;
      padding: 35px;
      border-radius: 25px;
      background: #ffffff0d;
      border: 1px solid #f0abfc33;
      backdrop-filter: blur(10px);
      box-shadow: 0 0 30px #a855f722;
      animation: fadeIn 1.5s ease;
    }

    .card p {
      line-height: 2;
      color: #f3e8ff;
      font-size: 16px;
    }

    /* Photo gallery */
    .gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 25px;
    }

    .photo {
      width: 260px;
      height: 280px;
      padding: 12px;
      background: #fff;
      color: #30104b;
      transform: rotate(-3deg);
      transition: 0.5s;
      box-shadow: 0 10px 30px #0005;
    }

    .photo:nth-child(2) {
      transform: rotate(4deg);
    }

    .photo:hover {
      transform: rotate(0deg) scale(1.08);
    }

    .photo img {
      width: 100%;
      height: 215px;
      object-fit: cover;
    }

    .photo p {
      font-family: 'Pacifico', cursive;
      margin-top: 8px;
      font-size: 14px;
    }

    /* Reasons cards */
    .reasons {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
    }

    .reason {
      width: 220px;
      padding: 25px;
      border-radius: 20px;
      background: #ffffff0d;
      border: 1px solid #f0abfc33;
      transition: 0.4s;
    }

    .reason:hover {
      transform: translateY(-10px);
      background: #c026d422;
    }

    .reason span {
      font-size: 35px;
    }

    .reason h3 {
      color: #f5d0fe;
      margin: 12px 0;
    }

    .reason p {
      font-size: 13px;
      color: #ddd6fe;
    }

    /* Surprise message */
    #surprise {
      display: none;
      margin: 25px auto;
      max-width: 600px;
      padding: 25px;
      background: #d946ef22;
      border: 1px solid #f0abfc66;
      border-radius: 20px;
      animation: popIn 0.7s ease;
    }

    #surprise p {
      line-height: 2;
      color: #fce7f3;
    }

    @keyframes popIn {
      from {
        opacity: 0;
        transform: scale(0.5);
      }
      to {
        opacity: 1;
        transform: scale(1);
      }
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(30px); }
      to { opacity: 1; transform: translateY(0); }
    }

    footer {
      padding: 35px;
      text-align: center;
      color: #d8b4fe;
      font-size: 14px;
    }

    @media (max-width: 600px) {
      nav {
        padding: 12px 15px;
      }

      nav a {
        margin-left: 8px;
        font-size: 10px;
      }

      .logo {
        font-size: 15px;
      }

      .hero p {
        font-size: 14px;
      }

      .card {
        padding: 25px 18px;
      }
    }
  </style>
</head>

<body>

  <!-- Navigation -->
  <nav>
    <div class="logo">💗 Raine Day</div>
    <div>
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#memories">Memories</a>
    </div>
  </nav>

  <!-- Hero -->
  <section class="hero" id="home">
    <div style="font-size: 35px;">💖 ✨ 🦋 ✨ 💖</div>

    <h1>Happy Birthday Sister Raine!</h1>

    <p id="typing"></p>

    <button class="btn" onclick="showSurprise()">
      💌 Open Your Surprise
    </button>

    <div id="surprise">
      <p>
        Happy Bithday Teh. 💗
        <br><br>
        All I can say is always remember that we're here if you need help. Also, do not pressure yourself; just do what you can, and that's enough. Don't you ever think that it's not enough. Love lots!🥹💕
      </p>
    </div>
  </section>

  <!-- About -->
  <section id="about">
    <h2 class="section-title">To My Sister 💌</h2>

    <div class="card">
      <p>
        Having a friend like you is one of the best things
        that ever happened to me. You are someone I can laugh with,
        talk to, play codm, and many more.
        <br><br>
        We're may not even by your side, and sometimes we get busy,
        but I hope you always know how much you mean to us.
        Thank you for being yourself. You are truly special to us. Alam mo yan teh.💕
      </p>
    </div>
  </section>

  <!-- Memories -->
  <section id="memories">
    <h2 class="section-title">Our Memories 📸</h2>

    <div class="gallery">
      <div class="photo">
        <!-- Replace photo1.jpg with your picture -->
        <img src="withme.jpg" alt="Our photo">
        <p>Best memories 💗</p>
      </div>

      <div class="photo">
        <!-- Replace photo2.jpg with your picture -->
        <img src="withthem.jpg" alt="Another photo">
        <p>Peak memories 💗</p>
      </div>

      <div class="photo">
        <!-- Replace photo3.jpg with your picture -->
        <img src="withmch.jpg" alt="With MCH!">
        <p>Always us 💗</p>
      </div>
    </div>
  </section>

  <!-- Reasons -->
  <section>
    <h2 class="section-title">T, I, T, E</h2>

    <div class="reasons">
      <div class="reason">
        <span>😂</span>
        <h3>Tranquility</h3>
        <p>i-search nalang ang meaning teh, napapagod nako mag english huhu</p>
      </div>

      <div class="reason">
        <span>🤍</span>
        <h3>Isolation</h3>
        <p>College. Self-explanatory. I hate college :( </p>
      </div>

      <div class="reason">
        <span>🌟</span>
        <h3>Togetherness</h3>
        <p>Teh kahit san talaga mapunta, basta magkakasama, eyyy</p>
      </div>

      <div class="reason">
        <span>🫶</span>
        <h3>Eternal</h3>
        <p>Eternal Beauty? Any-any nalang talaga AHHAHAHHA</p>
      </div>
    </div>
  </section>

  <footer>
    Ginawa ng pinaka masarap, maganda, at higit sa lahat, wala, ganda lang :p 💗<br>
    Lovelots! ✨
  </footer>

  <!-- Floating hearts and stars -->
  <script>
    const symbols = ["💗", "💖", "✨", "💕", "🦋", "🌸", "⭐"];

    function createFloating() {
      const item = document.createElement("div");
      item.className = "floating";
      item.textContent =
        symbols[Math.floor(Math.random() * symbols.length)];

      item.style.left = Math.random() * 100 + "vw";
      item.style.animationDuration =
        (5 + Math.random() * 7) + "s";
      item.style.fontSize =
        (15 + Math.random() * 20) + "px";

      document.body.appendChild(item);

      setTimeout(() => item.remove(), 13000);
    }

    setInterval(createFloating, 500);

    // Typewriter effect
    const message =
      "Different paths, same soul. Grateful for you, always. 💕";

    let index = 0;

    function typeWriter() {
      if (index < message.length) {
        document.getElementById("typing").textContent +=
          message.charAt(index);
        index++;
        setTimeout(typeWriter, 65);
      }
    }

    typeWriter();

    // Surprise button
    function showSurprise() {
      const surprise = document.getElementById("surprise");

      if (surprise.style.display === "block") {
        surprise.style.display = "none";
      } else {
        surprise.style.display = "block";
        surprise.scrollIntoView({
          behavior: "smooth",
          block: "center"
        });
      }
    }
  </script>

</body>
</html>
