<div align="center">

<!-- ████████████████████████████████████████████████████████████████████████
                    🔥 ANIMATED NAME BANNER — GLITCH + NEON + REVEAL 🔥
     ████████████████████████████████████████████████████████████████████████ -->

<svg width="800" height="200" viewBox="0 0 800 200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Neon glow filter -->
    <filter id="neon" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <!-- Sharper inner glow -->
    <filter id="glow2" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur stdDeviation="2" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <!-- Flicker animation for the glow layer -->
    <radialGradient id="bgGrad" cx="50%" cy="50%" r="70%">
      <stop offset="0%" stop-color="#0a0a0f"/>
      <stop offset="100%" stop-color="#020204"/>
    </radialGradient>
    <!-- Scanline pattern -->
    <pattern id="scanlines" patternUnits="userSpaceOnUse" width="800" height="4">
      <rect width="800" height="2" fill="rgba(0,0,0,0.15)"/>
    </pattern>
  </defs>

  <!-- Dark background -->
  <rect width="800" height="200" fill="url(#bgGrad)" rx="12"/>
  <!-- Subtle scanline overlay -->
  <rect width="800" height="200" fill="url(#scanlines)" rx="12" opacity="0.4"/>

  <!-- ── Ambient glow orbs ── -->
  <circle cx="120" cy="100" r="80" fill="#e8ff00" opacity="0.04">
    <animate attributeName="opacity" values="0.04;0.08;0.04" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="680" cy="100" r="90" fill="#ff3cac" opacity="0.04">
    <animate attributeName="opacity" values="0.04;0.07;0.04" dur="4s" repeatCount="indefinite"/>
  </circle>

  <!-- ──────────────────────────────────────────
         LAYER 1 — Red glitch copy (offset)
       ────────────────────────────────────────── -->
  <text x="400" y="138" text-anchor="middle"
        font-family="'Bebas Neue', 'Arial Black', sans-serif"
        font-size="130" font-weight="900" fill="#ff3cac" opacity="0.6"
        filter="url(#neon)" letter-spacing="14">
    DEEPITH
    <!-- Glitch horizontal shake -->
    <animateTransform attributeName="transform" type="translate"
      values="0,0  3,0  -2,0  0,0  -4,0  2,0  0,0"
      dur="0.3s" repeatCount="indefinite" calcMode="discrete"/>
  </text>

  <!-- ──────────────────────────────────────────
         LAYER 2 — Cyan glitch copy (offset opposite)
       ────────────────────────────────────────── -->
  <text x="400" y="138" text-anchor="middle"
        font-family="'Bebas Neue', 'Arial Black', sans-serif"
        font-size="130" font-weight="900" fill="#00f0ff" opacity="0.5"
        filter="url(#neon)" letter-spacing="14">
    DEEPITH
    <animateTransform attributeName="transform" type="translate"
      values="0,0  -3,0  4,0  0,0  2,0  -2,0  0,0"
      dur="0.3s" repeatCount="indefinite" calcMode="discrete"/>
  </text>

  <!-- ──────────────────────────────────────────
         LAYER 3 — Main bright neon text (stable)
       ────────────────────────────────────────── -->
  <text x="400" y="138" text-anchor="middle"
        font-family="'Bebas Neue', 'Arial Black', sans-serif"
        font-size="130" font-weight="900" fill="#ffffff"
        filter="url(#glow2)" letter-spacing="14">
    DEEPITH
  </text>

  <!-- ──────────────────────────────────────────
         LAYER 4 — Neon accent outline (pulsing)
       ────────────────────────────────────────── -->
  <text x="400" y="138" text-anchor="middle"
        font-family="'Bebas Neue', 'Arial Black', sans-serif"
        font-size="130" font-weight="900"
        fill="none" stroke="#e8ff00" stroke-width="1.2"
        filter="url(#neon)" letter-spacing="14" opacity="0.7">
    DEEPITH
    <animate attributeName="opacity" values="0.7;1;0.5;1;0.7" dur="2s" repeatCount="indefinite"/>
    <animate attributeName="stroke-width" values="1.2;2;0.8;1.5;1.2" dur="2s" repeatCount="indefinite"/>
  </text>

  <!-- ── Glitch clip rectangle that flickers across the text ── -->
  <rect x="0" y="85" width="800" height="8" fill="#e8ff00" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0.25;0;0;0;0.15;0" dur="1.8s" repeatCount="indefinite" calcMode="discrete"/>
    <animate attributeName="y" values="85;95;75;105;90;85" dur="1.8s" repeatCount="indefinite" calcMode="discrete"/>
  </rect>

  <!-- ── Subtitle ── -->
  <text x="400" y="172" text-anchor="middle"
        font-family="'Courier New', monospace"
        font-size="14" fill="#e8ff00" letter-spacing="6" opacity="0.85">
    SOFTWARE DEVELOPER &amp; PROBLEM SOLVER
    <animate attributeName="opacity" values="0.85;0.5;0.85" dur="3s" repeatCount="indefinite"/>
  </text>

  <!-- ── Corner decorations ── -->
  <text x="28" y="30" font-family="monospace" font-size="11" fill="#ffffff" opacity="0.2">&lt;/&gt;</text>
  <text x="740" y="30" font-family="monospace" font-size="11" fill="#ffffff" opacity="0.2">&lt;/&gt;</text>
  <text x="28" y="190" font-family="monospace" font-size="11" fill="#ffffff" opacity="0.2">&lt;/&gt;</text>
  <text x="740" y="190" font-family="monospace" font-size="11" fill="#ffffff" opacity="0.2">&lt;/&gt;</text>
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
