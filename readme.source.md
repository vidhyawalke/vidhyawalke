```aura width=860 height=120
<div style={{
  width: '100%', height: '100%', background: '#0d1117',
  display: 'flex', alignItems: 'center', fontFamily: 'Inter',
  position: 'relative', overflow: 'hidden', borderRadius: 8,
  border: '1px solid #30363d',
  padding: '0 24px'
}}>
  {/* Left: Avatar with elegant thin border */}
  <div style={{
    width: 64, height: 64, borderRadius: 32,
    border: '2px solid #30363d',
    display: 'flex', alignItems: 'center', justifyContent: 'center',
    marginRight: 20
  }}>
    <img src={github.user.avatarUrl || 'https://github.com/vidhyawalke.png'} width={58} height={58} style={{ borderRadius: 29 }} />
  </div>

  {/* Center/Info: Name, Bio, and Stats */}
  <div style={{ display: 'flex', flexDirection: 'column', gap: 4, flexGrow: 1 }}>
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
  <div style={{ display: 'flex', gap: 6, alignItems: 'center' }}>
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
  backgroundColor="#21262d"
  width={110}
  height={32}
  gradientStops={[
    { offset: '0%', color: '#30363d' },
    { offset: '100%', color: '#21262d' },
  ]}
/>
```

```aura width=100 height=32 link="mailto:vidhya.walke.official@gmail.com" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/gmail-icon.svg"
  text="Email"
  backgroundColor="#21262d"
  width={100}
  height={32}
  gradientStops={[
    { offset: '0%', color: '#30363d' },
    { offset: '100%', color: '#21262d' },
  ]}
/>
```

```aura width=105 height=32 link="https://www.kaggle.com/vidhyaw" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/kaggle-icon.svg"
  text="Kaggle"
  backgroundColor="#21262d"
  width={105}
  height={32}
  gradientStops={[
    { offset: '0%', color: '#30363d' },
    { offset: '100%', color: '#21262d' },
  ]}
/>
```

```aura width=100 height=32 link="https://vidhyawalke.blogspot.com/" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/blogger-icon.svg"
  text="Blog"
  backgroundColor="#21262d"
  width={100}
  height={32}
  gradientStops={[
    { offset: '0%', color: '#30363d' },
    { offset: '100%', color: '#21262d' },
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
