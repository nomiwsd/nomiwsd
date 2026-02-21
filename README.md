<div align="center">

<!-- ═══════════════════════════════════════════════════════════
     ANIMATED HERO BANNER
════════════════════════════════════════════════════════════ -->

<svg width="900" height="280" viewBox="0 0 900 280" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes fadeUp {
        from { opacity:0; transform:translateY(18px); }
        to   { opacity:1; transform:translateY(0);    }
      }
      @keyframes scanMove {
        from { transform:translateY(-60px); }
        to   { transform:translateY(340px); }
      }
      @keyframes lineGrow {
        from { stroke-dashoffset:300; opacity:0; }
        to   { stroke-dashoffset:0;   opacity:1; }
      }
      @keyframes blink {
        0%,100%{ opacity:1; } 50%{ opacity:0; }
      }
      @keyframes dotPop {
        0%  { opacity:0; }
        60% { opacity:0.7; }
        100%{ opacity:0.25; }
      }
      @keyframes glowPulse {
        0%,100%{ filter:drop-shadow(0 0 8px rgba(255,69,0,0.35)); }
        50%    { filter:drop-shadow(0 0 22px rgba(255,69,0,0.75)); }
      }
      .nm-main  { font-family:Impact,'Arial Black',sans-serif; font-size:110px; font-weight:900; fill:#F5ECD7;
                  animation:fadeUp 0.7s ease 0.1s both, glowPulse 3s ease-in-out 0.8s infinite; }
      .nm-red   { font-family:Impact,'Arial Black',sans-serif; font-size:110px; font-weight:900;
                  fill:rgba(255,30,0,0.2); animation:fadeUp 0.7s ease 0.1s both; }
      .nm-blue  { font-family:Impact,'Arial Black',sans-serif; font-size:110px; font-weight:900;
                  fill:rgba(0,90,255,0.16); animation:fadeUp 0.7s ease 0.1s both; }
      .label-top{ font-family:'Courier New',monospace; font-size:10.5px; fill:#FF4500; letter-spacing:6px;
                  animation:fadeUp 0.6s ease 0.55s both; }
      .label-sub{ font-family:'Courier New',monospace; font-size:12px; fill:#F5ECD7; letter-spacing:2px; opacity:0.82;
                  animation:fadeUp 0.6s ease 0.8s both; }
      .cursor   { animation:blink 0.75s step-end infinite; }
      .line-t   { stroke-dasharray:300; stroke-dashoffset:300; animation:lineGrow 0.55s ease 0.48s both; }
      .line-b   { stroke-dasharray:300; stroke-dashoffset:300; animation:lineGrow 0.55s ease 0.95s both; }
      .scan     { animation:scanMove 3.8s linear 1s infinite; }
      .d1{animation:dotPop 0.5s ease 0.35s both;}
      .d2{animation:dotPop 0.5s ease 0.55s both;}
      .d3{animation:dotPop 0.5s ease 0.45s both;}
      .d4{animation:dotPop 0.5s ease 0.65s both;}
      .d5{animation:dotPop 0.5s ease 0.40s both;}
      .d6{animation:dotPop 0.5s ease 0.60s both;}
      .d7{animation:dotPop 0.5s ease 0.50s both;}
      .d8{animation:dotPop 0.5s ease 0.70s both;}
      .chips{animation:fadeUp 0.5s ease 1.15s both;}
    </style>
    <pattern id="sl" x="0" y="0" width="2" height="4" patternUnits="userSpaceOnUse">
      <rect width="2" height="2" fill="rgba(0,0,0,0.22)"/>
    </pattern>
    <linearGradient id="lg" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%"   stop-color="transparent"/>
      <stop offset="50%"  stop-color="#FF4500"/>
      <stop offset="100%" stop-color="transparent"/>
    </linearGradient>
  </defs>

  <!-- BG -->
  <rect width="900" height="280" fill="#080808"/>

  <!-- Corner brackets -->
  <path d="M20,20 L20,42 M20,20 L42,20" stroke="#FF4500" stroke-width="1.5" fill="none" opacity="0.55"/>
  <path d="M880,20 L880,42 M880,20 L858,20" stroke="#FF4500" stroke-width="1.5" fill="none" opacity="0.55"/>
  <path d="M20,260 L20,238 M20,260 L42,260" stroke="#FF4500" stroke-width="1.5" fill="none" opacity="0.55"/>
  <path d="M880,260 L880,238 M880,260 L858,260" stroke="#FF4500" stroke-width="1.5" fill="none" opacity="0.55"/>

  <!-- Noise dots — left -->
  <circle class="d1" cx="75"  cy="55"  r="1.8" fill="#FF4500" opacity="0.6"/>
  <circle class="d2" cx="110" cy="215" r="1.2" fill="#F5ECD7" opacity="0.3"/>
  <circle class="d3" cx="55"  cy="155" r="2"   fill="#FF6B00" opacity="0.35"/>
  <circle class="d4" cx="90"  cy="235" r="1"   fill="#F5ECD7" opacity="0.2"/>
  <!-- Noise dots — right -->
  <circle class="d5" cx="825" cy="60"  r="1.8" fill="#FF4500" opacity="0.6"/>
  <circle class="d6" cx="858" cy="200" r="1.2" fill="#F5ECD7" opacity="0.3"/>
  <circle class="d7" cx="808" cy="140" r="2"   fill="#FF6B00" opacity="0.35"/>
  <circle class="d8" cx="840" cy="238" r="1"   fill="#F5ECD7" opacity="0.2"/>

  <!-- Scanline sweep -->
  <rect class="scan" x="0" y="0" width="900" height="50" fill="url(#sl)" opacity="0.4"/>

  <!-- Orange rules -->
  <line class="line-t" x1="315" y1="70" x2="585" y2="70" stroke="url(#lg)" stroke-width="1.2"/>
  <line class="line-b" x1="315" y1="200" x2="585" y2="200" stroke="url(#lg)" stroke-width="1.2"/>

  <!-- NM — chromatic aberration -->
  <text class="nm-red"  x="453" y="188" text-anchor="middle" transform="translate(4,-2)">NM</text>
  <text class="nm-blue" x="453" y="188" text-anchor="middle" transform="translate(-4,2)">NM</text>
  <text class="nm-main" x="450" y="188" text-anchor="middle">NM</text>

  <!-- Labels -->
  <text class="label-top" x="450" y="55" text-anchor="middle">MUHAMMAD  NOUMAN</text>
  <text class="label-sub" x="450" y="224" text-anchor="middle">FULL STACK DEV  ·  MERN  ·  TYPESCRIPT 95%+  ·  50+ PROJECTS</text>

  <!-- Cursor -->
  <rect class="cursor" x="626" y="212" width="7" height="14" fill="#FF4500"/>

  <!-- Chip badges -->
  <g class="chips">
    <rect x="296" y="242" width="118" height="20" rx="4" fill="rgba(255,69,0,0.08)" stroke="#FF4500" stroke-width="0.6"/>
    <text x="355" y="255.5" text-anchor="middle" font-family="Courier New,monospace" font-size="8.5" fill="#FF4500" letter-spacing="1.5">📍 ISLAMABAD, PK</text>

    <rect x="424" y="242" width="178" height="20" rx="4" fill="rgba(34,197,94,0.07)" stroke="#22c55e" stroke-width="0.6"/>
    <text x="513" y="255.5" text-anchor="middle" font-family="Courier New,monospace" font-size="8.5" fill="#22c55e" letter-spacing="1.5">🟢 OPEN · REMOTE · GULF</text>
  </g>
