<!DOCTYPE html>
<html>
<head>
<title>Suhani ❤️ Sourabh</title>
<style>
   body {
     text-align: center;
     font-family: Arial, sans-serif;
     background: linear-gradient(to right, #ff9a9e, #fad0c4);
     margin-top: 80px;
     color: white;
     overflow: hidden;
   }
   h1 { font-size: 34px; }
   h2 { font-weight: normal; font-size: 20px; margin-bottom: 30px; }
   .distance {
     font-size: 18px;
     margin-bottom: 40px;
   }
   button {
     padding: 12px 25px;
     font-size: 18px;
     margin: 10px;
     border: none;
     border-radius: 10px;
     cursor: pointer;
     transition: 0.3s;
   }
   .yes-button {
     background-color: #28a745;
     color: white;
   }
   .no-button {
     background-color: #dc3545;
     color: white;
   }
   .music-btn {
     background-color: white;
     color: #ff4d6d;
     font-size: 14px;
     margin-top: 20px;
   }
</style>
</head>
<body>
<h1>Bangalore ❤️ Kolkata</h1>
<h2>Suhani & Sourabh</h2>
<div class="distance">
   1560 km apart… but still connected by one heart 💞
</div>
<h1>Sourabh, will you be my Valentine? 💌</h1>
<button class="yes-button" onclick="handleYesClick()">Yes, always ❤️</button>
<button class="no-button" onclick="handleNoClick()">No 😢</button>
<br>
<button class="music-btn" onclick="playMusic()">Tap to Start Music 🎶</button>
<!-- Background Music -->
<audio id="bgMusic" loop>
<!-- Replace this link with any romantic MP3 you like -->
<source src="https://djpunjab.is/bollywood/mast-magan-mp3-song-dszsed.html">
</audio>
<script>
   const messages = [
     "But we survived long distance 🥺",
     "Think about our late night calls 📞",
     "Remember our future plans 💍",
     "Distance makes us stronger 💪❤️",
     "Okay fine… last chance 😭"
   ];
   let messageIndex = 0;
   function handleNoClick() {
     const noButton = document.querySelector(".no-button");
     const yesButton = document.querySelector(".yes-button");
     noButton.textContent = messages[messageIndex];
     messageIndex = (messageIndex + 1) % messages.length;
     const currentSize = parseFloat(
       window.getComputedStyle(yesButton).fontSize
     );
     yesButton.style.fontSize = (currentSize * 1.5) + "px";
   }
   function handleYesClick() {
     window.location.href = "yes_page.html";
   }
   function playMusic() {
     const music = document.getElementById("bgMusic");
     music.play();
   }
</script>
</body>
</html>
