<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1280 740" width="1280" height="740">
  <defs>
    <clipPath id="roundedCorners">
      <rect width="1280" height="740" rx="24" ry="24"/>
    </clipPath>
    <linearGradient id="blueTeal" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#00b4d8"/>
      <stop offset="50%" stop-color="#0077b6"/>
      <stop offset="100%" stop-color="#023e8a"/>
    </linearGradient>
    <linearGradient id="blueTealAnim" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#00b4d8">
        <animate attributeName="stop-color" values="#00b4d8;#0077b6;#023e8a;#00b4d8" dur="4s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" stop-color="#023e8a">
        <animate attributeName="stop-color" values="#023e8a;#00b4d8;#0077b6;#023e8a" dur="4s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>
    <linearGradient id="scanLine" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="rgba(0,180,216,0)"/>
      <stop offset="45%" stop-color="rgba(0,180,216,0.3)"/>
      <stop offset="50%" stop-color="rgba(0,180,216,0.8)"/>
      <stop offset="55%" stop-color="rgba(0,180,216,0.3)"/>
      <stop offset="100%" stop-color="rgba(0,180,216,0)"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <filter id="neonGlow">
      <feGaussianBlur stdDeviation="6" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="1280" height="740" fill="#0a1929" clip-path="url(#roundedCorners)"/>
  <rect width="1280" height="740" fill="url(#blueTeal)" opacity="0.08" clip-path="url(#roundedCorners)"/>

  <!-- Ambient Orbs -->
  <circle cx="200" cy="150" r="120" fill="#00b4d8" opacity="0.06">
    <animate attributeName="r" values="120;140;120" dur="5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.06;0.1;0.06" dur="5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="1080" cy="550" r="150" fill="#023e8a" opacity="0.06">
    <animate attributeName="r" values="150;170;150" dur="7s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.06;0.1;0.06" dur="7s" repeatCount="indefinite"/>
  </circle>
  <circle cx="640" cy="370" r="200" fill="#0077b6" opacity="0.04">
    <animate attributeName="r" values="200;220;200" dur="6s" repeatCount="indefinite"/>
  </circle>

  <!-- Floating Hearts -->
  <g opacity="0.3">
    <text x="150" y="100" font-size="20" fill="#00b4d8">
      ♥
      <animate attributeName="y" values="100;80;100" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.3;0.6;0.3" dur="4s" repeatCount="indefinite"/>
    </text>
    <text x="1100" y="200" font-size="16" fill="#0077b6">
      ♥
      <animate attributeName="y" values="200;175;200" dur="5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.2;0.5;0.2" dur="5s" repeatCount="indefinite"/>
    </text>
    <text x="950" y="650" font-size="18" fill="#00b4d8">
      ♥
      <animate attributeName="y" values="650;630;650" dur="3.5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.3;0.7;0.3" dur="3.5s" repeatCount="indefinite"/>
    </text>
  </g>

  <!-- Twinkling Sparkles -->
  <g>
    <circle cx="300" cy="200" r="2" fill="#fff">
      <animate attributeName="opacity" values="0;1;0" dur="2s" repeatCount="indefinite"/>
    </circle>
    <circle cx="900" cy="150" r="2.5" fill="#fff">
      <animate attributeName="opacity" values="0;1;0" dur="2.5s" repeatCount="indefinite" begin="0.5s"/>
    </circle>
    <circle cx="500" cy="600" r="1.5" fill="#fff">
      <animate attributeName="opacity" values="0;1;0" dur="3s" repeatCount="indefinite" begin="1s"/>
    </circle>
    <circle cx="1150" cy="400" r="2" fill="#fff">
      <animate attributeName="opacity" values="0;1;0" dur="2.2s" repeatCount="indefinite" begin="0.3s"/>
    </circle>
    <circle cx="100" cy="500" r="1.8" fill="#fff">
      <animate attributeName="opacity" values="0;1;0" dur="2.8s" repeatCount="indefinite" begin="0.8s"/>
    </circle>
  </g>

  <!-- Rising Particles -->
  <g>
    <circle cx="200" cy="700" r="3" fill="#00b4d8" opacity="0.4">
      <animate attributeName="cy" values="700;300;700" dur="8s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.4;0;0.4" dur="8s" repeatCount="indefinite"/>
    </circle>
    <circle cx="600" cy="700" r="2" fill="#0077b6" opacity="0.3">
      <animate attributeName="cy" values="700;250;700" dur="10s" repeatCount="indefinite" begin="2s"/>
      <animate attributeName="opacity" values="0.3;0;0.3" dur="10s" repeatCount="indefinite" begin="2s"/>
    </circle>
    <circle cx="1000" cy="700" r="2.5" fill="#023e8a" opacity="0.35">
      <animate attributeName="cy" values="700;200;700" dur="9s" repeatCount="indefinite" begin="4s"/>
      <animate attributeName="opacity" values="0.35;0;0.35" dur="9s" repeatCount="indefinite" begin="4s"/>
    </circle>
  </g>

  <!-- Terminal Line -->
  <g font-family="'Courier New', monospace" font-size="18" fill="#00e5ff">
    <text x="60" y="60">
      user@dev:~$ 
      <tspan fill="#00b4d8">cat README.md</tspan>
      <tspan>
        <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/>
        ▊
      </tspan>
    </text>
  </g>

  <!-- Name with Animated Gradient and Letter Pop-in -->
  <g font-family="'Georgia', serif" font-size="64" font-weight="bold" filter="url(#glow)">
    <text x="60" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="0.5s" fill="freeze"/>
      D
    </text>
    <text x="115" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="0.7s" fill="freeze"/>
      i
    </text>
    <text x="140" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="0.9s" fill="freeze"/>
      s
    </text>
    <text x="170" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1.1s" fill="freeze"/>
      h
    </text>
    <text x="210" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1.3s" fill="freeze"/>
      i
    </text>
    <text x="240" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1.5s" fill="freeze"/>
      &nbsp;
    </text>
    <text x="260" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1.7s" fill="freeze"/>
      N
    </text>
    <text x="310" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1.9s" fill="freeze"/>
      e
    </text>
    <text x="340" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="2.1s" fill="freeze"/>
      e
    </text>
    <text x="370" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="2.3s" fill="freeze"/>
      k
    </text>
    <text x="400" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="2.5s" fill="freeze"/>
      h
    </text>
    <text x="435" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="2.7s" fill="freeze"/>
      r
    </text>
    <text x="460" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="2.9s" fill="freeze"/>
      a
    </text>
  </g>

  <!-- Cycling Role Titles -->
  <g font-family="'Courier New', monospace" font-size="24" fill="#0077b6">
    <text x="60" y="210">
      <animate attributeName="opacity" values="0;1;1;0" dur="8s" repeatCount="indefinite"/>
      ▸ Full-Stack Developer
    </text>
    <text x="60" y="210" opacity="0">
      <animate attributeName="opacity" values="0;0;1;1;0" dur="8s" repeatCount="indefinite" begin="2s"/>
      ▸ AI/ML Enthusiast
    </text>
    <text x="60" y="210" opacity="0">
      <animate attributeName="opacity" values="0;0;1;1;0" dur="8s" repeatCount="indefinite" begin="4s"/>
      ▸ Gen AI Learner
    </text>
    <text x="60" y="210" opacity="0">
      <animate attributeName="opacity" values="0;0;1;1;0" dur="8s" repeatCount="indefinite" begin="6s"/>
      ▸ Open Source Contributor
    </text>
  </g>

  <!-- Tagline Quote Box -->
  <g>
    <rect x="60" y="240" width="500" height="50" rx="8" fill="#0d2137" stroke="#00b4d8" stroke-width="1" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="3.5s" fill="freeze"/>
    </rect>
    <text x="80" y="272" font-family="'Georgia', serif" font-size="18" fill="#b0d4e8" font-style="italic" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="3.8s" fill="freeze"/>
      "Code. Learn. Build. Repeat."
    </text>
  </g>

  <!-- Tech Stack Pills -->
  <g font-family="'Courier New', monospace" font-size="13">
    <!-- Row 1 -->
    <g>
      <rect x="60" y="320" width="80" height="28" rx="14" fill="#00b4d8" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4s" fill="freeze"/>
      </rect>
      <text x="100" y="339" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4s" fill="freeze"/>
        HTML
      </text>
    </g>
    <g>
      <rect x="150" y="320" width="80" height="28" rx="14" fill="#0077b6" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.2s" fill="freeze"/>
      </rect>
      <text x="190" y="339" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.2s" fill="freeze"/>
        CSS
      </text>
    </g>
    <g>
      <rect x="240" y="320" width="100" height="28" rx="14" fill="#023e8a" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.4s" fill="freeze"/>
      </rect>
      <text x="290" y="339" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.4s" fill="freeze"/>
        JavaScript
      </text>
    </g>
    <g>
      <rect x="350" y="320" width="90" height="28" rx="14" fill="#00b4d8" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.6s" fill="freeze"/>
      </rect>
      <text x="395" y="339" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.6s" fill="freeze"/>
        React
      </text>
    </g>
    <g>
      <rect x="450" y="320" width="120" height="28" rx="14" fill="#0077b6" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.8s" fill="freeze"/>
      </rect>
      <text x="510" y="339" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.8s" fill="freeze"/>
        Tailwind CSS
      </text>
    </g>
    <!-- Row 2 -->
    <g>
      <rect x="60" y="360" width="80" height="28" rx="14" fill="#023e8a" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5s" fill="freeze"/>
      </rect>
      <text x="100" y="379" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5s" fill="freeze"/>
        C++
      </text>
    </g>
    <g>
      <rect x="150" y="360" width="90" height="28" rx="14" fill="#00b4d8" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.2s" fill="freeze"/>
      </rect>
      <text x="195" y="379" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.2s" fill="freeze"/>
        Python
      </text>
    </g>
    <g>
      <rect x="250" y="360" width="70" height="28" rx="14" fill="#0077b6" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.4s" fill="freeze"/>
      </rect>
      <text x="285" y="379" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.4s" fill="freeze"/>
        Git
      </text>
    </g>
    <g>
      <rect x="330" y="360" width="90" height="28" rx="14" fill="#023e8a" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.6s" fill="freeze"/>
      </rect>
      <text x="375" y="379" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.6s" fill="freeze"/>
        GitHub
      </text>
    </g>
  </g>

  <!-- About Me Lines -->
  <g font-family="'Courier New', monospace" font-size="15" fill="#80b0c8">
    <text x="60" y="430" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="6s" fill="freeze"/>
      // About Me
    </text>
    <text x="60" y="455" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="6.3s" fill="freeze"/>
      const developer = {
    </text>
    <text x="80" y="478" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="6.6s" fill="freeze"/>
      name: "Dishi Neekhra",
    </text>
    <text x="80" y="501" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="6.9s" fill="freeze"/>
      role: "Full-Stack Developer & AI/ML Enthusiast",
    </text>
    <text x="80" y="524" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="7.2s" fill="freeze"/>
      passion: "Building things that matter",
    </text>
    <text x="60" y="547" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="7.5s" fill="freeze"/>
      };
    </text>
  </g>

  <!-- Animated Stats Bar -->
  <g opacity="0">
    <animate attributeName="opacity" values="0;1" dur="0.5s" begin="8s" fill="freeze"/>
    <text x="60" y="590" font-family="'Courier New', monospace" font-size="14" fill="#00b4d8">Stats</text>
    <rect x="60" y="600" width="500" height="8" rx="4" fill="#0d2137"/>
    <rect x="60" y="600" width="0" height="8" rx="4" fill="url(#blueTeal)">
      <animate attributeName="width" values="0;350" dur="1.5s" begin="8.5s" fill="freeze"/>
    </rect>
    <text x="570" y="608" font-family="'Courier New', monospace" font-size="12" fill="#b0d4e8">Repos: 70%</text>
  </g>

  <!-- Code Editor Card -->
  <g>
    <rect x="60" y="630" width="500" height="90" rx="8" fill="#0a1929" stroke="#0077b6" stroke-width="1" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="9s" fill="freeze"/>
    </rect>
    <g font-family="'Courier New', monospace" font-size="13" fill="#b0d4e8">
      <text x="80" y="655" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="9.5s" fill="freeze"/>
        <tspan fill="#00b4d8">function</tspan> <tspan fill="#0077b6">buildDreams</tspan>() {
      </text>
      <text x="100" y="678" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="10s" fill="freeze"/>
        <tspan fill="#023e8a">return</tspan> (
      </text>
      <text x="120" y="701" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="10.5s" fill="freeze"/>
        &lt;<tspan fill="#00b4d8">div</tspan>&gt;✨ <tspan fill="#00e5ff">"Code. Learn. Build. Repeat."</tspan> ✨&lt;/<tspan fill="#00b4d8">div</tspan>&gt;
      </text>
    </g>
  </g>

  <!-- Neon Sign -->
  <g filter="url(#neonGlow)">
    <text x="900" y="680" font-family="'Georgia', serif" font-size="28" fill="#00b4d8" text-anchor="middle" opacity="0">
      <animate attributeName="opacity" values="0;1;0.8;1;0.9;1" dur="3s" begin="11s" fill="freeze"/>
      KEEP CODING KEEP GROWING
    </text>
  </g>

  <!-- Character Image (Base64 placeholder) -->
  <g clip-path="url(#roundedCorners)">
    <!-- Hologram Formation -->
    <g>
      <animate attributeName="opacity" values="0;1" dur="2s" begin="0.5s" fill="freeze"/>
      <!-- Scan line effect -->
      <rect x="700" y="0" width="580" height="740" fill="url(#scanLine)">
        <animate attributeName="y" values="-740;0" dur="1.5s" begin="0.5s" fill="freeze"/>
      </rect>
      <!-- Image placeholder -->
      <image href="data:image/png;base64,YOUR_BASE64_IMAGE_HERE" x="700" y="50" width="500" height="640" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="1s" begin="1.5s" fill="freeze"/>
      </image>
    </g>

    <!-- Continuous Scanner -->
    <rect x="700" y="0" width="580" height="3" fill="url(#scanLine)" opacity="0.6">
      <animate attributeName="y" values="-740;740" dur="3.5s" repeatCount="indefinite" begin="2s"/>
    </rect>
  </g>
</svg>


<br>
&lt;svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1280 740" width="1280" height="740"&gt;
  <defs>
    <clipPath id="roundedCorners">
      <rect width="1280" height="740" rx="24" ry="24"/>
    </clipPath>
    <linearGradient id="blueTeal" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#00b4d8"/>
      <stop offset="50%" stop-color="#0077b6"/>
      <stop offset="100%" stop-color="#023e8a"/>
    </linearGradient>
    <linearGradient id="blueTealAnim" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#00b4d8">
        <animate attributeName="stop-color" values="#00b4d8;#0077b6;#023e8a;#00b4d8" dur="4s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" stop-color="#023e8a">
        <animate attributeName="stop-color" values="#023e8a;#00b4d8;#0077b6;#023e8a" dur="4s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>
    <linearGradient id="scanLine" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="rgba(0,180,216,0)"/>
      <stop offset="45%" stop-color="rgba(0,180,216,0.15)"/>
      <stop offset="50%" stop-color="rgba(0,180,216,0.4)"/>
      <stop offset="55%" stop-color="rgba(0,180,216,0.15)"/>
      <stop offset="100%" stop-color="rgba(0,180,216,0)"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <filter id="neonGlow">
      <feGaussianBlur stdDeviation="6" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- Background - Light -->
  <rect width="1280" height="740" fill="#ffffff" clip-path="url(#roundedCorners)"/>
  <rect width="1280" height="740" fill="url(#blueTeal)" opacity="0.04" clip-path="url(#roundedCorners)"/>

  <!-- Ambient Orbs -->
  <circle cx="200" cy="150" r="120" fill="#00b4d8" opacity="0.04">
    <animate attributeName="r" values="120;140;120" dur="5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.04;0.07;0.04" dur="5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="1080" cy="550" r="150" fill="#023e8a" opacity="0.04">
    <animate attributeName="r" values="150;170;150" dur="7s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.04;0.07;0.04" dur="7s" repeatCount="indefinite"/>
  </circle>

  <!-- Floating Hearts -->
  <g opacity="0.2">
    <text x="150" y="100" font-size="20" fill="#00b4d8">
      ♥
      <animate attributeName="y" values="100;80;100" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.2;0.4;0.2" dur="4s" repeatCount="indefinite"/>
    </text>
    <text x="1100" y="200" font-size="16" fill="#0077b6">
      ♥
      <animate attributeName="y" values="200;175;200" dur="5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.15;0.35;0.15" dur="5s" repeatCount="indefinite"/>
    </text>
  </g>

  <!-- Twinkling Sparkles -->
  <g>
    <circle cx="300" cy="200" r="2" fill="#0077b6">
      <animate attributeName="opacity" values="0;0.6;0" dur="2s" repeatCount="indefinite"/>
    </circle>
    <circle cx="900" cy="150" r="2.5" fill="#023e8a">
      <animate attributeName="opacity" values="0;0.6;0" dur="2.5s" repeatCount="indefinite" begin="0.5s"/>
    </circle>
    <circle cx="1150" cy="400" r="2" fill="#00b4d8">
      <animate attributeName="opacity" values="0;0.6;0" dur="2.2s" repeatCount="indefinite" begin="0.3s"/>
    </circle>
  </g>

  <!-- Terminal Line -->
  <g font-family="'Courier New', monospace" font-size="18" fill="#0a1929">
    <text x="60" y="60">
      user@dev:~$ 
      <tspan fill="#00b4d8">cat README.md</tspan>
      <tspan>
        <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/>
        ▊
      </tspan>
    </text>
  </g>

  <!-- Name -->
  <g font-family="'Georgia', serif" font-size="64" font-weight="bold" filter="url(#glow)">
    <text x="60" y="160" fill="url(#blueTealAnim)">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="0.5s" fill="freeze"/>
      Dishi Neekhra
    </text>
  </g>

  <!-- Cycling Role Titles -->
  <g font-family="'Courier New', monospace" font-size="24" fill="#0077b6">
    <text x="60" y="210">
      <animate attributeName="opacity" values="0;1;1;0" dur="8s" repeatCount="indefinite"/>
      ▸ Full-Stack Developer
    </text>
    <text x="60" y="210" opacity="0">
      <animate attributeName="opacity" values="0;0;1;1;0" dur="8s" repeatCount="indefinite" begin="2s"/>
      ▸ AI/ML Enthusiast
    </text>
    <text x="60" y="210" opacity="0">
      <animate attributeName="opacity" values="0;0;1;1;0" dur="8s" repeatCount="indefinite" begin="4s"/>
      ▸ Gen AI Learner
    </text>
    <text x="60" y="210" opacity="0">
      <animate attributeName="opacity" values="0;0;1;1;0" dur="8s" repeatCount="indefinite" begin="6s"/>
      ▸ Open Source Contributor
    </text>
  </g>

  <!-- Tagline Quote Box -->
  <g>
    <rect x="60" y="240" width="500" height="50" rx="8" fill="#f0f8ff" stroke="#00b4d8" stroke-width="1" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="3.5s" fill="freeze"/>
    </rect>
    <text x="80" y="272" font-family="'Georgia', serif" font-size="18" fill="#0a1929" font-style="italic" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="3.8s" fill="freeze"/>
      "Code. Learn. Build. Repeat."
    </text>
  </g>

  <!-- Tech Stack Pills -->
  <g font-family="'Courier New', monospace" font-size="13">
    <g>
      <rect x="60" y="320" width="80" height="28" rx="14" fill="#00b4d8" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4s" fill="freeze"/>
      </rect>
      <text x="100" y="339" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4s" fill="freeze"/>
        HTML
      </text>
    </g>
    <g>
      <rect x="150" y="320" width="80" height="28" rx="14" fill="#0077b6" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.2s" fill="freeze"/>
      </rect>
      <text x="190" y="339" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.2s" fill="freeze"/>
        CSS
      </text>
    </g>
    <g>
      <rect x="240" y="320" width="100" height="28" rx="14" fill="#023e8a" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.4s" fill="freeze"/>
      </rect>
      <text x="290" y="339" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.4s" fill="freeze"/>
        JavaScript
      </text>
    </g>
    <g>
      <rect x="350" y="320" width="90" height="28" rx="14" fill="#00b4d8" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.6s" fill="freeze"/>
      </rect>
      <text x="395" y="339" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.6s" fill="freeze"/>
        React
      </text>
    </g>
    <g>
      <rect x="450" y="320" width="120" height="28" rx="14" fill="#0077b6" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.8s" fill="freeze"/>
      </rect>
      <text x="510" y="339" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.8s" fill="freeze"/>
        Tailwind CSS
      </text>
    </g>
    <g>
      <rect x="60" y="360" width="80" height="28" rx="14" fill="#023e8a" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5s" fill="freeze"/>
      </rect>
      <text x="100" y="379" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5s" fill="freeze"/>
        C++
      </text>
    </g>
    <g>
      <rect x="150" y="360" width="90" height="28" rx="14" fill="#00b4d8" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.2s" fill="freeze"/>
      </rect>
      <text x="195" y="379" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.2s" fill="freeze"/>
        Python
      </text>
    </g>
    <g>
      <rect x="250" y="360" width="70" height="28" rx="14" fill="#0077b6" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.4s" fill="freeze"/>
      </rect>
      <text x="285" y="379" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.4s" fill="freeze"/>
        Git
      </text>
    </g>
    <g>
      <rect x="330" y="360" width="90" height="28" rx="14" fill="#023e8a" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.6s" fill="freeze"/>
      </rect>
      <text x="375" y="379" text-anchor="middle" fill="#fff" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.6s" fill="freeze"/>
        GitHub
      </text>
    </g>
  </g>

  <!-- About Me Lines -->
  <g font-family="'Courier New', monospace" font-size="15" fill="#444">
    <text x="60" y="430" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="6s" fill="freeze"/>
      // About Me
    </text>
    <text x="60" y="455" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="6.3s" fill="freeze"/>
      const developer = {
    </text>
    <text x="80" y="478" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="6.6s" fill="freeze"/>
      name: "Dishi Neekhra",
    </text>
    <text x="80" y="501" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="6.9s" fill="freeze"/>
      role: "Full-Stack Developer & AI/ML Enthusiast",
    </text>
    <text x="80" y="524" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="7.2s" fill="freeze"/>
      passion: "Building things that matter",
    </text>
    <text x="60" y="547" opacity="0">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="7.5s" fill="freeze"/>
      };
    </text>
  </g>

  <!-- Animated Stats Bar -->
  <g opacity="0">
    <animate attributeName="opacity" values="0;1" dur="0.5s" begin="8s" fill="freeze"/>
    <text x="60" y="590" font-family="
<br>

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 300 500" width="300" height="500">
  <defs>
    <linearGradient id="holographic" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="rgba(0,180,216,0.3)"/>
      <stop offset="25%" stop-color="rgba(0,119,182,0.2)"/>
      <stop offset="50%" stop-color="rgba(2,62,138,0.3)"/>
      <stop offset="75%" stop-color="rgba(0,180,216,0.2)"/>
      <stop offset="100%" stop-color="rgba(0,119,182,0.3)"/>
    </linearGradient>
    <linearGradient id="strapGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00b4d8"/>
      <stop offset="50%" stop-color="#0077b6"/>
      <stop offset="100%" stop-color="#00b4d8"/>
    </linearGradient>
    <clipPath id="cardClip">
      <rect x="50" y="120" width="200" height="280" rx="12"/>
    </clipPath>
    <filter id="glowRing">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- Swing Animation Group -->
  <g>
    <animateTransform attributeName="transform" type="rotate" values="-8,150,0;6,150,0;-4,150,0;2,150,0;-1,150,0;0,150,0" dur="3s" repeatCount="indefinite" calcMode="spline" keySplines="0.4 0 0.6 1;0.4 0 0.6 1;0.4 0 0.6 1;0.4 0 0.6 1;0.4 0 0.6 1"/>
    
    <!-- Drop-in Animation -->
    <g>
      <animateTransform attributeName="transform" type="translate" values="0,-500;0,0" dur="1.5s" fill="freeze" calcMode="spline" keySplines="0.25 0.1 0.25 1"/>
      
      <!-- Strap -->
      <rect x="140" y="0" width="20" height="130" rx="10" fill="url(#strapGrad)"/>
      <text x="150" y="65" text-anchor="middle" font-family="'Courier New', monospace" font-size="8" fill="#fff" transform="rotate(90,150,65)">DISHI-GLITCH</text>
      
      <!-- Metal Clasp -->
      <rect x="135" y="100" width="30" height="15" rx="3" fill="#c0c0c0" stroke="#888" stroke-width="1"/>
      <rect x="140" y="108" width="20" height="4" rx="2" fill="#999"/>
      
      <!-- Metal Ring -->
      <circle cx="150" cy="118" r="6" fill="none" stroke="#c0c0c0" stroke-width="3"/>
      
      <!-- Card Body -->
      <rect x="50" y="120" width="200" height="280" rx="12" fill="#0a1929" stroke="#00b4d8" stroke-width="2"/>
      
      <!-- Holographic Shine Sweep -->
      <rect x="50" y="120" width="200" height="280" rx="12" fill="url(#holographic)" clip-path="url(#cardClip)">
        <animate attributeName="x" values="-200;400" dur="4s" repeatCount="indefinite"/>
      </rect>
      
      <!-- Avatar Ring -->
      <circle cx="150" cy="200" r="45" fill="none" stroke="#00b4d8" stroke-width="3" filter="url(#glowRing)">
        <animate attributeName="stroke" values="#00b4d8;#0077b6;#023e8a;#00b4d8" dur="3s" repeatCount="indefinite"/>
      </circle>
      
      <!-- Avatar Image Placeholder -->
      <clipPath id="avatarClip">
        <circle cx="150" cy="200" r="40"/>
      </clipPath>
      <image href="data:image/png;base64,YOUR_BASE64_IMAGE_HERE" x="110" y="160" width="80" height="80" clip-path="url(#avatarClip)"/>
      
      <!-- Name -->
      <text x="150" y="270" text-anchor="middle" font-family="'Georgia', serif" font-size="16" font-weight="bold" fill="#00b4d8">Dishi Neekhra</text>
      
      <!-- Role -->
      <text x="150" y="290" text-anchor="middle" font-family="'Courier New', monospace" font-size="10" fill="#80b0c8">Full-Stack Developer</text>
      
      <!-- Handle -->
      <text x="150" y="310" text-anchor="middle" font-family="'Courier New', monospace" font-size="9" fill="#0077b6">@Dishi-glitch</text>
      
      <!-- Barcode -->
      <g transform="translate(75, 340)">
        <rect x="0" y="0" width="2" height="30" fill="#fff"/>
        <rect x="4" y="0" width="1" height="30" fill="#fff"/>
        <rect x="7" y="0" width="3" height="30" fill="#fff"/>
        <rect x="12" y="0" width="1" height="30" fill="#fff"/>
        <rect x="15" y="0" width="2" height="30" fill="#fff"/>
        <rect x="19" y="0" width="1" height="30" fill="#fff"/>
        <rect x="22" y="0" width="3" height="30" fill="#fff"/>
        <rect x="27" y="0" width="1" height="30" fill="#fff"/>
        <rect x="30" y="0" width="2" height="30" fill="#fff"/>
        <rect x="34" y="0" width="1" height="30" fill="#fff"/>
        <rect x="37" y="0" width="3" height="30" fill="#fff"/>
        <rect x="42" y="0" width="1" height="30" fill="#fff"/>
        <rect x="45" y="0" width="2" height="30" fill="#fff"/>
        <rect x="49" y="0" width="1" height="30" fill="#fff"/>
        <rect x="52" y="0" width="3" height="30" fill="#fff"/>
        <rect x="57" y="0" width="1" height="30" fill="#fff"/>
        <rect x="60" y="0" width="2" height="30" fill="#fff"/>
        <rect x="64" y="0" width="1" height="30" fill="#fff"/>
        <rect x="67" y="0" width="3" height="30" fill="#fff"/>
        <rect x="72" y="0" width="1" height="30" fill="#fff"/>
        <rect x="75" y="0" width="2" height="30" fill="#fff"/>
        <rect x="79" y="0" width="1" height="30" fill="#fff"/>
        <rect x="82" y="0" width="3" height="30" fill="#fff"/>
        <rect x="87" y="0" width="1" height="30" fill="#fff"/>
        <rect x="90" y="0" width="2" height="30" fill="#fff"/>
        <rect x="94" y="0" width="1" height="30" fill="#fff"/>
        <rect x="97" y="0" width="3" height="30" fill="#fff"/>
        <rect x="102" y="0" width="1" height="30" fill="#fff"/>
        <rect x="105" y="0" width="2" height="30" fill="#fff"/>
        <rect x="109" y="0" width="1" height="30" fill="#fff"/>
        <rect x="112" y="0" width="3" height="30" fill="#fff"/>
        <rect x="117" y="0" width="1" height="30" fill="#fff"/>
        <rect x="120" y="0" width="2" height="30" fill="#fff"/>
      </g>
      
      <!-- Bottom text -->
      <text x="150" y="390" text-anchor="middle" font-family="'Courier New', monospace" font-size="7" fill="#444">Code. Learn. Build. Repeat.</text>
    </g>
  </g>
</svg>

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 400 300" width="400" height="300">
  <defs>
    <linearGradient id="blueGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#00b4d8"/>
      <stop offset="100%" stop-color="#023e8a"/>
    </linearGradient>
  </defs>
  
  <rect width="400" height="300" fill="#0a1929" rx="16"/>
  
  <!-- Rank Ring -->
  <g transform="translate(80, 130)">
    <circle cx="0" cy="0" r="60" fill="none" stroke="#0d2137" stroke-width="8"/>
    <circle cx="0" cy="0" r="60" fill="none" stroke="url(#blueGrad)" stroke-width="8" stroke-dasharray="377" stroke-dashoffset="377" stroke-linecap="round">
      <animate attributeName="stroke-dashoffset" values="377;113" dur="2s" fill="freeze"/>
    </circle>
    <text x="0" y="-10" text-anchor="middle" font-family="'Georgia', serif" font-size="28" font-weight="bold" fill="#00b4d8">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1.5s" fill="freeze"/>
      A
    </text>
    <text x="0" y="15" text-anchor="middle" font-family="'Courier New', monospace" font-size="10" fill="#80b0c8">
      <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1.8s" fill="freeze"/>
      RANK
    </text>
  </g>
  
  <!-- Stats Rows -->
  <g font-family="'Courier New', monospace" font-size="13">
    <!-- Repos -->
    <g transform="translate(180, 80)">
      <text x="0" y="0" fill="#80b0c8" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="2s" fill="freeze"/>
        Repositories
      </text>
      <text x="180" y="0" fill="#00b4d8" text-anchor="end" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="2.2s" fill="freeze"/>
        12
      </text>
      <rect x="0" y="8" width="180" height="4" rx="2" fill="#0d2137" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="2.4s" fill="freeze"/>
      </rect>
      <rect x="0" y="8" width="0" height="4" rx="2" fill="url(#blueGrad)" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="2.6s" fill="freeze"/>
        <animate attributeName="width" values="0;126" dur="1s" begin="2.6s" fill="freeze"/>
      </rect>
    </g>
    
    <!-- Stars -->
    <g transform="translate(180, 120)">
      <text x="0" y="0" fill="#80b0c8" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="2.8s" fill="freeze"/>
        Stars
      </text>
      <text x="180" y="0" fill="#00b4d8" text-anchor="end" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="3s" fill="freeze"/>
        8
      </text>
      <rect x="0" y="8" width="180" height="4" rx="2" fill="#0d2137" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="3.2s" fill="freeze"/>
      </rect>
      <rect x="0" y="8" width="0" height="4" rx="2" fill="url(#blueGrad)" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="3.4s" fill="freeze"/>
        <animate attributeName="width" values="0;90" dur="1s" begin="3.4s" fill="freeze"/>
      </rect>
    </g>
    
    <!-- Contributions -->
    <g transform="translate(180, 160)">
      <text x="0" y="0" fill="#80b0c8" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="3.6s" fill="freeze"/>
        Contributions
      </text>
      <text x="180" y="0" fill="#00b4d8" text-anchor="end" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="3.8s" fill="freeze"/>
        156
      </text>
      <rect x="0" y="8" width="180" height="4" rx="2" fill="#0d2137" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="4s" fill="freeze"/>
      </rect>
      <rect x="0" y="8" width="0" height="4" rx="2" fill="url(#blueGrad)" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="4.2s" fill="freeze"/>
        <animate attributeName="width" values="0;108" dur="1s" begin="4.2s" fill="freeze"/>
      </rect>
    </g>
    
    <!-- Followers -->
    <g transform="translate(180, 200)">
      <text x="0" y="0" fill="#80b0c8" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="4.4s" fill="freeze"/>
        Followers
      </text>
      <text x="180" y="0" fill="#00b4d8" text-anchor="end" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="4.6s" fill="freeze"/>
        5
      </text>
      <rect x="0" y="8" width="180" height="4" rx="2" fill="#0d2137" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="4.8s" fill="freeze"/>
      </rect>
      <rect x="0" y="8" width="0" height="4" rx="2" fill="url(#blueGrad)" opacity="0">
        <animate attributeName="opacity" values="0;1" dur="0.3s" begin="5s" fill="freeze"/>
        <animate attributeName="width" values="0;72" dur="1s" begin="5s" fill="freeze"/>
      </rect>
    </g>
  </g>
</svg>

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 400 300" width="400" height="300">
  <defs>
    <linearGradient id="htmlGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00b4d8"/>
      <stop offset="100%" stop-color="#0077b6"/>
    </linearGradient>
    <linearGradient id="cssGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#0077b6"/>
      <stop offset="100%" stop-color="#023e8a"/>
    </linearGradient>
    <linearGradient id="jsGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#023e8a"/>
      <stop offset="100%" stop-color="#00b4d8"/>
    </linearGradient>
    <linearGradient id="pyGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00b4d8"/>
      <stop offset="100%" stop-color="#023e8a"/>
    </linearGradient>
    <linearGradient id="cppGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#0077b6"/>
      <stop offset="100%" stop-color="#00b4d8"/>
    </linearGradient>
  </defs>
  
  <rect width="400" height="300" fill="#0a1929" rx="16"/>
  
  <text x="200" y="40" text-anchor="middle" font-family="'Georgia', serif" font-size="18" font-weight="bold" fill="#00b4d8">Most Used Languages</text>
  
  <g font-family="'Courier New', monospace" font-size="12">
    <!-- HTML -->
    <g transform="translate(30, 80)">
      <text x="0" y="0" fill="#80b0c8">HTML</text>
      <text x="340" y="0" fill="#00b4d8" text-anchor="end">35%</text>
      <rect x="0" y="8" width="340" height="12" rx="6" fill="#0d2137"/>
      <rect x="0" y="8" width="0" height="12" rx="6" fill="url(#htmlGrad)">
        <animate attributeName="width" values="0;119" dur="1.5s" fill="freeze"/>
      </rect>
    </g>
    
    <!-- CSS -->
    <g transform="translate(30, 115)">
      <text x="0" y="0" fill="#80b0c8">CSS</text>
      <text x="340" y="0" fill="#00b4d8" text-anchor="end">25%</text>
      <rect x="0" y="8" width="340" height="12" rx="6" fill="#0d2137"/>
      <rect x="0" y="8" width="0" height="12" rx="6" fill="url(#cssGrad)">
        <animate attributeName="width" values="0;85" dur="1.5s" begin="0.3s" fill="freeze"/>
      </rect>
    </g>
    
    <!-- JavaScript -->
    <g transform="translate(30, 150)">
      <text x="0" y="0" fill="#80b0c8">JavaScript</text>
      <text x="340" y="0" fill="#00b4d8" text-anchor="end">20%</text>
      <rect x="0" y="8" width="340" height="12" rx="6" fill="#0d2137"/>
      <rect x="0" y="8" width="0" height="12" rx="6" fill="url(#jsGrad)">
        <animate attributeName="width" values="0;68" dur="1.5s" begin="0.6s" fill="freeze"/>
      </rect>
    </g>
    
    <!-- Python -->
    <g transform="translate(30, 185)">
      <text x="0" y="0" fill="#80b0c8">Python</text>
      <text x="340" y="0" fill="#00b4d8" text-anchor="end">12%</text>
      <rect x="0" y="8" width="340" height="12" rx="6" fill="#0d2137"/>
      <rect x="0" y="8" width="0" height="12" rx="6" fill="url(#pyGrad)">
        <animate attributeName="width" values="0;41" dur="1.5s" begin="0.9s" fill="freeze"/>
      </rect>
    </g>
    
    <!-- C++ -->
    <g transform="translate(30, 220)">
      <text x="0" y="0" fill="#80b0c8">C++</text>
      <text x="340" y="0" fill="#00b4d8" text-anchor="end">8%</text>
      <rect x="0" y="8" width="340" height="12" rx="6" fill="#0d2137"/>
      <rect x="0" y="8" width="0" height="12" rx="6" fill="url(#cppGrad)">
        <animate attributeName="width" values="0;27" dur="1.5s" begin="1.2s" fill="freeze"/>
      </rect>
    </g>
  </g>
</svg>

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 500 200" width="500" height="200">
  <defs>
    <linearGradient id="shineSweep" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(0,180,216,0)"/>
      <stop offset="50%" stop-color="rgba(0,180,216,0.3)"/>
      <stop offset="100%" stop-color="rgba(0,180,216,0)"/>
    </linearGradient>
    <linearGradient id="goldGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#ffd700"/>
      <stop offset="100%" stop-color="#ff8c00"/>
    </linearGradient>
    <linearGradient id="silverGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#e0e0e0"/>
      <stop offset="100%" stop-color="#a0a0a0"/>
    </linearGradient>
    <linearGradient id="bronzeGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#cd7f32"/>
      <stop offset="100%" stop-color="#8b4513"/>
    </linearGradient>
  </defs>
  
  <rect width="500" height="200" fill="#0a1929" rx="16"/>
  
  <!-- Shine Sweep -->
  <rect x="-500" y="0" width="500" height="200" fill="url(#shineSweep)">
    <animate attributeName="x" values="-500;500" dur="4s" repeatCount="indefinite"/>
  </rect>
  
  <!-- Trophy 1 - Gold -->
  <g transform="translate(50, 40)" opacity="0">
    <animate attributeName="opacity" values="0;1" dur="0.5s" begin="0.5s" fill="freeze"/>
    <rect x="0" y="0" width="120" height="130" rx="10" fill="#0d2137" stroke="#ffd700" stroke-width="1"/>
    <text x="60" y="40" text-anchor="middle" font-size="30">🏆</text>
    <text x="60" y="70" text-anchor="middle" font-family="'Courier New', monospace" font-size="12" fill="#ffd700" font-weight="bold">Gold</text>
    <text x="60" y="90" text-anchor="middle" font-family="'Courier New', monospace" font-size="10" fill="#80b0c8">Top Contributor</text>
    <text x="60" y="115" text-anchor="middle" font-family="'Courier New', monospace" font-size="9" fill="#ffd700">#1</text>
  </g>
  
  <!-- Trophy 2 - Silver -->
  <g transform="translate(190, 40)" opacity="0">
    <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1s" fill="freeze"/>
    <rect x="0" y="0" width="120" height="130" rx="10" fill="#0d2137" stroke="#c0c0c0" stroke-width="1"/>
    <text x="60" y="40" text-anchor="middle" font-size="30">🥈</text>
    <text x="60" y="70" text-anchor="middle" font-family="'Courier New', monospace" font-size="12" fill="#c0c0c0" font-weight="bold">Silver</text>
    <text x="60" y="90" text-anchor="middle" font-family="'Courier New', monospace" font-size="10" fill="#80b0c8">Quick Learner</text>
    <text x="60" y="115" text-anchor="middle" font-family="'Courier New', monospace" font-size="9" fill="#c0c0c0">#2</text>
  </g>
  
  <!-- Trophy 3 - Bronze -->
  <g transform="translate(330, 40)" opacity="0">
    <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1.5s" fill="freeze"/>
    <rect x="0" y="0" width="120" height="130" rx="10" fill="#0d2137" stroke="#cd7f32" stroke-width="1"/>
    <text x="60" y="40" text-anchor="middle" font-size="30">🥉</text>
    <text x="60" y="70" text-anchor="middle" font-family="'Courier New', monospace" font-size="12" fill="#cd7f32" font-weight="bold">Bronze</text>
    <text x="60" y="90" text-anchor="middle" font-family="'Courier New', monospace" font-size="10" fill="#80b0c8">Rising Star</text>
    <text x="60" y="115" text-anchor="middle" font-family="'Courier New', monospace" font-size="9" fill="#cd7f32">#3</text>
  </g>
</svg>

name: Generate Snake Animation

on:
  schedule:
    - cron: "0 0 * * *"  # Runs daily at midnight
  workflow_dispatch:  # Allows manual trigger

jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10
    
    steps:
      - name: Checkout repository
        uses: actions/checkout@v3
      
      - name: Generate snake.svg
        uses: Platane/snk@v3
        with:
          github_user_name: Dishi-glitch
          outputs: |
            dist/snake.svg?palette=github-dark&color_snake=#00b4d8&color_dots=#0a1929,#0d2137,#0077b6,#00b4d8,#023e8a
            dist/snake-light.svg?palette=github-light&color_snake=#0077b6&color_dots=#ffffff,#e0f0ff,#00b4d8,#0077b6,#023e8a
          
      - name: Push to output branch
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./dist
          publish_branch: output
          destination_dir: .
          keep_files: false

<br>
<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="banner.svg?v=1">
  <source media="(prefers-color-scheme: light)" srcset="banner-light.svg?v=1">
  &lt;img src="banner.svg?v=1" alt="Dishi Neekhra Banner" width="100%"&gt;
</picture>

<br><br>

<!-- Lanyard Badge -->
&lt;img src="lanyard.svg?v=1" alt="ID Badge" width="200"&gt;

<br><br>

<!-- Stats Cards -->
<table>
  <tr>
    <td>
      &lt;img src="stats.svg?v=1" alt="GitHub Stats" width="400"&gt;
    </td>
    <td>
      &lt;img src="langs.svg?v=1" alt="Top Languages" width="400"&gt;
    </td>
  </tr>
</table>

<br>

<!-- Trophies -->
&lt;img src="trophies.svg?v=1" alt="Trophies" width="500"&gt;

<br><br>

## 📊 Contribution Graph

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Dishi-glitch/Dishi-glitch/output/snake.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Dishi-glitch/Dishi-glitch/output/snake-light.svg">
  &lt;img src="https://raw.githubusercontent.com/Dishi-glitch/Dishi-glitch/output/snake.svg" alt="Snake Animation" width="100%"&gt;
</picture>

<br><br>

## 🚀 Featured Projects

| Project | Description | Tech Stack |
|---------|-------------|------------|
| [Project 1](https://github.com/Dishi-glitch/project1) | A cool full-stack web app | React, Node.js, MongoDB |
| [Project 2](https://github.com/Dishi-glitch/project2) | AI-powered tool | Python, TensorFlow, Flask |
| [Project 3](https://github.com/Dishi-glitch/project3) | Frontend UI library | React, Tailwind CSS, Framer Motion |

<br>

## 📫 Connect With Me

<a href="mailto:dishineekhra23@gmail.com">
  &lt;img src="https://img.shields.io/badge/Email-dishineekhra23%40gmail.com-00b4d8?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"&gt;
</a>
<a href="https://github.com/Dishi-glitch">
  &lt;img src="https://img.shields.io/badge/GitHub-@Dishi--glitch-0077b6?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"&gt;
</a>
<a href="https://linkedin.com/in/dishi-neekhra">
  &lt;img src="https://img.shields.io/badge/LinkedIn-Dishi%20Neekhra-023e8a?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"&gt;
</a>

<br><br>

<!-- Profile Views Counter -->
&lt;img src="https://komarev.com/ghpvc/?username=Dishi-glitch&color=00b4d8&style=flat-square" alt="Profile Views"&gt;

<br>

---

⭐️ From [Dishi-glitch](https://github.com/Dishi-glitch)

</div>
