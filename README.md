<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Priyadarshani — Work & Projects</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=DM+Mono:wght@400;500&family=Inter:wght@400;500&display=swap" rel="stylesheet"/>
<style>
:root {
  --bg: #0e0e10;
  --bg2: #16161a;
  --bg3: #1e1e24;
  --border: rgba(255,255,255,0.08);
  --border2: rgba(255,255,255,0.14);
  --text: #e8e8f0;
  --muted: #888899;
  --dim: #555566;
  --accent-a: #6ee7b7;   /* teal */
  --accent-b: #a78bfa;   /* purple */
  --accent-c: #fb923c;   /* orange */
  --accent-d: #60a5fa;   /* blue */
  --display: 'Syne', sans-serif;
  --mono: 'DM Mono', monospace;
  --body: 'Inter', sans-serif;
}
* { box-sizing: border-box; margin: 0; padding: 0; }
body {
  background: var(--bg);
  color: var(--text);
  font-family: var(--body);
  font-size: 14px;
  line-height: 1.65;
  min-height: 100vh;
}

/* ── page wrapper ── */
.page { max-width: 980px; margin: 0 auto; padding: 56px 40px 80px; }

/* ── hero ── */
.hero { margin-bottom: 72px; }
.hero-eyebrow {
  font-family: var(--mono);
  font-size: 11px;
  letter-spacing: .15em;
  text-transform: uppercase;
  color: var(--accent-a);
  margin-bottom: 16px;
}
.hero h1 {
  font-family: var(--display);
  font-size: clamp(48px, 7vw, 88px);
  font-weight: 800;
  line-height: 1.0;
  letter-spacing: -2px;
  color: #fff;
  margin-bottom: 24px;
}
.hero h1 em { color: var(--accent-b); font-style: normal; }
.hero-desc {
  max-width: 540px;
  font-size: 15px;
  color: var(--muted);
  line-height: 1.7;
  margin-bottom: 28px;
}
.hero-tags { display: flex; flex-wrap: wrap; gap: 8px; }
.tag {
  font-family: var(--mono);
  font-size: 11px;
  padding: 4px 11px;
  border-radius: 20px;
  border: 1px solid var(--border2);
  color: var(--muted);
  white-space: nowrap;
}
.tag.a { border-color: var(--accent-a); color: var(--accent-a); }
.tag.b { border-color: var(--accent-b); color: var(--accent-b); }
.tag.c { border-color: var(--accent-c); color: var(--accent-c); }
.tag.d { border-color: var(--accent-d); color: var(--accent-d); }

/* ── section ── */
.section { margin-bottom: 64px; }
.section-label {
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: .18em;
  text-transform: uppercase;
  color: var(--dim);
  margin-bottom: 24px;
  padding-bottom: 12px;
  border-bottom: 1px solid var(--border);
}

