<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>About Me</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Quicksand:wght@400;600&display=swap');

    body {
      font-family: 'Quicksand', sans-serif;
      background: url('https://images.unsplash.com/photo-1529676468690-d14f2f3ec0a5?auto=format&fit=crop&w=1350&q=80') no-repeat center center fixed;
      background-size: cover;
      margin: 0;
      padding: 0;
      position: relative;
      overflow-x: hidden;
    }
    .overlay {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background-color: rgba(255, 255, 255, 0.6);
      z-index: 0;
    }
    .container {
      max-width: 900px;
      margin: 60px auto;
      background: rgba(255, 255, 255, 0.95);
      border-radius: 20px;
      box-shadow: 0 12px 30px rgba(0,0,0,0.1);
      padding: 50px;
      transition: transform 0.3s ease-in-out;
      border: 1px solid #ddd;
      position: relative;
      z-index: 1;
    }
    .container:hover {
      transform: scale(1.02);
    }
    h1 {
      text-align: center;
      color: #cc3366;
      font-size: 40px;
      margin-bottom: 10px;
      animation: fadeInDown 1s ease-out;
      letter-spacing: 1px;
    }
    @keyframes fadeInDown {
      from {
        opacity: 0;
        transform: translateY(-30px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
    img {
      display: block;
      margin: 25px auto;
      width: 160px;
      height: 160px;
      border-radius: 50%;
      object-fit: cover;
      transition: transform 0.4s ease, box-shadow 0.4s ease;
      border: 4px solid #fff;
      box-shadow: 0 4px 15px rgba(0,0,0,0.2);
    }
    img:hover {
      transform: scale(1.1);
      box-shadow: 0 10px 25px rgba(0,0,0,0.3);
    }
    p {
      font-size: 18px;
      line-height: 1.8;
      color: #444;
      margin: 15px 0;
    }
    .section-title {
      font-size: 26px;
      color: #cc3366;
      margin-top: 50px;
      margin-bottom: 10px;
      position: relative;
    }
    .section-title::after {
      content: '';
      display: block;
      width: 60px;
      height: 4px;
      background-color: #cc3366;
      margin-top: 8px;
      border-radius: 2px;
    }
    .bible-verse {
      font-style: italic;
      text-align: center;
      margin-top: 40px;
      color: #2e2e2e;
      font-size: 19px;
      background: #fce8f1;
      padding: 20px;
      border-radius: 12px;
      border-left: 5px solid #cc3366;
    }
    footer {
      text-align: center;
      margin-top: 60px;
      font-size: 17px;
      color: #666;
    }
    footer::before {
      content: '';
      display: block;
      width: 100px;
      height: 2px;
      background: #ccc;
      margin: 30px auto 10px auto;
    }
    .petal {
      position: fixed;
      top: -10px;
      background-image: url('https://upload.wikimedia.org/wikipedia/commons/thumb/4/42/Cherry_blossom_icon.svg/48px-Cherry_blossom_icon.svg.png');
      background-size: contain;
      width: 24px;
      height: 24px;
      opacity: 0.6;
      animation: fall 10s linear infinite;
      z-index: 0;
    }
    @keyframes fall {
      0% { transform: translateY(0) rotate(0); }
      100% { transform: translateY(100vh) rotate(360deg); }
    }

    @media screen and (max-width: 600px) {
      .container {
        margin: 20px;
        padding: 30px 20px;
      }
      h1 {
        font-size: 32px;
      }
      p {
        font-size: 16px;
      }
    }
  </style>
</head>
<body>
  <div class="overlay"></div>
  <div class="container">
    <h1>About Me</h1>
    <img src="WhatsApp Image 2025-06-04 at 16.58.58_a158c685.jpg" alt="My Photo" />
    <p>Hello! I'm <strong>J.Jorvina</strong>, a passionate individual who loves to learn and grow. I have interests in travelling and writing. I enjoy solving problems and making things better. I'm a Christian.</p>

    <div class="section-title">Education</div>
    <p>I am studying in Class 8 at Maharishi Vidya Mandir - Avigna School. I'm always eager to expand my knowledge and take on new challenges.</p>

    <div class="section-title">Hobbies</div>
    <p>In my free time, I love cycling, dancing, singing, playing, and spending time with family and friends.</p>

    <div class="bible-verse">
      "I can do all things through Christ who strengthens me." – Philippians 4:13
    </div>

    <div style="text-align: center; margin-top: 30px;">
      <button onclick="alert('Hello! 😊')" style="padding: 12px 25px; background-color: #cc3366; color: white; font-size: 16px; border: none; border-radius: 8px; cursor: pointer; box-shadow: 0 4px 12px rgba(0,0,0,0.2); transition: background-color 0.3s ease;">
        Say Hello
      </button>
    </div>

    <footer>
      Made with ❤️ by J.Jorvina
    </footer>
  </div>

  <!-- Petals Script -->
  <script>
    for (let i = 0; i < 20; i++) {
      let petal = document.createElement("div");
      petal.classList.add("petal");
      petal.style.left = Math.random() * 100 + "vw";
      petal.style.animationDelay = Math.random() * 10 + "s";
      document.body.appendChild(petal);
    }
  </script>

  <!-- Background Music -->
  <audio autoplay loop hidden>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_6e049fe69e.mp3?filename=relaxing-music-box-20667.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
</body>
</html>
