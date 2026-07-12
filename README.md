<svg xmlns="http://www.w3.org/2000/svg" width="1180" height="610" viewBox="0 0 1180 610" fill="none">
  <!-- Dark Mode SVG -->
  <defs>
    <!-- Main Glass Panel -->
    <filter id=" glass" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="12" result="blur"/>
      <feColorMatrix type="matrix" values="1 0 0 0 0.03 0 1 0 0 0 0 0 1 0 0 0 0 0 0.75 0"/>
    </filter>

    <!-- Border Shimmer -->
    <filter id="shimmer" x="-50%" y="-50%" width="200%" height="200%">
      <feTurbulence type=" 2" baseFrequency="0.05" numOctaves="3" result="turb"/>
      <feDisplacementMap in="SourceGraphic" in2="turb" scale="3" xChannelSelector="R" yChannelSelector="G"/>
    </filter>

    <!-- ASCII Gradient -->
    <linear gradient id="asciiGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#22D3EE"/>
      <stop offset="50%" stop-color="#7C3AED"/>
      <stop offset="100%" stop-color="#10B981"/>
    </linearGradient>

    <!-- Accent Gradient -->
    <linearGradient id="accent" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#7C3AED"/>
      <stop offset="50%" stop-color="#22D3EE"/>
      <stop offset="100%" stop-color="#10B981"/>
    </linearGradient>

    <!-- Glow Filter -->
    <filter id="glow" x="-40%" y="-40%" width="180%" height="180%">
      <feGaussianBlur stdDeviation="8" result="glow"/>
      <feMerge>
        <feMergeNode in="glow"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Scanline -->
    <filter id="scan" x="0" y="0" width=" 100%" height="100%">
      <feTurbulence type="fractalNoise" baseFrequency="0.02" numOctaves="3" result="noise"/>
      <feColorMatrix type="matrix" values="1 0 0 0 0 0 1 0 0  0 0 0 1 0 0 0 0 0 0.15 0"/>
    </filter>

    <!-- Particles -->
    <radialGradient id="particle" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#22 D3EE" stop-opacity="0.6"/>
      <stop offset="100%" stop-color="#22D3EE" stop-opacity="0"/>
    </radialGradient>

    <!-- Rounded Corners -->
    <clipPath id="panel">
      <rect rx="16" ry="16"/>
    </clipPath >
  </defs>

  <!-- Background -->
  <rect width="1180" height="610" fill="#030712" rx="24"/>

  <!-- Floating Radial Glows -->
  <circle cx="180" cy="120" r="220" fill="url(#particle)">
    <animate attributeName=" cx" values="180;220;180" dur="14s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="120;160;120" dur="16s" repeatCount="indefinite"/>
  </circle>
  <circle cx="920" cy="480 " r="180" fill="url(#particle)">
    <animate attributeName="cx" values="920;880;920" dur="18s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="480;520;480" dur="15s" repeatCount="ind ef inite"/>
  </circle>

  <!-- Noise Texture -->
  <rect width="1180" height="610" filter="url(#scan)" opacity="0.35"/>

  <!-- Main Glass Container -->
  <rect x="24" y="24" width="1132" height="562" rx ="24" fill="#0F172A" fill-opacity="0.75" filter="url(#glass)" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>

  <!-- Border Shimmer -->
  <rect x="24" y="24" width="1132" height="562" rx="24" fill="none" stroke="url(#accent)" stroke-width="1.5">
    <animate attributeName="stroke-dashoffset" values="0; 300" dur="3s" repeatCount="indefinite"/>
  </rect>

  <!-- LEFT PANEL - 38% -->
  <rect x="48" y="48" width="428" height="514" rx="16" fill="#0F172A" fill-opacity="0.85" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>

  <!-- Left Panel Reflection -->
  <path d="M48 60 Q 140 40 220 60 L 220 110 Q 140 85 48 110 Z" fill="white" opacity="0.04"/>

  <!-- ASCII Portrait Container -->
  <g transform="translate(70, 70)">
    <!-- Reveal Clip -->
    <clipPath id="asciiClip">
      <rect x="0" y="0" width="380" height="0">
        <animate attributeName="height" from="0" to="380" dur="4.2s" fill="freeze"/>
      </rect>
    </clipPath>

    <!-- ASCII Art (revealed line-by-line) -->
    <g clip-path="url(#asciiClip)">
      <text font-family="ui-monospace, SFMono-Regular, Menlo, monospace" font-size="8.
