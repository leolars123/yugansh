<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Just for You</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap');

    body {
      margin: 0;
      padding: 0;
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #667eea, #764ba2);
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      min-height: 100vh;
      overflow-x: hidden;
      position: relative;
    }

    .stars {
      position: absolute;
      width: 100%;
      height: 100%;
      background: transparent url('https://media.giphy.com/media/l3vR85PnGsBwu1PFK/giphy.gif') repeat;
      opacity: 0.05;
      animation: moveStars 150s linear infinite;
      z-index: 0;
    }

    @keyframes moveStars {
      0% { background-position: 0 0; }
      100% { background-position: -5000px 2500px; }
    }

    .container {
      position: relative;
      z-index: 2;
      max-width: 850px;
      padding: 40px;
      background: rgba(0, 0, 0, 0.5);
      border-radius: 20px;
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
    }

    h1 {
      font-size: 3em;
      margin-bottom: 20px;
    }

    p {
      font-size: 1.5em;
      line-height: 1.8em;
      margin: 20px 0;
    }

    .photo-section {
      margin-top: 30px;
    }

    img {
      width: 300px;
      max-width: 90%;
      border-radius: 15px;
      margin: 15px 10px;
      box-shadow: 0 0 15px rgba(255,255,255,0.2);
    }

    .caption {
      font-size: 1.1em;
      margin-top: 5px;
      font-style: italic;
      color: #ffd700;
    }

    .button {
      margin-top: 30px;
      padding: 15px 30px;
      font-size: 1.2em;
      background: #ffd700;
      color: #333;
      border: none;
      border-radius: 40px;
      cursor: pointer;
      font-weight: bold;
      transition: 0.3s ease;
    }

    .button:hover {
      background: #fff176;
      transform: scale(1.05);
    }

    audio {
      display: none;
    }
  </style>
</head>
<body>
  <div class="stars"></div>
  <div class="container">
    <h1>Just for You 💛</h1>

    <p>No matter what you're feeling right now, just know I'm here.  
    Through the good, the chaos, and even the nothing — I got you. Always.  
    You don’t have to go through it alone.</p>

    <p>This isn’t just a website — it’s a reminder that I care, that I see you, and that your feelings matter.  
    You’ve got a friend in me who’s always gonna root for your light to shine again 🌟</p>

    <p>Take your time. You don't owe anyone your healing speed. But if your heart ever feels heavy,  
    remember this: you're loved, you're needed, and you're strong as hell.</p>

    <div class="photo-section">
      <img src="data:image/jpeg;base64,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" alt="First photo">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRZiEsQb05HsdUfiM0Aa3JTVvrVVZpyuQQwBxDu_AGf02ay7WMFKdu4J2vHEC9_xKqgYrc&usqp=CAU" alt="Second photo">
      <div class="caption">USSSSS!</div>
    </div>

    <button class="button" onclick="alert('You smiled. That’s all I needed 💛')">Smile Again 😊</button>


    <!-- Audio 2: La La Land - Mia & Sebastian's Theme -->
    <audio autoplay loop>
      <source src="<iframe data-testid="embed-iframe" style="border-radius:12px" src="https://open.spotify.com/embed/track/6yTKjpwpROUuFB3Vf0XeJN?utm_source=generator" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>" type="audio/mp3">
    </audio>
  </div>
</body>
</html>
