<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>For My Babe ❤️</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff9a9e 0%, #fad0c4 50%, #fbc2eb 100%);
      font-family: 'Georgia', serif;
      overflow-x: hidden;
    }

    .container {
      text-align: center;
      max-width: 600px;
      padding: 20px;
    }

    h1 {
      color: #fff;
      font-size: 2.2rem;
      margin-bottom: 30px;
      text-shadow: 0 2px 8px rgba(0,0,0,0.15);
    }

    .btn {
      background: #ff4d6d;
      color: white;
      border: none;
      padding: 16px 40px;
      font-size: 1.3rem;
      border-radius: 50px;
      cursor: pointer;
      box-shadow: 0 8px 20px rgba(255, 77, 109, 0.4);
      transition: all 0.3s ease;
      font-family: inherit;
    }

    .btn:hover {
      transform: scale(1.05);
      background: #ff2e55;
    }

    .content {
      display: none;
      opacity: 0;
      transition: opacity 1.2s ease;
      margin-top: 40px;
    }

    .content.show {
      display: block;
      opacity: 1;
    }

    .photo {
      width: 100%;
      max-width: 320px;
      border-radius: 20px;
      box-shadow: 0 15px 35px rgba(0,0,0,0.2);
      margin-bottom: 30px;
      border: 6px solid white;
    }

    .letter {
      background: white;
      padding: 30px 25px;
      border-radius: 16px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.1);
      text-align: left;
      line-height: 1.7;
      color: #333;
      position: relative;
    }

    .letter::before {
      content: "💌";
      position: absolute;
      top: -20px;
      left: 20px;
      font-size: 2rem;
    }

    .letter p {
      margin-bottom: 16px;
    }

    .signature {
      text-align: right;
      font-style: italic;
      margin-top: 25px;
      color: #ff4d6d;
      font-size: 1.15rem;
    }

    .hearts {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      overflow: hidden;
      z-index: -1;
    }

    .heart {
      position: absolute;
      font-size: 20px;
      animation: float 6s linear infinite;
      opacity: 0.7;
    }

    @keyframes float {
      0% {
        transform: translateY(100vh) rotate(0deg);
        opacity: 0.8;
      }
      100% {
        transform: translateY(-100px) rotate(360deg);
        opacity: 0;
      }
    }
  </style>
</head>
<body>

  <div class="hearts" id="hearts"></div>

  <div class="container">
    <h1>Something special for you 💕</h1>
    
    <button class="btn" id="revealBtn">Click me, my love</button>

    <div class="content" id="content">
      <!-- Replace the image source with your own photo -->
      <img 
        src="https://images.unsplash.com/photo-1516589178581-6cd7833ae3b2?w=600&q=80" 
        alt="Us" 
        class="photo"
      >

      <div class="letter">
        <p>My dearest,</p>
        
        <p>
          Every time I look at you, the world feels a little softer and a lot brighter. 
          You are my favorite hello and my hardest goodbye. 
          In a world full of ordinary days, you make mine extraordinary.
        </p>
        
        <p>
          Thank you for being the reason I smile for no reason, 
          the calm in my chaos, and the home I never knew I needed.
        </p>
        
        <p>
          I love you more than words can hold — but I hope these ones come close.
        </p>
        
        <div class="signature">
          Forever yours,<br>
          [Your Name]
        </div>
      </div>
    </div>
  </div>

  <script>
    const btn = document.getElementById('revealBtn');
    const content = document.getElementById('content');
    const heartsContainer = document.getElementById('hearts');

    btn.addEventListener('click', () => {
      content.classList.add('show');
      btn.style.display = 'none';
      createHearts();
    });

    function createHearts() {
      for (let i = 0; i < 25; i++) {
        setTimeout(() => {
          const heart = document.createElement('div');
          heart.classList.add('heart');
          heart.innerHTML = '❤️';
          heart.style.left = Math.random() * 100 + 'vw';
          heart.style.animationDuration = (Math.random() * 3 + 4) + 's';
          heart.style.fontSize = (Math.random() * 20 + 15) + 'px';
          heartsContainer.appendChild(heart);

          setTimeout(() => heart.remove(), 7000);
        }, i * 150);
      }
    }
  </script>
</body>
</html>