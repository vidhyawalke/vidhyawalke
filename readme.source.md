```aura width=860 height=120
<div style={{
  width: '100%', height: '100%', background: '#0d1117',
  display: 'flex', alignItems: 'center', fontFamily: 'Inter',
  position: 'relative', overflow: 'hidden', borderRadius: 8,
  border: '1px solid #30363d',
  padding: '0 24px'
}}>
  {/* Sleek top gradient accent line to add premium 'life' */}
  <div style={{
    position: 'absolute', top: 0, left: 0, width: '100%', height: 3,
    background: 'linear-gradient(90deg, #6366f1, #a855f7, #3b82f6)'
  }} />

  {/* Soft, slow-pulsing background glow that looks alive but professional */}
  <style>
    {`
      @keyframes soft-pulse {
        0%, 100% { transform: translate(0px, 0px) scale(1); opacity: 0.6; }
        50% { transform: translate(30px, -15px) scale(1.1); opacity: 0.85; }
      }
      #glow-bg {
        animation: soft-pulse 20s ease-in-out infinite;
      }
    `}
  </style>

  <svg width="860" height="120" style={{ position: 'absolute', top: 0, left: 0, pointerEvents: 'none' }}>
    <defs>
      <radialGradient id="g1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(99, 102, 241, 0.22)" />
        <stop offset="50%" stopColor="rgba(168, 85, 247, 0.10)" />
        <stop offset="100%" stopColor="rgba(168, 85, 247, 0)" />
      </radialGradient>
      <radialGradient id="g2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(59, 130, 246, 0.15)" />
        <stop offset="60%" stopColor="rgba(59, 130, 246, 0.06)" />
        <stop offset="100%" stopColor="rgba(59, 130, 246, 0)" />
      </radialGradient>
    </defs>
    <ellipse id="glow-bg" cx="720" cy="60" rx="260" ry="160" fill="url(#g1)" />
    <ellipse cx="480" cy="70" rx="180" ry="110" fill="url(#g2)" />
  </svg>

  {/* Left: Avatar with elegant purple border */}
  <div style={{
    width: 64, height: 64, borderRadius: 32,
    border: '2px solid rgba(168, 85, 247, 0.4)',
    display: 'flex', alignItems: 'center', justifyContent: 'center',
    marginRight: 20, zIndex: 10
  }}>
    <img src={github.user.avatarUrl || 'https://github.com/vidhyawalke.png'} width={58} height={58} style={{ borderRadius: 29 }} />
  </div>

  {/* Center/Info: Name, Bio, and Stats */}
  <div style={{ display: 'flex', flexDirection: 'column', gap: 4, flexGrow: 1, zIndex: 10 }}>
    <div style={{ display: 'flex', alignItems: 'baseline', gap: 12 }}>
      <span style={{ fontSize: 24, fontWeight: 700, color: '#ffffff', letterSpacing: '-0.5px' }}>
        Vidhya Walke
      </span>
      <span style={{ fontSize: 13, color: '#8b949e', fontWeight: 400 }}>
        Goa, India
      </span>
    </div>
    
    <div style={{ display: 'flex', fontSize: 14, color: '#c9d1d9', fontWeight: 400 }}>
      Data Science Graduate &bull; MERN Stack Developer &bull; Data Analytics Enthusiast
    </div>

    {/* Compact stats line */}
    <div style={{ display: 'flex', gap: 12, marginTop: 4, fontSize: 12, color: '#8b949e', fontWeight: 500 }}>
      <span style={{ color: '#58a6ff' }}>{github.stats.totalRepos} Repositories</span>
      <span>&bull;</span>
      <span style={{ color: '#a371f7' }}>{github.stats.totalStars} Stars</span>
      <span>&bull;</span>
      <span style={{ color: '#34d399' }}>{github.stats.totalCommits} Commits</span>
    </div>
  </div>

  {/* Right: Clean, professional tags (Python, React, SQL) */}
  <div style={{ display: 'flex', gap: 6, alignItems: 'center', zIndex: 10 }}>
    {['Python', 'React', 'SQL', 'MongoDB'].map(function(tag) {
      return (
        <div key={tag} style={{
          display: 'flex', padding: '4px 10px', borderRadius: 4,
          background: '#21262d', border: '1px solid #30363d',
          color: '#c9d1d9', fontSize: 11, fontWeight: 600,
        }}>{tag}</div>
      );
    })}
  </div>
</div>
```

```aura width=110 height=32 link="https://linkedin.com/in/vidhyawalke" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/linkedin-icon.png"
  text="LinkedIn"
  backgroundColor="#000000"
  width={110}
  height={32}
  gradientStops={[
    { offset: '0%', color: '#1d4ed8' },
    { offset: '100%', color: '#1e3a8a' },
  ]}
/>
```

```aura width=100 height=32 link="mailto:vidhya.walke.official@gmail.com" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/gmail-icon.svg"
  text="Email"
  backgroundColor="#000000"
  width={100}
  height={32}
  gradientStops={[
    { offset: '0%', color: '#b91c1c' },
    { offset: '100%', color: '#7f1d1d' },
  ]}
/>
```

```aura width=105 height=32 link="https://www.kaggle.com/vidhyaw" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/kaggle-icon.svg"
  text="Kaggle"
  backgroundColor="#000000"
  width={105}
  height={32}
  gradientStops={[
    { offset: '0%', color: '#0369a1' },
    { offset: '100%', color: '#0c4a6e' },
  ]}
/>
```

```aura width=100 height=32 link="https://vidhyawalke.blogspot.com/" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/blogger-icon.svg"
  text="Blog"
  backgroundColor="#000000"
  width={100}
  height={32}
  gradientStops={[
    { offset: '0%', color: '#c2410c' },
    { offset: '100%', color: '#7c2d12' },
  ]}
/>
```

<p align="center"><sub>𝗉𝗈𝗐𝖾𝗋𝖾𝖽 𝖻𝗒 <a href="https://github.com/collectioneur/readme-aura">𝗋𝖾𝖺𝖽𝗆𝖾-𝖺𝗎𝗋𝖺</a></sub></p>

---

## About Me

I'm a fresh M.Sc. Data Science graduate with hands-on experience in full-stack web development. I enjoy building things end to end, from training ML models to shipping web apps, and I care about writing clean code that holds up in the real world.

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
