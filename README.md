<div align="center">

<!-- ████████████████████████████████████████████████████████████████████████
                    🔥 ANIMATED NAME BANNER — GLITCH + NEON + REVEAL 🔥
     ████████████████████████████████████████████████████████████████████████ -->

<svg width="800" height="160" viewBox="0 0 800 160" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- deep neon glow -->
    <filter id="neon" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur in="SourceGraphic" stdDeviation="5" result="b1"/>
      <feGaussianBlur in="SourceGraphic" stdDeviation="2" result="b2"/>
      <feMerge>
        <feMergeNode in="b1"/>
        <feMergeNode in="b2"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <!-- tight glow for main text -->
    <filter id="glow" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur in="SourceGraphic" stdDeviation="3" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <!-- background gradient -->
    <radialGradient id="bg" cx="50%" cy="50%" r="75%">
      <stop offset="0%"   stop-color="#0c0c10"/>
      <stop offset="100%" stop-color="#020203"/>
    </radialGradient>
    <!-- horizontal scanline pattern -->
    <pattern id="scan" patternUnits="userSpaceOnUse" width="800" height="4">
      <rect width="800" height="1.5" fill="#ffffff" fill-opacity="0.03"/>
    </pattern>
    <!-- clip for the initial wipe-reveal of the name -->
    <clipPath id="wipe">
      <rect x="0" y="0" width="0" height="160">
        <animate attributeName="width" values="0;800" dur="0.9s" fill="freeze" calcMode="ease-out"/>
      </rect>
    </clipPath>
  </defs>

  <!-- ── background ── -->
  <rect width="800" height="160" rx="14" fill="url(#bg)"/>
  <rect width="800" height="160" rx="14" fill="url(#scan)"/>

  <!-- ── subtle pulsing ambient light behind name ── -->
  <ellipse cx="400" cy="75" rx="260" ry="55" fill="#e8ff00" opacity="0">
    <animate attributeName="opacity" values="0;0.045;0;0.03;0" dur="3.6s" repeatCount="indefinite"/>
  </ellipse>
  <ellipse cx="400" cy="75" rx="180" ry="40" fill="#00f0ff" opacity="0">
    <animate attributeName="opacity" values="0;0.04;0;0.025;0" dur="4.2s" repeatCount="indefinite"/>
  </ellipse>

  <!-- ════════════════════════════════════════════════
       ALL NAME LAYERS — wrapped in the wipe clip
       so they all reveal together in a single sweep
       ════════════════════════════════════════════════ -->
  <g clip-path="url(#wipe)">

    <!-- LAYER A — magenta glitch shadow (jitters via x) -->
    <text text-anchor="middle" y="118"
          font-family="'Arial Black', 'Impact', sans-serif"
          font-size="120" font-weight="900"
          fill="#ff3cac" opacity="0.55" filter="url(#neon)" letter-spacing="8">
      <tspan>DEEPITH</tspan>
      <!-- x oscillates: 400 → 404 → 396 → 402 → 398 → 400 … -->
      <animate attributeName="x" values="400;404;396;402;398;400;401;397;403;400" dur="0.35s" repeatCount="indefinite" calcMode="discrete"/>
    </text>

    <!-- LAYER B — cyan glitch shadow (opposite phase) -->
    <text text-anchor="middle" y="118"
          font-family="'Arial Black', 'Impact', sans-serif"
          font-size="120" font-weight="900"
          fill="#00f0ff" opacity="0.45" filter="url(#neon)" letter-spacing="8">
      <tspan>DEEPITH</tspan>
      <animate attributeName="x" values="400;396;404;398;402;400;399;403;397;400" dur="0.35s" repeatCount="indefinite" calcMode="discrete"/>
    </text>

    <!-- LAYER C — main crisp white text (locked center, no jitter) -->
    <text x="400" text-anchor="middle" y="118"
          font-family="'Arial Black', 'Impact', sans-serif"
          font-size="120" font-weight="900"
          fill="#ffffff" filter="url(#glow)" letter-spacing="8">
      DEEPITH
    </text>

    <!-- LAYER D — neon yellow outline that pulses -->
    <text x="400" text-anchor="middle" y="118"
          font-family="'Arial Black', 'Impact', sans-serif"
          font-size="120" font-weight="900"
          fill="none" stroke="#e8ff00" stroke-width="1.5"
          filter="url(#neon)" letter-spacing="8" opacity="0.6">
      DEEPITH
      <animate attributeName="opacity"      values="0.6;0.9;0.4;0.85;0.6" dur="2.2s" repeatCount="indefinite"/>
      <animate attributeName="stroke-width" values="1.5;2.5;0.7;2;1.5"     dur="2.2s" repeatCount="indefinite"/>
    </text>

    <!-- LAYER E — random horizontal glitch bar that flickers across -->
    <rect x="0" width="800" height="6" fill="#e8ff00" opacity="0">
      <animate attributeName="opacity" values="0;0;0;0.3;0;0;0;0.18;0;0" dur="2s" repeatCount="indefinite" calcMode="discrete"/>
      <animate attributeName="y"       values="60;80;55;95;70;88;60;75;90;60" dur="2s" repeatCount="indefinite" calcMode="discrete"/>
    </rect>

  </g><!-- end wipe clip -->

  <!-- ── subtitle below name ── -->
  <text x="400" y="148" text-anchor="middle"
        font-family="'Courier New', monospace"
        font-size="13" fill="#e8ff00" letter-spacing="5" opacity="0.8">
    SOFTWARE DEVELOPER &amp; PROBLEM SOLVER
    <animate attributeName="opacity" values="0.8;0.45;0.8" dur="3s" repeatCount="indefinite"/>
  </text>

  <!-- ── corner code tags ── -->
  <text x="22"  y="26" font-family="monospace" font-size="10" fill="#ffffff" opacity="0.18">&lt;/&gt;</text>
  <text x="758" y="26" font-family="monospace" font-size="10" fill="#ffffff" opacity="0.18">&lt;/&gt;</text>
  <text x="22"  y="152" font-family="monospace" font-size="10" fill="#ffffff" opacity="0.18">&lt;/&gt;</text>
  <text x="758" y="152" font-family="monospace" font-size="10" fill="#ffffff" opacity="0.18">&lt;/&gt;</text>