/* ── project cards ── */
.projects { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
.card {
  background: var(--bg2);
  border: 1px solid var(--border);
  border-radius: 12px;
  padding: 24px;
  position: relative;
  overflow: hidden;
  transition: border-color .2s, transform .15s;
}
.card:hover { border-color: var(--border2); transform: translateY(-2px); }
.card-accent {
  position: absolute; top: 0; left: 0; right: 0;
  height: 2px;
}
.card.ca .card-accent { background: var(--accent-a); }
.card.cb .card-accent { background: var(--accent-b); }
.card.cc .card-accent { background: var(--accent-c); }
.card.cd .card-accent { background: var(--accent-d); }

.card-num {
  font-family: var(--mono);
  font-size: 11px;
  color: var(--dim);
  margin-bottom: 12px;
}
.card h3 {
  font-family: var(--display);
  font-size: 17px;
  font-weight: 700;
  color: #fff;
  margin-bottom: 6px;
  line-height: 1.3;
}
.card-meta {
  font-family: var(--mono);
  font-size: 11px;
  color: var(--dim);
  margin-bottom: 14px;
}
.card-desc {
  font-size: 13px;
  color: var(--muted);
  line-height: 1.6;
  margin-bottom: 16px;
}
.card-stats { display: flex; flex-wrap: wrap; gap: 8px; margin-bottom: 16px; }
.stat-pill {
  font-family: var(--mono);
  font-size: 11px;
  padding: 3px 10px;
  border-radius: 4px;
  background: var(--bg3);
  color: var(--text);
}
.card.ca .stat-pill { background: rgba(110,231,183,.1); color: var(--accent-a); }
.card.cb .stat-pill { background: rgba(167,139,250,.1); color: var(--accent-b); }
.card.cc .stat-pill { background: rgba(251,146,60,.1); color: var(--accent-c); }
.card.cd .stat-pill { background: rgba(96,165,250,.1); color: var(--accent-d); }

.card-chips { display: flex; flex-wrap: wrap; gap: 6px; }
.chip {
  font-size: 11px;
  padding: 2px 8px;
  border-radius: 3px;
  background: var(--bg3);
  color: var(--dim);
  border: 1px solid var(--border);
}

.award {
  display: inline-flex; align-items: center; gap: 5px;
  font-family: var(--mono); font-size: 10.5px;
  background: rgba(251,191,36,.1);
  color: #fbbf24;
  border: 1px solid rgba(251,191,36,.25);
  padding: 3px 10px; border-radius: 4px; margin-bottom: 12px;
}

/* ── stack grid ── */
.stack-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 12px;
}
.stack-block {
  background: var(--bg2);
  border: 1px solid var(--border);
  border-radius: 10px;
  padding: 16px;
}
.stack-block h4 {
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: .12em;
  text-transform: uppercase;
  color: var(--dim);
  margin-bottom: 10px;
}
.stack-block p {
  font-family: var(--mono);
  font-size: 12px;
  color: var(--muted);
  line-height: 1.8;
}

/* ── timeline ── */
.timeline { display: flex; flex-direction: column; gap: 0; }
.tl-item {
  display: grid;
  grid-template-columns: 120px 1fr;
  gap: 24px;
  padding: 20px 0;
  border-bottom: 1px solid var(--border);
}
.tl-item:last-child { border-bottom: none; }
.tl-year {
  font-family: var(--mono);
  font-size: 11px;
  color: var(--dim);
  padding-top: 2px;
}
.tl-content h4 {
  font-family: var(--display);
  font-size: 14px;
  font-weight: 700;
  color: var(--text);
  margin-bottom: 2px;
}
.tl-content p { font-size: 13px; color: var(--muted); }

