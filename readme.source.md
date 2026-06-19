```aura width=860 height=180
<div style={{
  width: '100%', height: '100%', background: '#08080c',
  display: 'flex', alignItems: 'center', fontFamily: 'Inter',
  position: 'relative', overflow: 'hidden', borderRadius: 16,
  border: '1px solid rgba(110,80,220,0.18)',
  padding: '0 40px'
}}>

  <style>
    {`
      @keyframes float-slow {
        0%, 100% { transform: translateX(0px); opacity: 0.8; }
        50% { transform: translateX(300px); opacity: 1.2; }
      }
      @keyframes float-medium {
        0%, 100% { transform: translateX(0px); opacity: 0.7; }
        50% { transform: translateX(-200px); opacity: 1.1; }
      }
      @keyframes float-fast {
        0%, 100% { transform: translateX(0px); opacity: 0.9; }
        50% { transform: translateX(150px); opacity: 0.6; }
      }
      @keyframes float-diagonal {
        0%, 100% { transform: translateX(0px); opacity: 0.75; }
        50% { transform: translateX(250px); opacity: 1.0; }
      }
      @keyframes float-wave {
        0%, 100% { transform: translateX(0px); opacity: 0.65; }
        33% { transform: translateX(-120px); opacity: 0.9; }
        66% { transform: translateX(60px); opacity: 1.0; }
      }
      @keyframes float-pulse {
        0%, 100% { transform: scale(1); opacity: 0.8; }
        50% { transform: scale(1.2) translateY(-10px); opacity: 0.4; }
      }
      #glow-1 { animation: float-slow 8s ease-in-out infinite; }
      #glow-2 { animation: float-medium 12s ease-in-out infinite; }
      #glow-3 { animation: float-fast 9s ease-in-out infinite; }
      #glow-4 { animation: float-slow 11s ease-in-out infinite reverse; }
      #glow-5 { animation: float-medium 14s ease-in-out infinite reverse; }
      #glow-6 { animation: float-diagonal 10s ease-in-out infinite; }
      #glow-7 { animation: float-wave 13s ease-in-out infinite; }
      #glow-8 { animation: float-pulse 7s ease-in-out infinite; }
    `}
  </style>

  <svg width="860" height="180" style={{ position: 'absolute', top: 0, left: 0, pointerEvents: 'none' }}>
    <defs>
      <radialGradient id="g1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(110,20,210,0.72)" />
        <stop offset="40%" stopColor="rgba(90,15,180,0.35)" />
        <stop offset="70%" stopColor="rgba(90,15,180,0)" />
      </radialGradient>
      <radialGradient id="g2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(40,60,255,0.6)" />
        <stop offset="45%" stopColor="rgba(30,50,200,0.25)" />
        <stop offset="70%" stopColor="rgba(30,50,200,0)" />
      </radialGradient>
      <radialGradient id="g3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0,130,255,0.45)" />
        <stop offset="50%" stopColor="rgba(0,100,220,0.18)" />
        <stop offset="70%" stopColor="rgba(0,100,220,0)" />
      </radialGradient>
      <radialGradient id="g4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0,190,230,0.32)" />
        <stop offset="70%" stopColor="rgba(0,190,230,0)" />
      </radialGradient>
      <radialGradient id="g5" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(90,30,200,0.38)" />
        <stop offset="70%" stopColor="rgba(90,30,200,0)" />
      </radialGradient>
      <radialGradient id="g6" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(160,30,255,0.55)" />
        <stop offset="45%" stopColor="rgba(130,20,220,0.22)" />
        <stop offset="70%" stopColor="rgba(130,20,220,0)" />
      </radialGradient>
      <radialGradient id="g7" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(20,60,255,0.42)" />
        <stop offset="50%" stopColor="rgba(10,40,200,0.16)" />
        <stop offset="70%" stopColor="rgba(10,40,200,0)" />
      </radialGradient>
      <radialGradient id="g8" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0,170,255,0.40)" />
        <stop offset="50%" stopColor="rgba(0,130,220,0.15)" />
        <stop offset="70%" stopColor="rgba(0,130,220,0)" />
      </radialGradient>
    </defs>

    <ellipse id="glow-1" cx="180" cy="180" rx="260" ry="150" fill="url(#g1)" />
    <ellipse id="glow-2" cx="300" cy="190" rx="220" ry="130" fill="url(#g2)" />
    <ellipse id="glow-3" cx="420" cy="190" rx="180" ry="110" fill="url(#g3)" />
    <ellipse id="glow-4" cx="550" cy="200" rx="150" ry="90" fill="url(#g4)" />
    <ellipse id="glow-5" cx="750" cy="200" rx="130" ry="80" fill="url(#g5)" />
    <ellipse id="glow-6" cx="300" cy="190" rx="180" ry="110" fill="url(#g6)" />
    <ellipse id="glow-7" cx="490" cy="180" rx="220" ry="130" fill="url(#g7)" />
    <ellipse id="glow-8" cx="590" cy="200" rx="150" ry="100" fill="url(#g8)" />
  </svg>

  {/* Center/Info: Name and Bio only (No stats or tags strip) */}
  <div style={{ display: 'flex', flexDirection: 'column', gap: 6, flexGrow: 1, zIndex: 10 }}>
    <div style={{ display: 'flex', fontSize: 32, fontWeight: 800, color: '#ffffff', letterSpacing: '-1px', lineHeight: 1 }}>
      Vidhya Walke
    </div>
    
    <div style={{ display: 'flex', fontSize: 14, color: 'rgba(180,165,255,0.85)', fontWeight: 400, letterSpacing: '0.3px' }}>
      M.Sc. Data Science Graduate &bull; MERN Stack Developer &bull; Data Analytics Enthusiast
    </div>
  </div>
</div>
```