</svg>

<!-- ████████████████████████████████████████████████████████████████████████
                         BADGE ROW
     ████████████████████████████████████████████████████████████████████████ -->

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/deepithn12042004)&nbsp;
[![Portfolio](https://img.shields.io/badge/Portfolio-255E63?style=for-the-badge&logo=react&logoColor=white)](https://deepith.me)&nbsp;
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/deepu0101/)

<br/>

<!-- ████████████████████████████████████████████████████████████████████████
              ANIMATED TYPING BAR — "I build things for the web."
     ████████████████████████████████████████████████████████████████████████ -->

<svg width="600" height="48" viewBox="0 0 600 48" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <filter id="softGlow">
      <feGaussianBlur stdDeviation="1.5" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>
  <rect width="600" height="48" rx="8" fill="#0d0d10"/>
  <rect width="600" height="48" rx="8" fill="none" stroke="#e8ff00" stroke-width="0.8" opacity="0.3"/>

  <!-- Three terminal dots -->
  <circle cx="22" cy="24" r="4.5" fill="#ff5f57"/>
  <circle cx="38" cy="24" r="4.5" fill="#febc2e"/>
  <circle cx="54" cy="24" r="4.5" fill="#28c840"/>

  <!-- Prompt -->
  <text x="76" y="29" font-family="'Courier New', monospace" font-size="15" fill="#e8ff00" opacity="0.7">&gt;</text>

  <!-- Typing text with reveal clip -->
  <defs>
    <clipPath id="typeClip">
      <rect x="0" y="0" width="0" height="48">
        <animate attributeName="width" values="0;520" dur="2.2s" begin="0.6s" fill="freeze" calcMode="ease-out"/>
      </rect>
    </clipPath>
  </defs>
  <text clip-path="url(#typeClip)" x="94" y="29"
        font-family="'Courier New', monospace" font-size="15" fill="#ffffff" filter="url(#softGlow)">
    I build things for the web. ✦
  </text>

  <!-- Blinking cursor — slides to end after text types, then blinks -->
  <rect x="94" y="16" width="2.5" height="20" fill="#e8ff00" rx="1">
    <animate attributeName="x" values="94;370" dur="2.2s" begin="0.6s" fill="freeze" calcMode="ease-out"/>
    <animate attributeName="opacity" values="1;0" dur="1s" repeatCount="indefinite"/>
  </rect>
</svg>

<br/><br/>

---

</div>

## 🧠 About Me

I'm a passionate **Software Developer** who loves turning complex problems into elegant, user-friendly solutions. I thrive at the intersection of clean code and creative design — building things that not only *work*, but *wow*.

When I'm not shipping features, you'll find me grinding problems on **LeetCode**, exploring new frameworks, or iterating on side projects that push boundaries.

---

## ⚡ Tech Stack

<div align="center">

<!-- Tech badges row -->

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

</div>

---

## 🔗 Connect With Me

<div align="center">

| Platform   | Link                                                                 |
|:----------:|:-------------------------------------------------------------------- |
| 💼 LinkedIn | [deepithn12042004](https://linkedin.com/in/deepithn12042004)       |
| 🌐 Portfolio | [deepith.me](https://deepith.me)                                   |
| 🧩 LeetCode  | [deepu0101](https://leetcode.com/u/deepu0101/)                     |

</div>

---

<div align="center">

<!-- ████████████████████████████████████████████████████████████████████████
                  ANIMATED FOOTER TAGLINE
     ████████████████████████████████████████████████████████████████████████ -->

<svg width="500" height="36" viewBox="0 0 500 36" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <filter id="fg">
      <feGaussianBlur stdDeviation="1.8" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>
  <text x="250" y="24" text-anchor="middle"
        font-family="'Courier New', monospace" font-size="13"
        fill="#e8ff00" filter="url(#fg)" letter-spacing="3" opacity="0.75">
    ✦ CRAFTING DIGITAL EXPERIENCES — ONE LINE AT A TIME ✦
    <animate attributeName="opacity" values="0.75;0.4;0.75" dur="3.5s" repeatCount="indefinite"/>
  </text>
</svg>

</div>
