<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sobhan Moqadam</title>
<style>
  body {
    margin: 0;
    font-family: 'Courier New', monospace;
    background-color: #171717;
    color: #00f0ff;
  }
  .section {
    position: relative;
    padding: 50px 20px;
    overflow: hidden;
    margin: 30px auto;
    max-width: 900px;
    border-radius: 15px;
  }
  .section h1, .section h2, .section h3, .section p {
    position: relative;
    z-index: 1;
    text-align: center;
    margin: 10px 0;
  }
  h1 {
    font-size: 3em;
    text-shadow: 0 0 10px #00f0ff, 0 0 20px #00f0ff;
  }
  h2 {
    color: #ffd700;
    text-shadow: 0 0 5px #ffd700;
  }
  h3 {
    text-shadow: 0 0 5px #00f0ff;
  }
  .typing {
    font-size: 1.5em;
    text-shadow: 0 0 5px #00f0ff;
  }
  .tools img, .contact img {
    width: 50px;
    margin: 10px;
    filter: drop-shadow(0 0 5px #00f0ff);
    vertical-align: middle;
  }
  canvas {
    position: absolute;
    top: 0; left: 0;
    width: 100%;
    height: 100%;
    z-index: 0;
  }
</style>
</head>
<body>

<!-- Typing Section -->
<div class="section" id="typing-section">
  <canvas></canvas>
  <h1>Hi 👋, I'm Sobhan Moqadam</h1>
  <h3>Telegram Bot Developer • Bug Bounty Hunter • Scraper Writer • From Iran</h3>
  <p class="typing" id="typing"></p>
</div>

<!-- Tools Section -->
<div class="section" id="tools-section">
  <canvas></canvas>
  <h2>Languages & Tools</h2>
  <div class="tools">
    <img src="https://img.shields.io/badge/Python-171717?style=for-the-badge&logo=python&logoColor=00f0ff&color=171717" alt="Python">
    <img src="https://img.shields.io/badge/HTML5-171717?style=for-the-badge&logo=html5&logoColor=00f0ff&color=171717" alt="HTML">
    <img src="https://img.shields.io/badge/CSS3-171717?style=for-the-badge&logo=css3&logoColor=00f0ff&color=171717" alt="CSS">
    <img src="https://img.shields.io/badge/Linux-171717?style=for-the-badge&logo=linux&logoColor=00f0ff&color=171717" alt="Linux">
    <img src="https://img.shields.io/badge/Kali-171717?style=for-the-badge&logo=kalilinux&logoColor=00f0ff&color=171717" alt="Kali">
    <img src="https://img.shields.io/badge/MySQL-171717?style=for-the-badge&logo=mysql&logoColor=00f0ff&color=171717" alt="MySQL">
  </div>
</div>

<!-- Contact Section -->
<div class="section" id="contact-section">
  <canvas></canvas>
  <h2>Contact Me</h2>
  <div class="contact">
    <a href="https://linkedin.com/in/sobhanmoqadam" target="_blank">
      <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/linkedin.svg" alt="LinkedIn">
    </a>
    <a href="https://instagram.com/cyber_nest" target="_blank">
      <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/instagram.svg" alt="Instagram">
    </a>
  </div>
</div>

<!-- Typing Script -->
<script>
const texts = ["Telegram Bot Developer", "Bug Bounty Hunter", "Web Scraper"];
let count = 0, index = 0, currentText = "", letter = "";
(function type(){
  if(count === texts.length) count = 0;
  currentText = texts[count];
  letter = currentText.slice(0, ++index);
  document.getElementById("typing").textContent = letter;
  if(letter.length === currentText.length){
    count++; index=0; setTimeout(type,1000);
  } else setTimeout(type,150);
})();
</script>

<!-- Neon Lines Script -->
<script>
function createNeon(canvas) {
  const ctx = canvas.getContext('2d');
  canvas.width = canvas.offsetWidth;
  canvas.height = canvas.offsetHeight;

  const lines = [];
  for(let i=0;i<20;i++){
    lines.push({
      x: Math.random()*canvas.width,
      y: Math.random()*canvas.height/2, // فقط نیمه بالا
      length: 50 + Math.random()*100,
      speed: 0.5 + Math.random()*1.5,
      angle: Math.random()*2*Math.PI,
      color: 'rgba(0, 240, 255, 0.3)',
    });
  }

  function draw(){
    ctx.clearRect(0,0,canvas.width,canvas.height);
    lines.forEach(line=>{
      ctx.beginPath();
      ctx.moveTo(line.x, line.y);
      ctx.lineTo(line.x + Math.cos(line.angle)*line.length, line.y + Math.sin(line.angle)*line.length);
      ctx.strokeStyle = line.color;
      ctx.lineWidth = 2;
      ctx.shadowColor = '#00f0ff';
      ctx.shadowBlur = 10;
      ctx.stroke();
      line.x += Math.cos(line.angle)*line.speed;
      line.y += Math.sin(line.angle)*line.speed;
      if(line.x>canvas.width+50) line.x=-50;
      if(line.x<-50) line.x=canvas.width+50;
      if(line.y>canvas.height/2+50) line.y=-50;
      if(line.y<-50) line.y=canvas.height/2+50;
    });
    requestAnimationFrame(draw);
  }
  draw();
}

document.querySelectorAll('canvas').forEach(c => createNeon(c));
</script>

</body>
</html>
