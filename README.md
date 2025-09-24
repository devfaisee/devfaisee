<!-- README.md — Faisee (Hacker-Philosopher Art Edition) -->

<!-- ========== Animated Neon Glitch Header (inline SVG) ========== -->
<p align="center">
  <!-- Inline SVG Banner: neon gradient + subtle glitch + scanline -->
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1100 220" width="100%" preserveAspectRatio="xMidYMid meet" role="img" aria-label="Faisee — Code Artist">
    <defs>
      <linearGradient id="g1" x1="0" x2="1">
        <stop offset="0" stop-color="#00f0ff"/>
        <stop offset="0.5" stop-color="#9b00ff"/>
        <stop offset="1" stop-color="#ff0066"/>
      </linearGradient>

      <filter id="glitch" x="-20%" y="-20%" width="140%" height="140%">
        <!-- multiple displaced color channels for glitch -->
        <feColorMatrix in="SourceGraphic" result="orig" type="matrix"
          values="1 0 0 0 0
                  0 1 0 0 0
                  0 0 1 0 0
                  0 0 0 1 0"/>
        <feOffset in="orig" dx="-6" dy="0" result="r1"/>
        <feGaussianBlur in="r1" stdDeviation="0.6" result="b1"/>
        <feComposite in="b1" in2="orig" operator="in" result="c1"/>
        <feBlend in="orig" in2="c1" mode="screen" />
      </filter>

      <pattern id="scan" patternUnits="userSpaceOnUse" width="8" height="8">
        <rect width="8" height="4" y="0" fill="rgba(0,0,0,0.07)"></rect>
      </pattern>

      <mask id="fade">
        <linearGradient id="maskgrad" x1="0" x2="0" y1="0" y2="1">
          <stop offset="0" stop-color="#fff" stop-opacity="1"/>
          <stop offset="1" stop-color="#fff" stop-opacity="0.85"/>
        </linearGradient>
        <rect x="0" y="0" width="100%" height="100%" fill="url(#maskgrad)"/>
      </mask>
    </defs>

    <!-- background gradient -->
    <rect width="100%" height="100%" fill="#060812"/>

    <!-- subtle noise / scanlines -->
    <rect width="100%" height="100%" fill="url(#scan)" opacity="0.35" />

    <!-- main text (three layered copies for neon + chromatic glitch) -->
    <g transform="translate(40, 120)">
      <!-- shadow / glow copies for chroma split -->
      <text id="t-shadow" x="0" y="0" font-family="Fira Code,monospace" font-size="72" font-weight="700" letter-spacing="2" fill="none" stroke="#FF007A" stroke-width="2" transform="translate(6,4)" opacity="0.7">Faisee ⚡ Code Artist</text>

      <g filter="url(#glitch)">
        <text x="0" y="0" font-family="Fira Code,monospace" font-size="72" font-weight="800" letter-spacing="2" fill="url(#g1)" >
          Faisee ⚡ Code Artist
          <animate attributeName="x" values="0;2;0;-1;0" dur="3s" repeatCount="indefinite" />
        </text>
      </g>

      <!-- neon outline -->
      <text x="0" y="0" font-family="Fira Code,monospace" font-size="72" font-weight="800" letter-spacing="2" fill="none" stroke="rgba(255,255,255,0.06)" stroke-width="1">
        Faisee ⚡ Code Artist
      </text>
    </g>

    <!-- subtle scanline sweep -->
    <rect width="1100" height="220" fill="rgba(255,255,255,0.02)" mask="url(#fade)">
      <animate attributeName="x" from="-1100" to="1100" dur="7s" repeatCount="indefinite"/>
    </rect>

    <!-- tiny tagline -->
    <g transform="translate(40, 170)" fill="#9CA3AF" font-family="ui-monospace, SFMono-Regular, Menlo, Monaco, " font-size="14">
      <text x="0" y="0">Code is my canvas · Logic is my paint · I ship with intent</text>
    </g>
  </svg>
</p>

<!-- ========== Small Animated Monogram Logo ========== -->
<p align="center">
  <!-- Monogram SVG (F) as mark — animated stroke -->
  <svg xmlns="http://www.w3.org/2000/svg" width="110" height="110" viewBox="0 0 110 110" aria-label="Faisee monogram">
    <defs>
      <linearGradient id="lg2" x1="0" x2="1">
        <stop offset="0" stop-color="#00F0FF" />
        <stop offset="1" stop-color="#FF0066" />
      </linearGradient>
    </defs>
    <circle cx="55" cy="55" r="52" fill="#071024"/>
    <path d="M36 32 L74 32 L50 54 L74 78 L36 78" fill="none" stroke="url(#lg2)" stroke-width="6" stroke-linecap="round" stroke-linejoin="round" stroke-opacity="0.95">
      <animate attributeName="stroke-dasharray" from="0 300" to="240 300" dur="1.6s" fill="freeze" />
    </path>
  </svg>