</svg>

<br/>

[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/nouman-frontenddev)
[![Email](https://img.shields.io/badge/email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:nomimalik8051@gmail.com)
[![GitHub](https://img.shields.io/badge/github-%23181717.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/nomiwsd)
[![WhatsApp](https://img.shields.io/badge/whatsapp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/923187680511)

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════
     WHO AM I — terminal block
════════════════════════════════════════════════════════════ -->

```ts
// muhammad-nouman.config.ts

export const developer = {
  name:        "Muhammad Nouman",
  title:       "Full Stack Developer  —  MERN Stack Specialist",
  experience:  "2+ years  ·  50+ production projects delivered",
  current:     "Software Engineer @ Inflix Limited, Islamabad",
  typescript:  "95%+ coverage across all enterprise applications",
  core:        ["React.js", "Next.js 14+", "Node.js", "Express.js", "MongoDB"],
  also:        ["Redux Toolkit", "Stripe/PayPal", "Electron.js", "Prisma", "GSAP"],
  domains:     ["E-Commerce", "Healthcare", "Food Tech", "Fintech", "Blockchain"],
  available:   "Remote  ·  Pakistan  ·  Saudi Arabia  ·  Qatar  ·  UAE",
  reach:       "nomimalik8051@gmail.com  ·  +92 318 7680511",
} as const;
```

<br/>

<!-- ═══════════════════════════════════════════════════════════
     SKILLS — animated SVG bars
════════════════════════════════════════════════════════════ -->

## ⬛ &nbsp;Skills

<div align="center">

<svg width="860" height="375" viewBox="0 0 860 375" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      .sk  { font-family:'Courier New',monospace; font-size:11px; fill:#F5ECD7; letter-spacing:0.8px; }
      .pct { font-family:'Courier New',monospace; font-size:10px; fill:#FF4500; }
      .hd  { font-family:Impact,'Arial Black',sans-serif; font-size:11px; fill:#FF4500; letter-spacing:3px; }
      @keyframes bw { from{width:0} to{width:var(--w)} }
      .b{animation:bw 1.3s cubic-bezier(0.23,1,0.32,1) both;}
      .b1 {--w:211px; animation-delay:0.10s;}
      .b2 {--w:209px; animation-delay:0.18s;}
      .b3 {--w:209px; animation-delay:0.26s;}
      .b4 {--w:198px; animation-delay:0.34s;}
      .b5 {--w:202px; animation-delay:0.42s;}
      .b6 {--w:187px; animation-delay:0.50s;}
      .b7 {--w:176px; animation-delay:0.58s;}
      .b8 {--w:204px; animation-delay:0.14s;}
      .b9 {--w:204px; animation-delay:0.22s;}
      .b10{--w:192px; animation-delay:0.30s;}
      .b11{--w:197px; animation-delay:0.38s;}
      .b12{--w:173px; animation-delay:0.46s;}
      .b13{--w:180px; animation-delay:0.54s;}
    </style>
    <linearGradient id="go" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%"   stop-color="#FF4500"/>
      <stop offset="100%" stop-color="#FF8C00"/>
    </linearGradient>
    <linearGradient id="gb" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%"   stop-color="#2563EB"/>
      <stop offset="100%" stop-color="#06B6D4"/>
    </linearGradient>
  </defs>

  <rect width="860" height="375" fill="#0D0D0D" rx="8"/>

  <!-- ── LEFT: Frontend ── -->
  <text class="hd" x="40" y="36">▸ FRONTEND</text>

  <text class="sk"  x="40"  y="62">React.js</text><text class="pct" x="212" y="62">96%</text>
  <rect x="40" y="67" width="220" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b1" x="40" y="67" width="0" height="5" rx="2.5" fill="url(#go)"/>

  <text class="sk"  x="40"  y="93">Next.js 14+</text><text class="pct" x="212" y="93">95%</text>
  <rect x="40" y="98" width="220" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b2" x="40" y="98" width="0" height="5" rx="2.5" fill="url(#go)"/>

  <text class="sk"  x="40"  y="124">TypeScript</text><text class="pct" x="212" y="124">95%+</text>
  <rect x="40" y="129" width="220" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b3" x="40" y="129" width="0" height="5" rx="2.5" fill="url(#go)"/>

  <text class="sk"  x="40"  y="155">Redux Toolkit</text><text class="pct" x="212" y="155">90%</text>
  <rect x="40" y="160" width="220" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b4" x="40" y="160" width="0" height="5" rx="2.5" fill="url(#go)"/>

  <text class="sk"  x="40"  y="186">Tailwind CSS</text><text class="pct" x="212" y="186">92%</text>
  <rect x="40" y="191" width="220" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b5" x="40" y="191" width="0" height="5" rx="2.5" fill="url(#go)"/>

  <text class="sk"  x="40"  y="217">GSAP / Framer Motion</text><text class="pct" x="212" y="217">85%</text>
  <rect x="40" y="222" width="220" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b6" x="40" y="222" width="0" height="5" rx="2.5" fill="url(#go)"/>

  <text class="sk"  x="40"  y="248">Electron.js</text><text class="pct" x="212" y="248">80%</text>
  <rect x="40" y="253" width="220" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b7" x="40" y="253" width="0" height="5" rx="2.5" fill="url(#go)"/>

  <!-- divider -->
  <line x1="300" y1="22" x2="300" y2="350" stroke="#1e1e1e" stroke-width="1"/>

  <!-- ── RIGHT: Backend ── -->
  <text class="hd" x="330" y="36">▸ BACKEND &amp; CLOUD</text>

  <text class="sk"  x="330" y="62">Node.js / Express.js</text><text class="pct" x="564" y="62">85%</text>
  <rect x="330" y="67" width="240" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b8"  x="330" y="67" width="0" height="5" rx="2.5" fill="url(#gb)"/>

  <text class="sk"  x="330" y="93">MongoDB / Prisma ORM</text><text class="pct" x="564" y="93">85%</text>
  <rect x="330" y="98" width="240" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b9"  x="330" y="98" width="0" height="5" rx="2.5" fill="url(#gb)"/>

  <text class="sk"  x="330" y="124">Firebase / Supabase</text><text class="pct" x="564" y="124">82%</text>
  <rect x="330" y="129" width="240" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b10" x="330" y="129" width="0" height="5" rx="2.5" fill="url(#gb)"/>

  <text class="sk"  x="330" y="155">Stripe / PayPal / Webhooks</text><text class="pct" x="564" y="155">83%</text>
  <rect x="330" y="160" width="240" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b11" x="330" y="160" width="0" height="5" rx="2.5" fill="url(#gb)"/>

  <text class="sk"  x="330" y="186">Python / Django</text><text class="pct" x="564" y="186">72%</text>
  <rect x="330" y="191" width="240" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b12" x="330" y="191" width="0" height="5" rx="2.5" fill="url(#gb)"/>

  <text class="sk"  x="330" y="217">Git / CI-CD / Docker</text><text class="pct" x="564" y="217">75%</text>
  <rect x="330" y="222" width="240" height="5" rx="2.5" fill="#1c1c1c"/>
  <rect class="b b13" x="330" y="222" width="0" height="5" rx="2.5" fill="url(#gb)"/>

  <!-- ── Stats row ── -->
  <line x1="28" y1="278" x2="832" y2="278" stroke="#1a1a1a" stroke-width="1"/>

  <text x="107" y="310" text-anchor="middle" font-family="Impact,Arial,sans-serif" font-size="32" fill="#FF4500">2+</text>
  <text x="107" y="330" text-anchor="middle" font-family="Courier New,monospace" font-size="8.5" fill="#F5ECD7" opacity="0.4" letter-spacing="1.5">YEARS EXP</text>

  <line x1="214" y1="285" x2="214" y2="345" stroke="#1a1a1a" stroke-width="1"/>

  <text x="322" y="310" text-anchor="middle" font-family="Impact,Arial,sans-serif" font-size="32" fill="#FF4500">50+</text>
  <text x="322" y="330" text-anchor="middle" font-family="Courier New,monospace" font-size="8.5" fill="#F5ECD7" opacity="0.4" letter-spacing="1.5">PROJECTS</text>

  <line x1="430" y1="285" x2="430" y2="345" stroke="#1a1a1a" stroke-width="1"/>

  <text x="538" y="310" text-anchor="middle" font-family="Impact,Arial,sans-serif" font-size="32" fill="#FF4500">10+</text>
  <text x="538" y="330" text-anchor="middle" font-family="Courier New,monospace" font-size="8.5" fill="#F5ECD7" opacity="0.4" letter-spacing="1.5">PROD SITES</text>

  <line x1="646" y1="285" x2="646" y2="345" stroke="#1a1a1a" stroke-width="1"/>

  <text x="748" y="310" text-anchor="middle" font-family="Impact,Arial,sans-serif" font-size="32" fill="#FF4500">99%</text>
  <text x="748" y="330" text-anchor="middle" font-family="Courier New,monospace" font-size="8.5" fill="#F5ECD7" opacity="0.4" letter-spacing="1.5">TS COVERAGE</text>
</svg>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════
     EXPERIENCE — clean timeline
════════════════════════════════════════════════════════════ -->

## ⬛ &nbsp;Experience

<table>
<tr>
<td width="22%" valign="top" align="right">

`Jul 2024 → Now`

</td>
<td width="4%" align="center">🔶</td>
<td width="74%" valign="top">

**Software Engineer — MERN Stack** &nbsp;·&nbsp; **Inflix Limited**, Islamabad

- Architected **Zextons** e-commerce (Next.js 14, TS 99.8%) — 1000+ products, **40% faster** loads via SSR/SSG
- Integrated **Stripe + PayPal** with webhooks — **99.9% uptime**, automated reconciliation
- Built **Sell Zextons** resale marketplace — automated price evaluation, multi-vendor dashboards, RBAC
- Redux Toolkit architecture — cut prop drilling **40%**, boosted app performance **30%**
- Shipped **GTechGuide** blogging platform (TS 97%) — Supabase, Cloudinary, Prisma ORM

</td>
</tr>
<tr>
<td width="22%" valign="top" align="right">

`Oct 2023 → Jun 2024`

</td>
<td width="4%" align="center">🔷</td>
<td width="74%" valign="top">

**Frontend Developer** &nbsp;·&nbsp; **Vesprr**, Wah Cantt *(Remote)*

- Delivered **5+ client projects** — Shipzilla, An Nakhla Aid, Servfind — 100% client satisfaction
- Built **An Nakhla Aid** charity site — donation tracking, donor management, automated PDF receipts
- Developed **Servfind** PMS — task tracking, team collaboration, admin + client dashboards
- Implemented **Chart.js** data dashboards, role-based auth, real-time update capabilities

</td>
</tr>
</table>

<br/>

<!-- ═══════════════════════════════════════════════════════════
     PROJECTS — 2-column table cards
════════════════════════════════════════════════════════════ -->

## ⬛ &nbsp;Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 🛒 &nbsp;Zextons E-Commerce
`Production` &nbsp;·&nbsp; **TS 99.8%**

Complete e-commerce solution — 1000+ products, SSR for SEO, cart, wishlist, JWT auth, RBAC, admin dashboard, and full Stripe + PayPal integration.

`Next.js 14` &nbsp;`Redux` &nbsp;`MongoDB` &nbsp;`Stripe` &nbsp;`PayPal` &nbsp;`ShadcnUI`

</td>
<td width="50%" valign="top">

### 📦 &nbsp;Sell Zextons — Resale Market
`Production` &nbsp;·&nbsp; **TS 95.8%**

Tech gadget resale marketplace — automated price evaluation engine, multi-vendor seller dashboards, quality verification, admin approval workflows.

`Next.js` &nbsp;`TypeScript` &nbsp;`Redux` &nbsp;`MongoDB` &nbsp;`Tailwind`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ✍️ &nbsp;GTechGuide Blogging Platform
`Production` &nbsp;·&nbsp; **TS 97%**

Modern blog platform — CRUD posts, advanced search, cloud media management, Prisma ORM, Supabase auth.

`Next.js` &nbsp;`Supabase` &nbsp;`Prisma` &nbsp;`Cloudinary` &nbsp;`TypeScript`

</td>
<td width="50%" valign="top">

### 🍽️ &nbsp;Benny's Kitchen — Food Ordering
`Production` &nbsp;·&nbsp; **TS 97.5%**

Restaurant platform — digital menu, online ordering, real-time order tracking, customer push notifications.

`Next.js` &nbsp;`React.js` &nbsp;`TypeScript` &nbsp;`Tailwind CSS`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🖥️ &nbsp;EasyDine — Desktop POS
`Enterprise` &nbsp;·&nbsp; **Cross-Platform**

Full restaurant POS — order management, kitchen display, billing, inventory tracking. **Works offline** — Windows / macOS / Linux.

`Electron.js` &nbsp;`React.js` &nbsp;`Node.js` &nbsp;`MongoDB`

</td>
<td width="50%" valign="top">

### 🕌 &nbsp;Islamic Worship App
`Production` &nbsp;·&nbsp; **Full Stack**

Cross-platform Islamic app — prayer times, Quran, Hadith library, Islamic calendar. Python/Django backend for data processing.

`Next.js` &nbsp;`TypeScript` &nbsp;`Python` &nbsp;`Django`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🏠 &nbsp;Ruhr Property Website
`Production`

Real estate platform — property listings, virtual tours, advanced filters, Google Maps integration.

`React.js` &nbsp;`Tailwind CSS` &nbsp;`Google Maps API`

</td>
<td width="50%" valign="top">

### 🧪 &nbsp;Chemical Sticker Generator
`Production`

Custom chemical / safety sticker creator — template library, preview, PDF export for labs and workplaces.

`React.js` &nbsp;`Node.js` &nbsp;`Express.js` &nbsp;`MongoDB`

</td>
</tr>
</table>

<br/>

<!-- ═══════════════════════════════════════════════════════════
     GITHUB STATS
════════════════════════════════════════════════════════════ -->

## ⬛ &nbsp;GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=nomiwsd&show_icons=true&hide_border=true&theme=github_dark&count_private=true&include_all_commits=true&title_color=FF4500&icon_color=FF4500&text_color=F5ECD7&bg_color=0D0D0D" height="168"/>
&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=nomiwsd&layout=compact&hide_border=true&theme=github_dark&title_color=FF4500&text_color=F5ECD7&bg_color=0D0D0D" height="168"/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=nomiwsd&hide_border=true&theme=github-dark-blue&ring=FF4500&fire=FF4500&currStreakLabel=FF4500&background=0D0D0D&sideLabels=F5ECD7&currStreakNum=F5ECD7&dates=555555&stroke=1a1a1a" height="148"/>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════
     EDUCATION
════════════════════════════════════════════════════════════ -->

## ⬛ &nbsp;Education & Certifications

```
🎓  B.Sc. Computer Science          University of Wah, Wah Cantt         2019 – 2023
📜  Front-End Development           Meta (Coursera)                       Certified
📜  JavaScript Programming          Meta (Coursera)                       Certified
```

<br/>

<!-- ═══════════════════════════════════════════════════════════
     FOOTER BANNER
════════════════════════════════════════════════════════════ -->

<div align="center">

<svg width="860" height="80" viewBox="0 0 860 80" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes availPulse { 0%,100%{opacity:0.55} 50%{opacity:1} }
      .avail-dot { animation:availPulse 1.8s ease-in-out infinite; }
    </style>
  </defs>
  <rect width="860" height="80" rx="8" fill="#0D0D0D"/>
  <line x1="30" y1="40" x2="830" y2="40" stroke="#1a1a1a" stroke-width="1"/>
  <circle class="avail-dot" cx="48" cy="40" r="5" fill="#22c55e"/>
  <text x="62" y="44" font-family="Courier New,monospace" font-size="10.5" fill="#22c55e" letter-spacing="1.5">AVAILABLE — REMOTE  ·  PAKISTAN  ·  SAUDI ARABIA  ·  QATAR  ·  UAE</text>
  <text x="430" y="62" text-anchor="middle" font-family="Courier New,monospace" font-size="9" fill="#F5ECD7" opacity="0.35" letter-spacing="2">nomimalik8051@gmail.com  ·  +92 318 7680511  ·  github.com/nomiwsd</text>
</svg>

<sub>Crafted with intent — not templates &nbsp;·&nbsp; Muhammad Nouman &nbsp;·&nbsp; 2025</sub>

</div>
