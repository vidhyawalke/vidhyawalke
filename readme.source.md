```aura width=760 height=140
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

  <svg width="760" height="140" style={{ position: 'absolute', top: 0, left: 0, pointerEvents: 'none' }}>
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

  {/* Name and subtitle */}
  <div style={{ display: 'flex', flexDirection: 'column', gap: 5, flexGrow: 1, zIndex: 10 }}>
    <div style={{ display: 'flex', fontSize: 28, fontWeight: 800, color: '#ffffff', letterSpacing: '-0.7px', lineHeight: 1 }}>
      Vidhya Walke
    </div>
    <div style={{ display: 'flex', fontSize: 11, color: 'rgba(210,205,255,0.82)', fontWeight: 500, letterSpacing: '0.8px' }}>
      M.Sc. DATA SCIENCE GRADUATE · GOA, INDIA
    </div>
  </div>
</div>
```

```aura width=142 height=44 link="https://vidhya-walke-portfolio.vercel.app/" inline align=center
<div style={{ display: 'flex', width: '100%', height: '100%', alignItems: 'center', justifyContent: 'center', padding: '0 6px' }}>
  <SocialMediaButton
    icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/portfolio-icon.svg?v=2"
    text="Portfolio"
    backgroundColor="#000000"
    width={130}
    height={44}
    gradientStops={[
      { offset: '0%', color: '#2dd4bf' },
      { offset: '30%', color: '#000000' },
      { offset: '60%', color: '#34d399' },
      { offset: '80%', color: '#000000' },
      { offset: '100%', color: '#10b981' },
    ]}
  />
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

```aura width=142 height=44 link="https://leetcode.com/u/vidhyawalke/" inline align=center
<div style={{ display: 'flex', width: '100%', height: '100%', alignItems: 'center', justifyContent: 'center', padding: '0 6px' }}>
  <SocialMediaButton
    icon="https://raw.githubusercontent.com/vidhyawalke/vidhyawalke/main/icons/leetcode-icon.svg"
    text="LeetCode"
    backgroundColor="#000000"
    width={130}
    height={44}
    gradientStops={[
      { offset: '0%', color: '#ffa116' },
      { offset: '30%', color: '#000000' },
      { offset: '60%', color: '#ffb800' },
      { offset: '80%', color: '#000000' },
      { offset: '100%', color: '#f89b14' },
    ]}
  />