</p>

---

<p align="center"><em style="color:#9CA3AF">Manifesto — hacker-philosopher: I prefer fewer features done excellently over many half-finished attempts. Beauty and utility must co-exist.</em></p>

---

## 🔮 What I build (short & sharp)
- **Small, surgical tools** that shave developer friction.  
- **Minimal front-ends** with crisp UX & accessibility.  
- **Open-source starters** that people can clone and ship in < 30 minutes.

---

## 🧭 Stack (my creative palette)
<p align="center">
  <img src="https://skillicons.dev/icons?i=js,ts,react,nextjs,tailwind,nodejs,python,html,css,git,github,figma" alt="skills" />
</p>

---

## 🚀 Spotlight — featured repos (one-liners)
- **portfolio-by-faisee** — Minimal Next.js portfolio starter: fast, accessible, brandable.  
- **weatharia** — Small weather microapp showcasing clean UI and caching patterns.  
- **portfolio-tailwind** — Pixel-first Tailwind scaffolding with thoughtful defaults.

*(Open any repo and drop an issue — I read them.)*

---

## 🧩 Projects — gallery (visual + value)
<p align="center">
  <a href="https://github.com/devfaisee/portfolio-by-faisee" style="text-decoration:none">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=devfaisee&repo=portfolio-by-faisee&theme=dark&hide_border=true" alt="portfolio-by-faisee" />
  </a>
  <a href="https://github.com/devfaisee/weatharia" style="text-decoration:none">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=devfaisee&repo=weatharia&theme=dark&hide_border=true" alt="weatharia" />
  </a>
  <a href="https://github.com/devfaisee/portfolio-tailwind" style="text-decoration:none">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=devfaisee&repo=portfolio-tailwind&theme=dark&hide_border=true" alt="portfolio-tailwind" />
  </a>
</p>

---

## 🧠 Quick pitch — why hire/collab me
- I ship pragmatic solutions fast.  
- I balance **design** with **engineering**.  
- I fix things that block people, not just features that look cool.

---

## ✉️ Contact
- Email: `hi@devfaisee.dev`  
- Twitter: [@devfaisee](https://twitter.com/devfaisee)  
- Or open an issue on any repo — I actually respond.

---

<!-- Footer Wave (SVG) -->
<p align="center">
  <svg viewBox="0 0 1200 80" width="100%" height="60" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
    <defs>
      <linearGradient id="fg1" x1="0" x2="1">
        <stop offset="0" stop-color="#00F0FF" />
        <stop offset="1" stop-color="#FF0080" />
      </linearGradient>
    </defs>
    <path d="M0,30 C300,120 900,-40 1200,30 L1200,80 L0,80 Z" fill="url(#fg1)">
      <animate attributeName="d" dur="8s" repeatCount="indefinite"
        values="
          M0,30 C300,120 900,-40 1200,30 L1200,80 L0,80 Z;
          M0,30 C300,-40 900,120 1200,30 L1200,80 L0,80 Z;
          M0,30 C300,100 900,-20 1200,30 L1200,80 L0,80 Z;
          M0,30 C300,120 900,-40 1200,30 L1200,80 L0,80 Z
        " />
    </path>
  </svg>
</p>

---

### ✨ Pro tips to make this 1,000x nicer
1. Put the SVGs in `assets/` and reference them as files (faster and cleaner): `/assets/banner.svg` & `/assets/mark.svg`.  
2. Add a tiny `meta` README in each featured repo with a one-sentence mission and "how to run" so visitors instantly grok it.  
3. Keep your repo README template consistent so every project reads like part of your brand.

---

### 🗂 Optional: Save SVGs as separate files (recommended)
- Create folder: `/assets/`  
- Save the banner SVG content (from the banner block above) to `assets/banner.svg`.  
- Save the monogram SVG content to `assets/mark.svg`.  
- Replace the inline blocks with:
  ```html
  <p align="center">
    <img src="./assets/banner.svg" width="100%" alt="Faisee — Code Artist" />
  </p>
  <p align="center">
    <img src="./assets/mark.svg" width="110" alt="Faisee mark" />
  </p>