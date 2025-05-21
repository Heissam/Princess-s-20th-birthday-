<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>You're Invited to Princess's 20th Birthday!</title>
  <style>
    body {
      background: linear-gradient(135deg, #0e0e0e 0%, #1a1a2e 100%);
      text-align: center;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      padding: 40px 20px;
      color: white;
      overflow-x: hidden;
      min-height: 100vh;
      position: relative;
    }

    /* Watermark Style */
    .watermark {
      position: fixed;
      bottom: 20px;
      left: 20px;
      opacity: 0.85;
      z-index: 10;
      width: 250px;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
      transition: all 0.3s ease;
      border: 2px solid rgba(0, 180, 255, 0.5);
    }

    .watermark:hover {
      opacity: 1;
      transform: scale(1.03);
      box-shadow: 0 8px 25px rgba(0, 180, 255, 0.3);
    }

    .container {
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
      position: relative;
      z-index: 1;
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 30px;
      background: linear-gradient(90deg, #00a8ff, #00f2ff);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      text-shadow: 0 0 10px rgba(0, 168, 255, 0.3);
    }

    .pop {
      display: inline-block;
      animation: pop 1s ease-in-out forwards;
      transform-origin: center;
    }

    @keyframes pop {
      0% { transform: scale(0); opacity: 0; }
      50% { transform: scale(1.1); opacity: 1; }
      100% { transform: scale(1); }
    }

    .sparkle {
      animation: sparkle 2s infinite ease-in-out;
    }

    @keyframes sparkle {
      0% { box-shadow: 0 0 10px #00a8ff; }
      50% { box-shadow: 0 0 20px #00f2ff; }
      100% { box-shadow: 0 0 10px #00a8ff; }
    }

    .gift-box {
      width: 150px;
      height: 150px;
      background: linear-gradient(145deg, #00a8ff, #0077ff);
      margin: 0 auto;
      border-radius: 10px;
      position: relative;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
    }

    .gift-box::before {
      content: '';
      position: absolute;
      width: 30px;
      height: 150px;
      background: rgba(255, 255, 255, 0.8);
      left: 60px;
      top: 0;
    }

    .gift-box::after {
      content: '';
      position: absolute;
      width: 150px;
      height: 30px;
      background: rgba(255, 255, 255, 0.8);
      top: 60px;
      left: 0;
    }

    .invitation {
      margin: 40px auto;
      font-size: 1.4rem;
      animation: floatIn 2s ease-in-out forwards;
      opacity: 0;
      max-width: 600px;
      line-height: 1.6;
      background: rgba(0, 168, 255, 0.1);
      padding: 20px;
      border-radius: 10px;
      border: 1px solid rgba(0, 168, 255, 0.3);
    }

    @keyframes floatIn {
      0% { transform: translateY(-50px); opacity: 0; }
      100% { transform: translateY(0); opacity: 1; }
    }

    iframe {
      margin: 30px auto;
      width: 100%;
      max-width: 500px;
      height: 500px;
      border: none;
      border-radius: 10px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
    }

    .thank-you {
      display: none;
      font-size: 1.8rem;
      margin: 50px auto;
      animation: fadeIn 2s ease-in;
      max-width: 600px;
      padding: 20px;
      background: rgba(0, 242, 255, 0.1);
      border-radius: 10px;
      border: 1px solid rgba(0, 242, 255, 0.3);
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    .music-control {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: rgba(0, 0, 0, 0.5);
      border-radius: 50%;
      width: 50px;
      height: 50px;
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
      z-index: 100;
      border: 1px solid rgba(0, 168, 255, 0.5);
    }

    .music-control i {
      font-size: 24px;
      color: #00a8ff;
    }

    @media (max-width: 600px) {
      h1 {
        font-size: 2rem;
      }
      
      .invitation {
        font-size: 1.2rem;
        padding: 15px;
      }
      
      iframe {
        height: 400px;
      }
      
      .thank-you {
        font-size: 1.4rem;
        padding: 15px;
      }

      .watermark {
        width: 180px;
        bottom: 10px;
        left: 10px;
      }
    }
  </style>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
  <!-- Watermark with your flyer -->
  <img src="1000643197.jpg" alt="20 Shades of Blue - Princess's 20th Birthday" class="watermark">

  <div class="container">
    <h1>You're Invited to Princess's 20th!</h1>

    <div class="pop sparkle">
      <div class="gift-box"></div>
    </div>

    <div class="invitation">
      You're cordially invited to "20 Shades of Blue" - A celebration in honor of Princess's 20th Birthday!<br><br>
      Come dressed in your best shade of blue and let's light up the night in 20 shades of fabulous!
    </div>

    <div id="form-container">
      <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSc1aI9beUYkIxtmZBSYSMa8U1prTqerTSwY8kQAE2805G5GmA/viewform?embedded=true" loading="lazy">Loading…</iframe>
    </div>

    <div class="thank-you" id="thankYouMessage">
      Thank you for RSVPing! We can't wait to celebrate with you on June 7th!
    </div>
  </div>

  <!-- Birthday music - "Celebration" by Kool & The Gang (royalty-free version) -->
  <audio id="bg-music" loop>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-8.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <div class="music-control" id="musicControl">
    <i class="fas fa-music"></i>
  </div>

  <script>
    // Music control
    const music = document.getElementById("bg-music");
    const musicControl = document.getElementById("musicControl");
    let musicPlaying = false;
    
    // Try to play music on user interaction (to bypass autoplay restrictions)
    document.body.addEventListener('click', function() {
      if (!musicPlaying) {
        music.volume = 0.3;
        music.play().then(() => {
          musicPlaying = true;
          musicControl.innerHTML = '<i class="fas fa-pause"></i>';
        }).catch(e => {
          console.log("Audio playback failed:", e);
        });
      }
    }, { once: true });
    
    musicControl.addEventListener('click', function(e) {
      e.stopPropagation();
      if (musicPlaying) {
        music.pause();
        musicControl.innerHTML = '<i class="fas fa-music"></i>';
      } else {
        music.play();
        musicControl.innerHTML = '<i class="fas fa-pause"></i>';
      }
      musicPlaying = !musicPlaying;
    });

    // Form submission detection
    const iframe = document.querySelector("iframe");
    const thankYouMsg = document.getElementById("thankYouMessage");
    const formContainer = document.getElementById("form-container");

    // More reliable way to detect form submission
    window.addEventListener('message', function(event) {
      // Check if the message is from the Google Forms domain
      if (event.origin === "https://docs.google.com") {
        if (event.data.includes("form-submit-success")) {
          formContainer.style.display = "none";
          thankYouMsg.style.display = "block";
          
          // Small celebration effect
          thankYouMsg.classList.add("sparkle");
          setTimeout(() => {
            thankYouMsg.classList.remove("sparkle");
          }, 3000);
        }
      }
    });

    // Fallback method
    setInterval(() => {
      try {
        const url = iframe.contentWindow.location.href;
        if (url.includes("formResponse")) {
          formContainer.style.display = "none";
          thankYouMsg.style.display = "block";
        }
      } catch (e) {
        // Ignore CORS issue
      }
    }, 1000);
  </script>
</body>
</html>