</div>
```



---

# Vidhya Walke - Data Science & Full Stack Developer

<p align="center">
  <a href="https://vidhya-walke-portfolio.vercel.app/"><strong>🌐 Portfolio</strong></a> &nbsp;•&nbsp;
  <a href="https://linkedin.com/in/vidhyawalke"><strong>💼 LinkedIn</strong></a> &nbsp;•&nbsp;
  <a href="mailto:vidhya.walke.official@gmail.com"><strong>✉️ Email</strong></a> &nbsp;•&nbsp;
  <a href="https://www.kaggle.com/vidhyawalke"><strong>📊 Kaggle</strong></a> &nbsp;•&nbsp;
  <a href="https://leetcode.com/u/vidhyawalke/"><strong>💻 LeetCode</strong></a> &nbsp;•&nbsp;
  <a href="https://github.com/vidhyawalke"><strong>🐙 GitHub</strong></a>
</p>

> **M.Sc. Data Science Graduate & Full Stack Developer** specializing in Machine Learning, Retrieval-Augmented Generation (RAG), and Web Applications. Based in Goa, India.

---

## 👨‍💻 About Me

I’m **Vidhya Walke**, a full-stack developer with a strong academic and practical foundation in data science (M.Sc. Data Science from Goa Business School, Goa University). I bridge the gap between machine learning algorithms and production web systems, transforming complex data into scalable, accessible, and intuitive digital experiences.

- 🤖 **Applied AI & Machine Learning:** Building LLM applications, semantic search with FAISS and LangChain, and predictive machine learning models.
- 🌐 **Full-Stack Web Development:** Developing fast, responsive web applications using React, Node.js, FastAPI, and modern frontend architectures.
- 📊 **Data Science & Analytics:** Exploratory data analysis, statistical modeling, recommendation systems, and interactive Tableau dashboards.
- 🎯 **Continuous Learning:** Solving algorithmic problems on LeetCode and building open-source projects.

---

## 🚀 Featured Projects

### 1. [RAG PDF Knowledge Assistant](https://github.com/vidhyawalke/rag-pdf-knowledge-assistant)
*AI-Powered Document Assistant & Semantic Search Engine*
- **Problem & Solution:** Enables semantic search and grounded question-answering over lengthy PDF documents. Indexes document text into dense vector embeddings using FAISS cosine similarity and queries Google Gemini asynchronously via FastAPI with strict page citation tags to eliminate hallucinations.
- **Tech Stack:** `Python`, `FastAPI`, `FAISS`, `Google Gemini API`, `LangChain`
- **Links:** [Repository](https://github.com/vidhyawalke/rag-pdf-knowledge-assistant)

### 2. [CO–PO Correlation Assessment Tool](https://github.com/vidhyawalke/co-po-mapper)
*Curriculum Mapping & Accreditation Analytics Web App*
- **Problem & Solution:** Developed an institutional curriculum assessment platform during my DMC internship that calculates Course Outcome (CO) to Program Outcome (PO) attainment matrices from raw student marks. Replaced manual spreadsheet macros, saving over 70% of calculation time with NAAC-compliant audit reports.
- **Tech Stack:** `React`, `Zustand`, `SheetJS`, `Tailwind CSS`, `JavaScript`
- **Links:** [Repository](https://github.com/vidhyawalke/co-po-mapper)

### 3. [Customer Segmentation Prediction App](https://github.com/vidhyawalke/customer-segmentations-kmeans-app)
*Unsupervised Machine Learning & Interactive Streamlit Web App*
- **Problem & Solution:** Operationalizes unsupervised customer segmentation into a production-ready web application using PyCaret and KMeans clustering. Allows marketers to input customer behavioral and demographic metrics to receive instant cluster predictions and cohort breakdowns.
- **Tech Stack:** `Python`, `PyCaret`, `Streamlit`, `Scikit-Learn`, `Pandas`
- **Links:** [Repository](https://github.com/vidhyawalke/customer-segmentations-kmeans-app)

### 4. [Spam Email Classification Model](https://github.com/vidhyawalke/spam-email-classification)
*End-to-End NLP & Deep Learning Spam Classifier*
- **Problem & Solution:** Built an NLP pipeline comparing classical machine learning classifiers with Artificial Neural Networks (ANN) and Long Short-Term Memory (LSTM) recurrent architectures. Achieves 99.2% spam detection accuracy and is deployed as an interactive Streamlit app for real-time inference.
- **Tech Stack:** `Python`, `Streamlit`, `LSTM`, `ANN`, `TF-IDF`, `NLP`, `Scikit-Learn`
- **Links:** [Repository](https://github.com/vidhyawalke/spam-email-classification)

### 5. [Goodreads Web Scraping Pipeline](https://github.com/vidhyawalke/goodreads-web-scraping)
*Automated Web Scraping & Data Extraction Pipeline*
- **Problem & Solution:** Crawls and parses multi-page Goodreads book catalogs using throttled HTTP requests and Selenium. Captures book titles, author metadata, ratings, and reader engagement metrics into clean, structured CSV datasets ready for exploratory data analysis.
- **Tech Stack:** `Python`, `BeautifulSoup`, `Selenium`, `Requests`, `Pandas`
- **Links:** [Repository](https://github.com/vidhyawalke/goodreads-web-scraping)

### 6. [Movie Recommendation System](https://github.com/vidhyawalke/Movie-Recommendation-System-in-Python)
*Collaborative Filtering & Matrix Factorization Engine*
- **Problem & Solution:** Predicts user ratings and generates top-N recommendations on 100,000 MovieLens ratings across 943 users and 1,682 movies using user-based and item-based collaborative filtering alongside Singular Value Decomposition (SVD) matrix factorization to tackle data sparsity.
- **Tech Stack:** `Python`, `Collaborative Filtering`, `SVD`, `Scikit-Learn`, `Pandas`
- **Links:** [Repository](https://github.com/vidhyawalke/Movie-Recommendation-System-in-Python)

---

## 🛠️ Skills & Technologies

| Domain | Technologies & Frameworks |
| :--- | :--- |
| **Languages** | Python, SQL, JavaScript (ES6+), HTML5, CSS3, R |
| **Data Science & AI/ML** | Machine Learning, Retrieval-Augmented Generation (RAG), Deep Learning (ANN, LSTM), NLP, Recommendation Systems, FAISS Vector Search, Scikit-Learn, PyCaret, Pandas, NumPy |
| **Web & Full Stack** | React, Node.js, FastAPI, Flask, Streamlit, RESTful APIs, Tailwind CSS, Vite |
| **Databases & Tools** | PostgreSQL, MongoDB, Git, GitHub, Tableau, Docker, Jupyter Notebook, Google Search Console |

---

## 🤝 Connect with Me

- 🌐 **Portfolio Website:** [vidhya-walke-portfolio.vercel.app](https://vidhya-walke-portfolio.vercel.app/)
- 💼 **LinkedIn:** [linkedin.com/in/vidhyawalke](https://www.linkedin.com/in/vidhyawalke)
- 🐙 **GitHub:** [github.com/vidhyawalke](https://github.com/vidhyawalke)
- 📊 **Kaggle:** [kaggle.com/vidhyawalke](https://www.kaggle.com/vidhyawalke)
- 💻 **LeetCode:** [leetcode.com/u/vidhyawalke](https://leetcode.com/u/vidhyawalke/)
- 📧 **Email:** [vidhya.walke.official@gmail.com](mailto:vidhya.walke.official@gmail.com)

---

<p align="center">
  <sub>Designed & Developed by <a href="https://github.com/vidhyawalke">Vidhya Walke</a> • © 2026</sub>
</p>
