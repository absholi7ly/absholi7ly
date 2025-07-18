<!-- README.md as an interactive portfolio (HTML styled Markdown) -->

<!-- MATRIX RAIN EFFECT BACKGROUND -->
<style>
  body {
    margin: 0;
    font-family: 'Fira Code', monospace;
    background: black;
    color: #00ff99;
    overflow-x: hidden;
    background-image: radial-gradient(circle, #001f1f 10%, black 90%);
  }
  canvas#matrix {
    position: fixed;
    top: 0; left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
  }
</style>
<canvas id="matrix"></canvas>
<script>
const canvas = document.getElementById("matrix"), ctx = canvas.getContext("2d");
canvas.height = window.innerHeight; canvas.width = window.innerWidth;
const chars = "アァイイウエオカキクケコサシスセソタチツテト0123456789".split("");
const cols = canvas.width / 20; const drops = Array(Math.floor(cols)).fill(1);
function drawMatrix() {
  ctx.fillStyle = "rgba(0, 0, 0, 0.05)";
  ctx.fillRect(0, 0, canvas.width, canvas.height);
  ctx.fillStyle = "#0f0";
  ctx.font = "16px monospace";
  for (let i = 0; i < drops.length; i++) {
    const text = chars[Math.floor(Math.random() * chars.length)];
    ctx.fillText(text, i * 20, drops[i] * 20);
    if (drops[i] * 20 > canvas.height || Math.random() > 0.95) drops[i] = 0;
    drops[i]++;
  }
}
setInterval(drawMatrix, 33);
</script>

<!-- AUDIO ON LOAD -->
<audio autoplay hidden>
  <source src="https://assets.mixkit.co/active_storage/sfx/1132/1132-preview.mp3" type="audio/mpeg">
</audio>

<!-- TERMINAL WELCOME -->
<h1 align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=700&size=22&pause=1000&center=true&vCenter=true&width=435&lines=Welcome+to+absholi7ly's+Cyber+Terminal...;Security+Researcher+%2F+Exploit+Developer+%2F+Shadow+Pentester"/>
</h1>

<!-- PROFILE CARD -->
<div align="center">
  <img src="https://avatars.githubusercontent.com/u/104905682?v=4" width="120" style="border-radius: 50%;" />
  <h2>Hi, I'm <strong>absholi7ly</strong> — Cybersecurity Specialist</h2>
  <p>🐍 Python Scripter | 🌐 Web Exploiter | 🎯 Bug Hunter | 💻 Network Sniffer | 👻 OSINT Operative</p>
  <img src="https://skillicons.dev/icons?i=python,linux,bash,git,github,html,burpsuite,wireshark,vscode"/>
</div>

<!-- QR CODE + EMAIL -->
<div align="center">
  <img src="https://api.qrserver.com/v1/create-qr-code/?data=https://github.com/absholi7ly&size=120x120" alt="QR Code" />
  <p>📩 <a href="mailto:Abdualhadi.khalifa96@gmail.com">Email Me</a></p>
</div>

<!-- ABOUT ME SECTIONS -->
<details>
<summary><strong>🧠 Who am I?</strong></summary>
<p>
  I am an independent vulnerability hunter who operates in the shadows. I specialize in identifying and exploiting web vulnerabilities, building proof-of-concept (PoC) scripts, and conducting deep security research. My methodology is stealthy, creative, and unconventional.
</p>
</details>

<details>
<summary><strong>📡 Skills & Tools</strong></summary>
<ul>
  <li>Web Exploitation & Bug Hunting (XSS, RCE, SQLi, SSRF, etc.)</li>
  <li>Python Scripting for Automation</li>
  <li>Burp Suite, Wireshark, Nmap, etc.</li>
  <li>Network Analysis & Packet Capture</li>
  <li>Shell & Bash Automation</li>
</ul>
</details>

<!-- GITHUB STATS -->
<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=absholi7ly&show_icons=true&theme=radical"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=absholi7ly&layout=compact&theme=radical"/>
</div>

<!-- CHART.JS RADAR -->
<h3 align="center">My Technical Radar</h3>
<canvas id="skillRadar" width="400" height="300"></canvas>
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script>
const ctxRadar = document.getElementById('skillRadar');
new Chart(ctxRadar, {
  type: 'radar',
  data: {
    labels: ['Web Exploit', 'Python', 'Networking', 'Recon', 'PoC Dev', 'Linux'],
    datasets: [{
      label: 'Skill Level',
      data: [9, 8, 7, 9, 8, 7],
      backgroundColor: 'rgba(0, 255, 150, 0.2)',
      borderColor: 'rgba(0, 255, 150, 1)',
      borderWidth: 2
    }]
  },
  options: {
    scales: {
      r: {
        angleLines: { display: false },
        suggestedMin: 0,
        suggestedMax: 10
      }
    }
  }
});
</script>

<!-- PROJECTS PREVIEW -->
<h3 align="center">🚀 Featured Projects</h3>
<div align="center">
  <a href="https://github.com/absholi7ly/CVE-2025-20337-PoC">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=absholi7ly&repo=CVE-2025-20337-PoC&theme=radical"/>
  </a>
</div>

<!-- SIGNATURE -->
<p align="center">
  ───────▄▀▄─────▄▀▄
  ─────▄█░░▀▀▀▀▀░░█▄
  ─▄▄──█░░░░░░░░░░░█──▄▄
  █▄▄█─█░░▀░░┬░░▀░░█─█▄▄█<br/>
  <strong>~ absholi7ly</strong>
</p>

