<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 800 200" width="100%" height="200">
  <defs>
    <!-- Shifting dark animated gradient background -->
    <linearGradient id="bgGradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#1a001a">
        <animate attributeName="stop-color" values="#1a001a; #33001a; #1a001a" dur="4s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="#000000">
        <animate attributeName="stop-color" values="#000000; #1a001a; #000000" dur="4s" repeatCount="indefinite" />
      </stop>
    </linearGradient>
  </defs>

  <rect width="100%" height="100%" fill="url(#bgGradient)" rx="10" />

  <style>
    .neon-text {
      /* Uses Impact as it is web-safe and bold, similar to Anton */
      font-family: Impact, sans-serif;
      font-size: 85px;
      letter-spacing: 5px;
      fill: transparent;
      stroke: #F75C7E;
      stroke-width: 2px;
      stroke-dasharray: 400;
      stroke-dashoffset: 400;
      animation: drawText 4s ease-in-out infinite alternate;
    }

    @keyframes drawText {
      0% {
        stroke-dashoffset: 400;
        fill: transparent;
        filter: drop-shadow(0 0 2px #F75C7E);
      }
      40% {
        stroke-dashoffset: 0;
        fill: transparent;
        filter: drop-shadow(0 0 5px #F75C7E);
      }
      100% {
        stroke-dashoffset: 0;
        fill: #F75C7E;
        filter: drop-shadow(0 0 15px #F75C7E);
      }
    }
  </style>

  <!-- Animated Text -->
  <text x="50%" y="55%" dominant-baseline="middle" text-anchor="middle" class="neon-text">
    DEEPITH N
  </text>
</svg>
