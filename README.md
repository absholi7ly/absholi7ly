<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>absholi7ly - Cybersecurity Engineer</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <link href="https://fonts.googleapis.com/css2?family=Share+Tech+Mono&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Share Tech Mono', monospace;
      background-color: #000;
      color: #0f0;
      overflow-x: hidden;
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
    canvas {
      display: block;
    }
    .terminal {
      background-color: rgba(0, 0, 0, 0.8);
      border: 2px solid #0f0;
      padding: 1rem;
      margin: 2rem;
      font-size: 1rem;
      white-space: pre-wrap;
      animation: typing 3s steps(30, end), blink-caret 0.75s step-end infinite;
    }
    @keyframes typing {
      from { width: 0; }
      to { width: 100%; }
    }
    @keyframes blink-caret {
      from, to { border-color: transparent; }
      50% { border-color: #0f0; }
    }
    .btn {
      display: inline-block;
      background: #00ffcc;
      color: #000;
      padding: 0.5rem 1rem;
      margin: 0.5rem;
      text-decoration: none;
      font-weight: bold;
      border-radius: 5px;
      box-shadow: 0 0 10px #00ffcc, 0 0 40px #00ffcc;
    }
    .project-card {
      background: #111;
      padding: 1rem;
      margin: 1rem;
      border: 1px solid #0f0;
      border-radius: 10px;
      box-shadow: 0 0 10px #0f0;
    }
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
      gap: 1rem;
      margin: 2rem;
    }
    .skill-bar {
      background: #333;
      border: 1px solid #0f0;
      height: 20px;
      border-radius: 5px;
      overflow: hidden;
    }
    .skill-bar-fill {
      height: 100%;
      background: #0f0;
      width: 80%;
    }
    .timeline {
      margin: 2rem;
      border-left: 2px solid #0f0;
      padding-left: 1rem;
    }
    .timeline-entry {
      margin: 1rem 0;
    }
    .search {
      margin: 1rem;
    }
  </style>
</head>
<body>
  <canvas class="matrix"></canvas>  <div class="terminal">
    <h2>Welcome to absholi7ly’s Realm</h2>
    <p>Independent Vulnerability Hunter | Exploit Developer | Cybersecurity Engineer in the Shadows</p>
  </div>  <div class="search">
    <input type="text" placeholder="Search projects..." style="width: 100%; padding: 0.5rem;">
  </div>  <div class="skills-grid">
    <div>
      <strong>Burp Suite</strong>
      <div class="skill-bar"><div class="skill-bar-fill" style="width: 90%"></div></div>
    </div>
    <div>
      <strong>Wireshark</strong>
      <div class="skill-bar"><div class="skill-bar-fill" style="width: 85%"></div></div>
    </div>
    <div>
      <strong>Python Scripting</strong>
      <div class="skill-bar"><div class="skill-bar-fill" style="width: 95%"></div></div>
    </div>
  </div>  <div class="timeline">
    <div class="timeline-entry">
      <h4>2023</h4>
      <p>Discovered multiple CVEs in government platforms.</p>
    </div>
    <div class="timeline-entry">
      <h4>2024</h4>
      <p>Developed POCs for critical RCE vulnerabilities.</p>
    </div>
  </div>  <div class="project-card">
    <h3>🔐 Exploit Hub</h3>
    <p>Repository for advanced exploits and bypass techniques.</p>
    <a href="#" class="btn">Explore</a>
  </div>  <div class="project-card">
    <h3>🛡️ XSS Toolkit</h3>
    <p>Custom scripts and tools to detect and test XSS vectors.</p>
    <a href="#" class="btn">Try it</a>
  </div>  <script>
    // Matrix Effect
    const canvas = document.querySelector("canvas");
    const ctx = canvas.getContext("2d");
    canvas.height = window.innerHeight;
    canvas.width = window.innerWidth;
    const chars = "01";
    const fontSize = 14;
    const columns = canvas.width / fontSize;
    const drops = Array.from({ length: columns }, () => 1);
    function draw() {
      ctx.fillStyle = "rgba(0, 0, 0, 0.05)";
      ctx.fillRect(0, 0, canvas.width, canvas.height);
      ctx.fillStyle = "#0f0";
      ctx.font = `${fontSize}px monospace`;
      for (let i = 0; i < drops.length; i++) {
        const text = chars[Math.floor(Math.random() * chars.length)];
        ctx.fillText(text, i * fontSize, drops[i] * fontSize);
        if (drops[i] * fontSize > canvas.height && Math.random() > 0.975) drops[i] = 0;
        drops[i]++;
      }
    }
    setInterval(draw, 35);

    // Sound Effect on Load
    const sound = new Audio('https://www.soundjay.com/button/beep-07.wav');
    sound.volume = 0.3;
    window.addEventListener('load', () => sound.play());
  </script></body>
</html>