/* ── links ── */
.links { display: flex; gap: 12px; }
.link-btn {
  font-family: var(--mono);
  font-size: 12px;
  padding: 8px 18px;
  border-radius: 6px;
  border: 1px solid var(--border2);
  color: var(--muted);
  text-decoration: none;
  transition: all .15s;
  display: inline-flex; align-items: center; gap: 6px;
}
.link-btn:hover { border-color: var(--accent-a); color: var(--accent-a); }
.link-btn.primary { background: var(--accent-a); color: #0e0e10; border-color: var(--accent-a); font-weight: 600; }
.link-btn.primary:hover { opacity: .9; }

@media (max-width: 680px) {
  .page { padding: 32px 20px; }
  .projects { grid-template-columns: 1fr; }
  .stack-grid { grid-template-columns: 1fr 1fr; }
  .tl-item { grid-template-columns: 1fr; gap: 4px; }
}
</style>
</head>
<body>
<div class="page">

  <!-- ── HERO ── -->
  <div class="hero">
    <div class="hero-eyebrow">// data scientist · ai/ml · fordham university</div>
    <h1>Priyadarshani<br/><em>Gangurde</em></h1>
    <p class="hero-desc">
      I build ML systems that predict, classify, and explain — across healthcare,
      finance, and retail. 6+ years shipping end-to-end pipelines from raw data
      to deployed models.
    </p>
    <div class="hero-tags">
      <span class="tag a">Python</span>
      <span class="tag a">TensorFlow</span>
      <span class="tag a">PyTorch</span>
      <span class="tag b">LangChain</span>
      <span class="tag b">Vertex AI</span>
      <span class="tag c">AWS SageMaker</span>
      <span class="tag c">Snowflake</span>
      <span class="tag d">Tableau</span>
      <span class="tag d">Power BI</span>
      <span class="tag">XGBoost</span>
      <span class="tag">MLflow</span>
      <span class="tag">Docker</span>
    </div>
  </div>

  <!-- ── PROJECTS ── -->
  <div class="section">
    <div class="section-label">// selected projects</div>
    <div class="projects">

      <!-- IoMT -->
      <div class="card ca">
        <div class="card-accent"></div>
        <div class="card-num">01</div>
        <div class="award">🏆 2nd Prize · Fordham CIS 2025</div>
        <h3>IoMT Intrusion Detection</h3>
        <div class="card-meta">Master's Thesis · Fordham University · 2024–2025</div>
        <p class="card-desc">
          Protocol-aware ML system detecting cyberattacks on medical IoT devices.
          Benchmarked 8 classifiers across 4 class-balancing strategies on the
          CICIoMT2024 dataset. Balanced Random Forest achieved 98% recall on rare
          MQTT and Spoofing attacks.
        </p>
        <div class="card-stats">
          <span class="stat-pill">7.8M records</span>
          <span class="stat-pill">48 features</span>
          <span class="stat-pill">99.81% accuracy</span>
          <span class="stat-pill">Macro F1 = 0.97</span>
        </div>
        <div class="card-chips">
          <span class="chip">Python</span>
          <span class="chip">Scikit-learn</span>
          <span class="chip">XGBoost</span>
          <span class="chip">SMOTE</span>
          <span class="chip">Random Forest</span>
        </div>
      </div>

      <!-- Customer Segmentation -->
      <div class="card cb">
        <div class="card-accent"></div>
        <div class="card-num">02</div>
        <h3>Customer Segmentation & Product Recommendation</h3>
        <div class="card-meta">Fordham University · 2025</div>
        <p class="card-desc">
          Full recommendation pipeline on 392K retail transactions. RFM analysis →
          K-Means clustering → Market Basket (Apriori) → Neural Network collaborative
          filter. Three independent recommendation engines for each customer cluster.
        </p>
        <div class="card-stats">
          <span class="stat-pill">392K transactions</span>
          <span class="stat-pill">Silhouette = 0.41</span>
          <span class="stat-pill">1M+ Apriori rules</span>
          <span class="stat-pill">94% significant</span>
        </div>
        <div class="card-chips">
          <span class="chip">K-Means</span>
          <span class="chip">TensorFlow</span>
          <span class="chip">mlxtend</span>
          <span class="chip">RFM</span>
          <span class="chip">Apriori</span>
        </div>
      </div>

      <!-- AI Flashcard -->
      <div class="card cc">
        <div class="card-accent"></div>
        <div class="card-num">03</div>
        <h3>AI Flashcard Generator</h3>
        <div class="card-meta">Fordham University · Published Paper · 2024</div>
        <p class="card-desc">
          AI teaching assistant that transforms YouTube videos into structured Q&amp;A
          flashcards. Handles transcript retrieval, tiktoken preprocessing, LangChain
          key-concept extraction via Gemini, and JSON output delivery. Designed for
          students, educators, and self-learners.
        </p>
        <div class="card-stats">
          <span class="stat-pill">FastAPI backend</span>
          <span class="stat-pill">LLM-powered</span>
          <span class="stat-pill">Peer reviewed</span>
        </div>
        <div class="card-chips">
          <span class="chip">LangChain</span>
          <span class="chip">Vertex AI</span>
          <span class="chip">FastAPI</span>
          <span class="chip">YouTube API</span>
          <span class="chip">tiktoken</span>
        </div>
      </div>

      <!-- CO2 -->
      <div class="card cd">
        <div class="card-accent"></div>
        <div class="card-num">04</div>
        <h3>CO₂ Emissions Prediction</h3>
        <div class="card-meta">Fordham University · 2023</div>
        <p class="card-desc">
          Predicted vehicle tailpipe emissions from engine features on 7,385 Canadian
          vehicle records. Full pipeline: EDA, transmission/fuel-type encoding, Z-score
          outlier removal, feature normalization, 80/20 split, model training, and
          interactive Plotly visualizations for stakeholders.
        </p>
        <div class="card-stats">
          <span class="stat-pill">LR R² = 0.906</span>
          <span class="stat-pill">RF R² = 0.973</span>
          <span class="stat-pill">7,385 records</span>
        </div>
        <div class="card-chips">
          <span class="chip">Random Forest</span>
          <span class="chip">Linear Regression</span>
          <span class="chip">Plotly</span>
          <span class="chip">Pandas</span>
          <span class="chip">Scikit-learn</span>
        </div>
      </div>

    </div>
  </div>

  <!-- ── STACK ── -->
  <div class="section">
    <div class="section-label">// tech stack</div>
    <div class="stack-grid">
      <div class="stack-block">
        <h4>Languages</h4>
        <p>Python<br/>SQL<br/>R</p>
      </div>
      <div class="stack-block">
        <h4>ML / DL</h4>
        <p>TensorFlow<br/>PyTorch<br/>XGBoost<br/>Scikit-learn</p>
      </div>
      <div class="stack-block">
        <h4>Cloud / MLOps</h4>
        <p>AWS SageMaker<br/>Snowflake<br/>Databricks<br/>MLflow · Docker</p>
      </div>
      <div class="stack-block">
        <h4>GenAI</h4>
        <p>LangChain<br/>Vertex AI<br/>Gemini API<br/>FastAPI</p>
      </div>
    </div>
  </div>

  <!-- ── EXPERIENCE ── -->
  <div class="section">
    <div class="section-label">// experience</div>
    <div class="timeline">
      <div class="tl-item">
        <div class="tl-year">2024 →</div>
        <div class="tl-content">
          <h4>Data Scientist — Philips</h4>
          <p>Healthcare AI · New Jersey, USA · EHR modeling, NLP on clinical notes, AWS SageMaker pipelines</p>
        </div>
      </div>
      <div class="tl-item">
        <div class="tl-year">2020 – 2023</div>
        <div class="tl-content">
          <h4>Data Analyst — Deloitte</h4>
          <p>Consulting · India · Marketing analytics, churn prediction (XGBoost), +12% SMS CTR</p>
        </div>
      </div>
      <div class="tl-item">
        <div class="tl-year">2018 – 2020</div>
        <div class="tl-content">
          <h4>Data Analyst — Genpact</h4>
          <p>Banking & Financial Services · India · Credit risk, fraud detection, ARIMA forecasting</p>
        </div>
      </div>
      <div class="tl-item">
        <div class="tl-year">2023 – 2025</div>
        <div class="tl-content">
          <h4>MS in Data Science — Fordham University</h4>
          <p>New York, USA · Graduate School of Arts & Science</p>
        </div>
      </div>
    </div>
  </div>

  <!-- ── LINKS ── -->
  <div class="section">
    <div class="section-label">// contact</div>
    <div class="links">
      <a class="link-btn primary" href="mailto:iampriyadarshanigangurde@gmail.com">✉ Email me</a>
      <a class="link-btn" href="https://www.linkedin.com/in/darshani-pri-31b413403/">↗ LinkedIn</a>
    </div>
  </div>

</div>
</body>
</html>
