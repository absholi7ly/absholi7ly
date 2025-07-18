<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>absholi7ly | Cybersecurity Engineer</title>
  <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet" />
  <style>
    body {
      margin: 0;
      font-family: 'Fira Code', monospace;
      background-color: #0e0e0e;
      color: #e0e0e0;
      overflow-x: hidden;
    }
    .container {
      max-width: 900px;
      margin: 0 auto;
      padding: 2rem;
    }
    h1, h2 {
      color: #00ffcc;
    }
    .matrix {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background: black;
      z-index: -1;
    }
    .timeline {
      border-left: 2px solid #00ffcc;
      margin: 2rem 0;
      padding-left: 1rem;
    }
    .timeline-item {
      margin-bottom: 1.5rem;
    }
    .counter {
      font-size: 2rem;
      margin: 2rem 0;
    }
    .terminal {
      background: #111;
      color: #0f0;
      padding: 1rem;
      border-radius: 8px;
      font-size: 1rem;
      margin-bottom: 2rem;
    }
    .project-showcase {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1rem;
    }
    .card {
      background: #1e1e1e;
      border: 1px solid #444;
      padding: 1rem;
      border-radius: 8px;
      transition: transform 0.3s;
    }
    .card:hover {
      transform: scale(1.05);
    }
    .stats {
      margin: 2rem 0;
    }
    .radar {
      width: 100%;
      max-width: 500px;
      margin: auto;
    }
  </style>
</head>
<body>
  <canvas class="matrix"></canvas>
  <div class="container">
    <h1>👾 Absholi7ly</h1>
    <h2>Independent Vulnerability Hunter | Exploit Developer | Cybersecurity Engineer</h2><div class="terminal">
  <p><strong>$ whoami</strong></p>
  <p>🧠 Security Researcher</p>
  <p>🕵️ Exploit Deployment Specialist</p>
  <p>💻 Python/Web Scripter</p>
</div>

<h2>📈 GitHub Stats</h2>
<div class="stats">
  <img src="https://github-readme-stats.vercel.app/api?username=absholi7ly&show_icons=true&theme=radical" alt="GitHub Stats" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=absholi7ly&theme=radical" alt="GitHub Streak" />
</div>

<h2>📅 Career Timeline</h2>
<div class="timeline">
  <div class="timeline-item">🔍 2020 - Started Bug Bounty & CTFs</div>
  <div class="timeline-item">🚨 2021 - Reported multiple CVEs</div>
  <div class="timeline-item">💡 2022 - Built internal exploit automation tools</div>
  <div class="timeline-item">🔐 2023 - Joined underground security collectives</div>
</div>

<h2>📊 Radar of Expertise</h2>
<div class="radar">
  <img src="https://cr-skills-chart-widget.vercel.app/api?username=absholi7ly&labels=true" alt="Skills Radar" />
</div>

<h2>🧪 PoC / Projects</h2>
<div class="project-showcase">
  <div class="card">
    <h3>🔍 CVE-2025-20337</h3>
    <p>Remote Root RCE on Cisco ISE - Python PoC</p>
  </div>
  <div class="card">
    <h3>🕷️ Web Vuln Scanner</h3>
    <p>Custom scanner for XSS/LFI/SQLi detection</p>
  </div>
  <div class="card">
    <h3>🦞 ShellDrop</h3>
    <p>Reverse Shell deployment tool with payload rotator</p>
  </div>
</div>

<h2>🎯 Contact</h2>
<p>Email: <a href="mailto:Abdualhadi.khalifa96@gmail.com">Abdualhadi.khalifa96@gmail.com</a></p>
<p>Telegram: <a href="https://t.me/absholi7ly">@absholi7ly</a></p>

  </div>  <!-- Matrix Rain Script -->  <script>
    const canvas = document.querySelector(".matrix");
    const ctx = canvas.getContext("2d");
    canvas.height = window.innerHeight;
    canvas.width = window.innerWidth;
    const letters = "01".split("");
    const fontSize = 14;
    const columns = canvas.width / fontSize;
    const drops = Array(Math.floor(columns)).fill(1);

    function draw() {
      ctx.fillStyle = "rgba(0, 0, 0, 0.05)";
      ctx.fillRect(0, 0, canvas.width, canvas.height);
      ctx.fillStyle = "#0f0";
      ctx.font = fontSize + "px monospace";
      for (let i = 0; i < drops.length; i++) {
        const text = letters[Math.floor(Math.random() * letters.length)];
        ctx.fillText(text, i * fontSize, drops[i] * fontSize);
        if (drops[i] * fontSize > canvas.height && Math.random() > 0.975) drops[i] = 0;
        drops[i]++;
      }
    }
    setInterval(draw, 33);
  </script>  <!-- Sound Effect on Load -->  <audio autoplay>
    <source src="https://assets.mixkit.co/sfx/preview/mixkit-retro-arcade-casino-notification-211.mp3" type="audio/mpeg">
  </audio>
</body>
</html>
