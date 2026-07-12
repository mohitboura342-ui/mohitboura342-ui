<svg xmlns="http://www.w3.org/2000/svg" width="1180" height="610" viewBox="0 0 1180 610" fill="none">
  <defs>
    <linearGradient id="bgGrad" x1="0" y1="0" x2="1180" y2="610" gradientUnits="userSpaceOnUse">
      <stop offset="0%" stop-color="#030712"/>
      <stop offset="100%" stop-color="#0B1020"/>
    </linearGradient>

    <radialGradient id="glow1" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse" gradientTransform="translate(190 130) rotate(45) scale(260 220)">
      <stop offset="0%" stop-color="#7C3AED" stop-opacity=".32"/>
      <stop offset="100%" stop-color="#7C3AED" stop-opacity="0"/>
    </radialGradient>

    <radialGradient id="glow2" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse" gradientTransform="translate(930 110) rotate(120) scale(300 260)">
      <stop offset="0%" stop-color="#22D3EE" stop-opacity=".24"/>
      <stop offset="100%" stop-color="#22D3EE" stop-opacity="0"/>
    </radialGradient>

    <radialGradient id="glow3" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse" gradientTransform="translate(930 500) rotate(30) scale(340 220)">
      <stop offset="0%" stop-color="#10B981" stop-opacity=".15"/>
      <stop offset="100%" stop-color="#10B981" stop-opacity="0"/>
    </radialGradient>

    <linearGradient id="panelGrad" x1="0" y1="0" x2="0" y2="610">
      <stop offset="0%" stop-color="#0F172A" stop-opacity=".92"/>
      <stop offset="100%" stop-color="#0B1220" stop-opacity=".82"/>
    </linearGradient>

    <linearGradient id="borderGrad" x1="0" y1="0" x2="1180" y2="0">
      <stop offset="0%" stop-color="#7C3AED"/>
      <stop offset="45%" stop-color="#22D3EE"/>
      <stop offset="100%" stop-color="#10B981"/>
      <animate attributeName="x1" values="0;1180;0" dur="8s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="1180;2360;1180" dur="8s" repeatCount="indefinite"/>
    </linearGradient>

    <linearGradient id="asciiGrad" x1="0" y1="0" x2="380" y2="0">
      <stop offset="0%" stop-color="#22D3EE"/>
      <stop offset="50%" stop-color="#A78BFA"/>
      <stop offset="100%" stop-color="#10B981"/>
      <animate attributeName="x1" values="0;380;0" dur="10s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="380;760;380" dur="10s" repeatCount="indefinite"/>
    </linearGradient>

    <linearGradient id="pillGrad" x1="0" y1="0" x2="200" y2="0">
      <stop offset="0%" stop-color="#0EA5E9" stop-opacity=".22"/>
      <stop offset="50%" stop-color="#A855F7" stop-opacity=".18"/>
      <stop offset="100%" stop-color="#10B981" stop-opacity=".18"/>
      <animate attributeName="x1" values="0;200;0" dur="7s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="200;400;200" dur="7s" repeatCount="indefinite"/>
    </linearGradient>

    <filter id="blur24" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur stdDeviation="24"/>
    </filter>

    <filter id="blur10" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur stdDeviation="10"/>
    </filter>

    <filter id="glow">
      <feGaussianBlur stdDeviation="3.2" result="b"/>
      <feColorMatrix in="b" type="matrix" values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 18 -7"/>
    </filter>

    <clipPath id="leftClip">
      <rect x="0" y="0" width="448" height="610" rx="30"/>
    </clipPath>

    <clipPath id="rightClip">
      <rect x="452" y="0" width="728" height="610" rx="30"/>
    </clipPath>

    <mask id="scanMask">
      <rect width="1180" height="610" fill="white"/>
      <rect y="-110" width="1180" height="110" fill="black">
        <animateTransform attributeName="transform" type="translate" values="0 0;0 820" dur="4.8s" repeatCount="indefinite"/>
      </rect>
    </mask>

    <mask id="reveal1">
      <rect x="0" y="0" width="180" height="0" fill="white">
        <animate attributeName="height" values="0;92;92" dur="2.8s" repeatCount="indefinite"/>
      </rect>
    </mask>

    <mask id="reveal2">
      <rect x="0" y="0" width="360" height="0" fill="white">
        <animate attributeName="height" values="0;82;82" dur="3.2s" begin="0.4s" repeatCount="indefinite"/>
      </rect>
    </mask>

    <style>
      .title { font: 700 44px Inter, Segoe UI, Arial, sans-serif; fill: #F8FAFC; }
      .sub { font: 500 19px Inter, Segoe UI, Arial, sans-serif; fill: #94A3B8; }
      .label { font: 600 14px Inter, Segoe UI, Arial, sans-serif; fill: #94A3B8; letter-spacing: .08em; }
      .text { font: 500 16px Inter, Segoe UI, Arial, sans-serif; fill: #E2E8F0; }
      .small { font: 500 13px Inter, Segoe UI, Arial, sans-serif; fill: #CBD5E1; }
      .pill { font: 600 13px Inter, Segoe UI, Arial, sans-serif; fill: #E2E8F0; }
      .mono { font: 500 12px "SFMono-Regular", Consolas, monospace; fill: #93C5FD; }
    </style>
  </defs>

  <rect width="1180" height="610" rx="30" fill="url(#bgGrad)"/>
  <rect width="1180" height="610" rx="30" fill="url(#glow1)" filter="url(#blur24)"/>
  <rect width="1180" height="610" rx="30" fill="url(#glow2)" filter="url(#blur24)"/>
  <rect width="1180" height="610" rx="30" fill="url(#glow3)" filter="url(#blur24)"/>

  <g opacity=".35" mask="url(#scanMask)">
    <rect width="1180" height="610" fill="none"/>
    <path d="M0 0H1180" stroke="#FFFFFF" stroke-opacity=".08"/>
    <path d="M0 72H1180" stroke="#FFFFFF" stroke-opacity=".03"/>
    <path d="M0 144H1180" stroke="#FFFFFF" stroke-opacity=".03"/>
    <path d="M0 216H1180" stroke="#FFFFFF" stroke-opacity=".03"/>
    <path d="M0 288H1180" stroke="#FFFFFF" stroke-opacity=".03"/>
    <path d="M0 360H1180" stroke="#FFFFFF" stroke-opacity=".03"/>
    <path d="M0 432H1180" stroke="#FFFFFF" stroke-opacity=".03"/>
    <path d="M0 504H1180" stroke="#FFFFFF" stroke-opacity=".03"/>
  </g>

  <g opacity=".35">
    <circle cx="118" cy="96" r="2.2" fill="#22D3EE">
      <animate attributeName="cy" values="96;74;96" dur="4s" repeatCount="indefinite"/>
    </circle>
    <circle cx="370" cy="172" r="1.8" fill="#A78BFA">
      <animate attributeName="cy" values="172;150;172" dur="5.2s" repeatCount="indefinite"/>
    </circle>
    <circle cx="1032" cy="122" r="2.2" fill="#10B981">
      <animate attributeName="cy" values="122;140;122" dur="4.4s" repeatCount="indefinite"/>
    </circle>
    <circle cx="1070" cy="478" r="1.8" fill="#22D3EE">
      <animate attributeName="cy" values="478;454;478" dur="6s" repeatCount="indefinite"/>
    </circle>
  </g>

  <g clip-path="url(#leftClip)" transform="translate(18 18)">
    <rect x="0" y="0" width="422" height="574" rx="24" fill="url(#panelGrad)" stroke="url(#borderGrad)" stroke-opacity=".45"/>
    <rect x="0" y="0" width="422" height="574" rx="24" fill="#FFFFFF" opacity=".02"/>
    <g opacity=".55" filter="url(#blur10)">
      <rect x="18" y="20" width="130" height="2" rx="1" fill="#22D3EE"/>
      <rect x="270" y="40" width="110" height="2" rx="1" fill="#A855F7"/>
    </g>
    <g transform="translate(28 42)">
      <text class="mono" x="0" y="0">╭──────────────────────────────╮</text>
      <text class="mono" x="0" y="18">│  &gt; scanning portrait...      │</text>
      <text class="mono" x="0" y="36">│  &gt; id: mohit-boura          │</text>
      <text class="mono" x="0" y="54">│  &gt; status: online           │</text>
    </g>

    <g opacity=".95" transform="translate(46 132) scale(1.02)">
      <g filter="url(#glow)">
        <text x="0" y="0" class="mono" fill="url(#asciiGrad)">⣿⣿⣿⡿⠿⠿⠿⠿⠿⢿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿</text>
        <text x="0" y="18" class="mono" fill="url(#asciiGrad)">⣿⠋⠀⠀⠀⠀⢀⣤⣶⣦⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⣿</text>
        <text x="0" y="36" class="mono" fill="url(#asciiGrad)">⣿⠀⠀⠀⠀⣰⣿⣿⣿⣿⣿⣿⣦⠀⠀⠀⠀⠀⠀⠀⠀⣿</text>
        <text x="0" y="54" class="mono" fill="url(#asciiGrad)">⣿⠀⠀⠀⢸⣿⣿⣿⣿⣿⣿⣿⣿⣿⡇⠀⠀⠀⠀⠀⠀⣿</text>
        <text x="0" y="72" class="mono" fill="url(#asciiGrad)">⣿⠀⠀⠀⢸⣿⡏⠀⠀⠉⠉⠀⠀⢹⣿⡇⠀⠀⠀⠀⠀⣿</text>
        <text x="0" y="90" class="mono" fill="url(#asciiGrad)">⣿⠀⠀⠀⠸⣿⣧⣀⣀⣀⣀⣀⣴⣿⠇⠀⠀⠀⠀⠀⣿</text>
        <text x="0" y="108" class="mono" fill="url(#asciiGrad)">⣿⠀⠀⠀⠀⠈⠻⣿⣿⣿⣿⣿⠟⠁⠀⠀⠀⠀⠀⠀⣿</text>
        <text x="0" y="126" class="mono" fill="url(#asciiGrad)">⣿⠀⠀⠀⠀⠀⠀⠀⠈⠉⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿</text>
        <text x="0" y="144" class="mono" fill="url(#asciiGrad)">⣿⣿⣿⡄⠀⠀⢀⣀⣀⣀⣀⣀⡀⠀⠀⢠⣿⣿⣿⣿⣿⣿</text>
        <text x="0" y="162" class="mono" fill="url(#asciiGrad)">⣿⣿⣿⣿⡀⠀⠈⠉⠉⠉⠉⠉⠁⠀⢀⣿⣿⣿⣿⣿⣿⣿</text>
      </g>
      <animateTransform attributeName="transform" type="translate" values="0 0;0 -4;0 0" dur="5s" repeatCount="indefinite"/>
      <g opacity=".95">
        <rect x="342" y="156" width="2.5" height="18" fill="#A78BFA">
          <animate attributeName="opacity" values="0;1;0" dur="1s" repeatCount="indefinite"/>
        </rect>
      </g>
    </g>

    <rect x="18" y="500" width="386" height="52" rx="16" fill="#0B1220" fill-opacity=".55" stroke="url(#borderGrad)" stroke-opacity=".18"/>
    <text x="34" y="530" class="small">Generated for Mohit Boura • premium profile header</text>
  </g>

  <g clip-path="url(#rightClip)" transform="translate(462 18)">
    <rect x="0" y="0" width="700" height="574" rx="24" fill="url(#panelGrad)" stroke="url(#borderGrad)" stroke-opacity=".45"/>
    <rect x="0" y="0" width="700" height="574" rx="24" fill="#FFFFFF" opacity=".02"/>
    <rect x="24" y="18" width="652" height="28" rx="14" fill="#FFFFFF" opacity=".04"/>
    <circle cx="44" cy="32" r="5" fill="#EF4444" opacity=".8"/>
    <circle cx="62" cy="32" r="5" fill="#F59E0B" opacity=".8"/>
    <circle cx="80" cy="32" r="5" fill="#22C55E" opacity=".8"/>

    <text x="34" y="92" class="sub">Hi 👋</text>
    <text x="34" y="142" class="title">I'm Mohit Boura</text>

    <text x="34" y="180" class="text">
      <tspan>Data Analyst</tspan>
      <animate attributeName="opacity" values="0;1;1;0" dur="9s" repeatCount="indefinite"/>
    </text>
    <text x="34" y="180" class="text" opacity="0">
      <animate attributeName="opacity" values="0;1;1;0" dur="9s" begin="1.5s" repeatCount="indefinite"/>
      <tspan>AI Developer</tspan>
    </text>
    <text x="34" y="180" class="text" opacity="0">
      <animate attributeName="opacity" values="0;1;1;0" dur="9s" begin="3s" repeatCount="indefinite"/>
      <tspan>Full Stack Developer</tspan>
    </text>
    <text x="34" y="180" class="text" opacity="0">
      <animate attributeName="opacity" values="0;1;1;0" dur="9s" begin="4.5s" repeatCount="indefinite"/>
      <tspan>Machine Learning Engineer</tspan>
    </text>
    <text x="34" y="180" class="text" opacity="0">
      <animate attributeName="opacity" values="0;1;1;0" dur="9s" begin="6s" repeatCount="indefinite"/>
      <tspan>Computer Vision Enthusiast</tspan>
    </text>
    <text x="34" y="180" class="text" opacity="0">
      <animate attributeName="opacity" values="0;1;1;0" dur="9s" begin="7.5s" repeatCount="indefinite"/>
      <tspan>Open Source Contributor</tspan>
    </text>

    <rect x="34" y="193" width="9" height="22" rx="3" fill="#22D3EE">
      <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/>
    </rect>

    <g transform="translate(34 246)">
      <text class="label" x="0" y="0">LOCATION</text>
      <text class="text" x="0" y="28">📍 Uttarakhand, India</text>

      <text class="label" x="0" y="70">EDUCATION</text>
      <text class="text" x="0" y="98">🎓 B.Com (Analytics &amp; Technology)</text>
      <text class="small" x="0" y="120">Uttarakhand Open University</text>

      <text class="label" x="0" y="156">CURRENT FOCUS</text>
      <text class="text" x="0" y="184">Building AI Applications • Machine Learning</text>
      <text class="text" x="0" y="208">Computer Vision • Data Analytics • Generative AI</text>
      <text class="text" x="0" y="232">Open Source</text>

      <text class="label" x="0" y="268">PORTFOLIO</text>
      <text class="small" x="0" y="294">github.com/mohitboura342-ui</text>

      <text class="label" x="0" y="330">EMAIL</text>
      <text class="small" x="0" y="356">your-email@example.com</text>
    </g>

    <g transform="translate(34 444)">
      <text class="label" x="0" y="0">SKILLS</text>

      <g transform="translate(0 18)">
        <g><rect x="0" y="0" rx="14" ry="14" width="86" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">Python</text></g>
        <g transform="translate(94 0)"><rect x="0" y="0" rx="14" ry="14" width="76" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">Pandas</text></g>
        <g transform="translate(178 0)"><rect x="0" y="0" rx="14" ry="14" width="72" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">NumPy</text></g>
        <g transform="translate(258 0)"><rect x="0" y="0" rx="14" ry="14" width="108" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">Scikit-Learn</text></g>
        <g transform="translate(374 0)"><rect x="0" y="0" rx="14" ry="14" width="92" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">TensorFlow</text></g>
        <g transform="translate(474 0)"><rect x="0" y="0" rx="14" ry="14" width="76" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">OpenCV</text></g>
        <g transform="translate(558 0)"><rect x="0" y="0" rx="14" ry="14" width="52" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">SQL</text></g>
      </g>

      <g transform="translate(0 56)">
        <g><rect x="0" y="0" rx="14" ry="14" width="78" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">Power BI</text></g>
        <g transform="translate(86 0)"><rect x="0" y="0" rx="14" ry="14" width="84" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">Streamlit</text></g>
        <g transform="translate(178 0)"><rect x="0" y="0" rx="14" ry="14" width="54" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">Flask</text></g>
        <g transform="translate(240 0)"><rect x="0" y="0" rx="14" ry="14" width="68" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">React</text></g>
        <g transform="translate(316 0)"><rect x="0" y="0" rx="14" ry="14" width="74" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">Next.js</text></g>
        <g transform="translate(398 0)"><rect x="0" y="0" rx="14" ry="14" width="76" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">Node.js</text></g>
        <g transform="translate(482 0)"><rect x="0" y="0" rx="14" ry="14" width="74" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">TypeScript</text></g>
        <g transform="translate(564 0)"><rect x="0" y="0" rx="14" ry="14" width="90" height="30" fill="url(#pillGrad)" stroke="#FFFFFF" stroke-opacity=".08"/><text x="14" y="20" class="pill">Tailwind</text></g>
      </g>
    </g>

    <g transform="translate(34 556)">
      <circle cx="0" cy="0" r="9" fill="#7C3AED" opacity=".22"/>
      <circle cx="0" cy="0" r="5" fill="#7C3AED"/>
      <text x="18" y="5" class="small">GitHub</text>

      <circle cx="110" cy="0" r="9" fill="#22D3EE" opacity=".22"/>
      <circle cx="110" cy="0" r="5" fill="#22D3EE"/>
      <text x="128" y="5" class="small">LinkedIn</text>

      <circle cx="236" cy="0" r="9" fill="#10B981" opacity=".22"/>
      <circle cx="236" cy="0" r="5" fill="#10B981"/>
      <text x="254" y="5" class="small">Portfolio</text>

      <circle cx="360" cy="0" r="9" fill="#A855F7" opacity=".22"/>
      <circle cx="360" cy="0" r="5" fill="#A855F7"/>
      <text x="378" y="5" class="small">Twitter / X</text>
    </g>
  </g>

  <rect x="1" y="1" width="1178" height="608" rx="29" fill="none" stroke="#FFFFFF" stroke-opacity=".06"/>
</svg>