```aura width=132 height=44 link="https://linkedin.com/in/vidhyawalke" inline align=center
<div style={{ display: 'flex', width: '100%', height: '100%', alignItems: 'center', justifyContent: 'center', padding: '0 6px' }}>
  <SocialMediaButton
    icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/linkedin-icon.png"
    text="LinkedIn"
    backgroundColor="#000000"
    width={120}
    height={44}
    gradientStops={[
      { offset: '0%', color: '#818cf8' },
      { offset: '30%', color: '#000000' },
      { offset: '60%', color: '#9298f8' },
      { offset: '80%', color: '#000000' },
      { offset: '100%', color: '#7479f5' },
    ]}
  />
</div>
```

```aura width=122 height=44 link="mailto:vidhya.walke.official@gmail.com" inline align=center
<div style={{ display: 'flex', width: '100%', height: '100%', alignItems: 'center', justifyContent: 'center', padding: '0 6px' }}>
  <SocialMediaButton
    icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/gmail-icon.svg"
    text="Email"
    backgroundColor="#000000"
    width={110}
    height={44}
    gradientStops={[
      { offset: '0%', color: '#d855f7' },
      { offset: '30%', color: '#000000' },
      { offset: '60%', color: '#b557e8' },
      { offset: '80%', color: '#000000' },
      { offset: '100%', color: '#cc6ef9' },
    ]}
  />
</div>
```

```aura width=132 height=44 link="https://www.kaggle.com/vidhyaw" inline align=center
<div style={{ display: 'flex', width: '100%', height: '100%', alignItems: 'center', justifyContent: 'center', padding: '0 6px' }}>
  <SocialMediaButton
    icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/kaggle-icon.svg"
    text="Kaggle"
    backgroundColor="#000000"
    width={120}
    height={44}
    gradientStops={[
      { offset: '0%', color: '#5dc8f9' },
      { offset: '30%', color: '#000000' },
      { offset: '60%', color: '#7dd3fc' },
      { offset: '80%', color: '#000000' },
      { offset: '100%', color: '#4ec3f8' },
    ]}
  />
</div>
```

```aura width=122 height=44 link="https://vidhyawalke.blogspot.com/" inline align=center
<div style={{ display: 'flex', width: '100%', height: '100%', alignItems: 'center', justifyContent: 'center', padding: '0 6px' }}>
  <SocialMediaButton
    icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/blogger-icon.svg"
    text="Blog"
    backgroundColor="#000000"
    width={110}
    height={44}
    gradientStops={[
      { offset: '0%', color: '#f472b6' },
      { offset: '30%', color: '#000000' },
      { offset: '60%', color: '#fb7eb8' },
      { offset: '80%', color: '#000000' },
      { offset: '100%', color: '#f06aae' },
    ]}
  />
</div>
```

---

## About Me

I recently finished my M.Sc. in Data Science. Along the way, I fell in love with full-stack web development—specifically building clean, end-to-end apps using the MERN stack. I enjoy bridging the gap between data-driven machine learning models and functional, user-facing applications. 

I'm not interested in writing code that only works on my local machine; I like building things that actually get shipped and work. Right now, I'm focused on leveling up my backend skills, sharpening my algorithms, and looking for my first professional role in data analytics, data science, or full-stack engineering.

---

## What I Work With

**Data Science & ML**
`Python` · `NumPy` · `Pandas` · `Scikit-learn` · `Matplotlib` · `Seaborn` · `LightGBM` · `Power BI` · `MySQL` · `MongoDB`

**Full-Stack Web Development (MERN)**
`MongoDB` · `Express.js` · `React` · `Node.js` · `HTML` · `CSS` · `JavaScript`

**Tools & Platforms**
`Git` · `GitHub` · `VS Code` · `Kaggle` · `Jupyter Notebook`

---

## Featured Work

Check out my pinned repositories below — they cover machine learning pipelines, data analysis notebooks, and full-stack apps.

- **ML Projects** — End-to-end classification and prediction pipelines with model evaluation
- **Data Analytics** — EDA and visualization notebooks, also published on [Kaggle](https://www.kaggle.com/vidhyaw)
- **MERN Apps** — Full-stack web applications built with MongoDB, Express, React, and Node.js

---

## Currently Working On

- Real-world ML and data analytics projects
- Full-stack applications using the MERN stack
- Data Structures and Algorithms

---

## Open To

Entry-level roles in Data Analytics, Data Science, or Full-Stack Development. Also open to freelance, remote, and open-source work.

---

## Let's Connect

[LinkedIn](https://linkedin.com/in/vidhyawalke) &nbsp;·&nbsp; [Email](mailto:vidhya.walke.official@gmail.com) &nbsp;·&nbsp; [Kaggle](https://www.kaggle.com/vidhyawalke) &nbsp;·&nbsp; [Blog](https://vidhyawalke.blogspot.com/)

---

<p align="center"><i>"Building today to become better than yesterday."</i></p>
