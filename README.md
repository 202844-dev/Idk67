<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Funny Meme Page</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #111;
      color: white;
      text-align: center;
    }
    header {
      background: #222;
      padding: 20px;
      font-size: 2rem;
      font-weight: bold;
    }
    .meme-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 20px;
    }
    .meme {
      background: #1e1e1e;
      border-radius: 12px;
      padding: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.5);
    }
    .meme img {
      width: 100%;
      border-radius: 10px;
    }
    .caption {
      margin-top: 10px;
      font-size: 1.1rem;
    }
    footer {
      background: #222;
      padding: 10px;
      font-size: 0.9rem;
      color: #aaa;
    }
  </style>
</head>
<body>

<header>
  😂 My Meme Website 😂
</header>

<section class="meme-container">
  <div class="meme">
    <img src="https://i.imgflip.com/1bij.jpg" alt="Distracted Boyfriend">
    <div class="caption">When homework is due but memes exist</div>
  </div>

  <div class="meme">
    <img src="https://i.imgflip.com/26am.jpg" alt="Grumpy Cat">
    <div class="caption">No. Just no.</div>
  </div>

  <div class="meme">
    <img src="https://i.imgflip.com/30b1gx.jpg" alt="Drake Meme">
    <div class="caption">Studying ❌  Looking at memes ✅</div>
  </div>
</section>

<footer>
  Made for free • Meme life forever
</footer>

</body>
</html>
