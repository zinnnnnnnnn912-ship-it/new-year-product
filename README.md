[index.html](https://github.com/user-attachments/files/23392181/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>New Year, New Legends</title>
  <style>
    /* 全局設定 */
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Arial', sans-serif;
    }


    body {
      background: linear-gradient(to bottom, #8B0000, #0B0B3B);
      color: #fff;
      min-height: 100vh;
      padding: 20px;
    }

    header {
      text-align: center;
      padding: 40px 20px;
    }

    header h1 {
      font-size: 3rem;
      margin-bottom: 10px;
      color: #FFD700;
      text-shadow: 2px 2px #FF4500;
    }

    header p {
      font-size: 1.2rem;
      color: #FFE4B5;
    }

    .episode {
      background: rgba(0, 0, 0, 0.5);
      border-radius: 15px;
      padding: 20px;
      margin: 30px auto;
      max-width: 800px;
      box-shadow: 0 0 15px #FFD700;
    }

    .episode h2 {
      color: #FF6347;
      margin-bottom: 10px;
      text-align: center;
    }

    .episode p {
      margin-bottom: 15px;
      line-height: 1.6;
      color: #FFFACD;
    }

    .video-container {
      position: relative;
      padding-bottom: 56.25%; /* 16:9 */
      padding-top: 25px;
      height: 0;
    }

    .video-container iframe {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      border: none;
      border-radius: 10px;
    }

    footer {
      text-align: center;
      padding: 30px 10px;
      color: #FFD700;
      font-size: 0.9rem;
    }

    /* 星星裝飾 */
    .stars {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      background: transparent;
      z-index: 0;
    }

    .star {
      position: absolute;
      width: 2px;
      height: 2px;
      background: white;
      border-radius: 50%;
      animation: twinkle 2s infinite alternate;
    }

    @keyframes twinkle {
      from { opacity: 0.2; }
      to { opacity: 1; }
    }
  </style>
</head>
<body>

  <div class="stars">
    <!-- 生成星星 -->
    <script>
      const starsContainer = document.currentScript.parentNode;
      for(let i=0;i<100;i++){
        const star = document.createElement('div');
        star.classList.add('star');
        star.style.top = Math.random()*100 + '%';
        star.style.left = Math.random()*100 + '%';
        star.style.width = (Math.random()*3+1) + 'px';
        star.style.height = star.style.width;
        star.style.animationDuration = (Math.random()*3+1) + 's';
        starsContainer.appendChild(star);
      }
    </script>
  </div>

  <header>
    <h1>New Year, New Legends</h1>
    <p>Discover Taiwan's Nian Monster and New Zealand's Matariki legends!</p>
  </header>

  <section class="episode">
    <h2>Episode 1: 台灣年獸的故事</h2>
    <p>探索台灣過年傳說中的年獸，了解年獸如何影響現代過年的習俗：紅色、聲音與光的魔力。</p>
    <div class="video-container">
      <iframe src="https://www.youtube.com/embed/y7iqehll-UQ" title="Episode 1: 台灣年獸的故事" allowfullscreen></iframe>
    </div>
  </section>

  <section class="episode">
    <h2>Episode 2: The Legend of Matariki</h2>
    <p>了解紐西蘭毛利人的新年——Matariki 星群傳說，以及它如何象徵新的開始與豐收。</p>
    <div class="video-container">
      <iframe src="https://www.youtube.com/embed/PQXa7aVFlps" title="Episode 2: The Legend of Matariki" allowfullscreen></iframe>
    </div>
  </section>

  <footer>
    &copy; 2025 New Year, New Legends. All Rights Reserved.
  </footer>

</body>
</html>
