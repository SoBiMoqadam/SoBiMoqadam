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
    background-color: #0d0d0d;
    color: #00f0ff;
  }

  /* Common section style */
  .section {
    position: relative;
    padding: 60px 20px;
    max-width: 900px;
    margin: 50px auto;
    border-radius: 15px;
    overflow: hidden;
  }

  /* Neon moving lines */
  .section::before {
    content: "";
    position: absolute;
    top: 0; left: 0;
    width: 100%; height: 100%;
    background: repeating-linear-gradient(
      45deg,
      rgba(0,240,255,0.2),
      rgba(0,240,255,0.2) 1px,
      transparent 2px,
      transparent 10px
    );
    animation: moveLines 5s linear infinite;
    z-index: 0;
  }

  @keyframes moveLines {
    0% {background-position: 0 0;}
    100% {background-position: 200px 200px;}
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
    overflow: hidden;
    border-right: .15em solid #00f0ff;
    white-space: nowrap;
    animation: typing 3s steps(30, end), blink 0.75s step-end infinite;
  }

  @keyframes typing {
    from { width: 0 }
    to { width: 100% }
  }

  @keyframes blink {
    50% { border-color: transparent; }
  }

  .typing {
    font-size: 1.5em;
    color: #00f0ff;
    text-align: center;
    overflow: hidden;
    border-right: .15em solid #00f0ff;
    white-space: nowrap;
    animation: typing2 4s steps(40, end) infinite, blink 0.75s step-end infinite;
  }

  @keyframes typing2 {
    0%, 20% { width: 0; }
    40%, 60% { width: 100%; }
    80%, 100% { width: 0; }
  }

  /* Tools */
  .tools img {
    width: 60px;
    margin: 10px;
    filter: drop-shadow(0 0 10px #00f0ff);
    vertical-align: middle;
  }

  /* Contact */
  .contact img {
    width: 50px;
    margin: 10px;
    filter: drop-shadow(0 0 10px #00f0ff);
    vertical-align: middle;
  }

</style>
</head>
<body>

<!-- Typing Section -->
<div class="section">
  <h1>Hi 👋, I'm Sobhan Moqadam</h1>
  <h3>Telegram Bot Developer • Bug Bounty Hunter • Scraper Writer • From Iran</h3>
  <p class="typing">Telegram Bot Developer • Bug Bounty • Web Scraper</p>
</div>

<!-- Tools Section -->
<div class="section">
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
<div class="section">
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

</body>
</html>
