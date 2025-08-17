<div align="center">
  <h1>
    <a href="" style="color:#00f0ff; text-shadow: 0 0 10px #00f0ff, 0 0 20px #00f0ff, 0 0 30px #00f0ff, 0 0 40px #00f0ff;">
      Hi 👋, I'm Sobhan Moqadam
    </a>
  </h1>
  <h3 style="color:#00f0ff; text-shadow: 0 0 5px #00f0ff;">
    Telegram Bot Developer • Bug Bounty Hunter • Scraper Writer • From Iran
  </h3>

  <p style="font-size:18px; color:#00f0ff; font-family:monospace;">
    <span id="typing"></span>
  </p>

  <img align="right" alt="sheikh python" width="400" src="https://mir-s3-cdn-cf.behance.net/project_modules/hd/06f21a161921919.63cd7887d0a70.gif">
</div>

<br><br>

<!-- Languages -->
<h2 align="center" style="color:#ffd700; text-shadow: 0 0 5px #ffd700;">Languages & Tools</h2>
<p align="center">
  <img src="https://img.shields.io/badge/Python-171717?style=for-the-badge&logo=python&logoColor=00f0ff&color=171717" style="border-radius:15px"/>
  <img src="https://img.shields.io/badge/HTML5-171717?style=for-the-badge&logo=html5&logoColor=00f0ff&color=171717" style="border-radius:15px"/>
  <img src="https://img.shields.io/badge/CSS3-171717?style=for-the-badge&logo=css3&logoColor=00f0ff&color=171717" style="border-radius:15px"/>
</p>

<h2 align="center" style="color:#ffd700; text-shadow: 0 0 5px #ffd700;">Tools & Technologies</h2>
<p align="center">
  <img src="https://img.shields.io/badge/Linux-171717?style=for-the-badge&logo=linux&logoColor=00f0ff&color=171717" style="border-radius:15px"/>
  <img src="https://img.shields.io/badge/Kali-171717?style=for-the-badge&logo=kalilinux&logoColor=00f0ff&color=171717" style="border-radius:15px"/>
  <img src="https://img.shields.io/badge/MySQL-171717?style=for-the-badge&logo=mysql&logoColor=00f0ff&color=171717" style="border-radius:15px"/>
</p>

<br><br>

<!-- GitHub Stats -->
<div align="center">
  <img align="center" src="https://github-readme-stats.vercel.app/api/top-langs/?username=SoBiMoqadam&langs_count=5&layout=compact&theme=gruvbox_duo&hide_border=true&bg_color=171717&title_color=00f0ff&icon_color=00f0ff&text_color=ffffff&count_private=true" alt="Top Languages"/>
</div>
<br/>
<div align="center">
  <img align="center" src="https://github-readme-stats.vercel.app/api?username=SoBiMoqadam&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&bg_color=171717&title_color=00f0ff&icon_color=00f0ff&text_color=ffffff" alt="GitHub Stats"/>
</div>

<br><br>

<!-- Contact -->
<h2 align="center" style="color:#00f0ff; text-shadow: 0 0 5px #00f0ff;">Contact Me</h2>
<p align="center">
  <a href="https://linkedin.com/in/sobhanmoqadam" target="_blank">
    <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/linkedin.svg" width="40" height="40"/>
  </a>
  <a href="https://instagram.com/cyber_nest" target="_blank">
    <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/instagram.svg" width="40" height="40"/>
  </a>
</p>

<!-- Typing Animation Script -->
<script>
const texts = ["Telegram Bot Developer", "Bug Bounty Hunter", "Web Scraper"];
let count = 0;
let index = 0;
let currentText = "";
let letter = "";

(function type(){
  if(count === texts.length){
    count = 0;
  }
  currentText = texts[count];
  letter = currentText.slice(0, ++index);
  document.getElementById("typing").textContent = letter;
  if(letter.length === currentText.length){
    count++;
    index = 0;
    setTimeout(type, 1000);
  } else {
    setTimeout(type, 150);
  }
})();
</script>
