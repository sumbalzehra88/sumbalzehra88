<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Sumbal Zehra — Computer Systems Engineering portfolio featuring machine learning, embedded AI, IoT, networking, and digital systems projects.">
<title>Sumbal Zehra — Portfolio</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Mono:wght@400;500&family=Syne:wght@400;500;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@2.44.0/tabler-icons.min.css">
<style>
*{box-sizing:border-box;margin:0;padding:0}
:root{
  --bg:#0a0a0a;
  --surface:#111111;
  --surface2:#1a1a1a;
  --border:#2a2a2a;
  --text:#f0ede8;
  --muted:#6b6b6b;
  --accent:#e8d5b0;
  --accent2:#4a9eff;
  --green:#3ecf8e;
  --red:#ff6b6b;
}
body{background:var(--bg);color:var(--text);font-family:'Syne',sans-serif;min-height:100vh;-webkit-font-smoothing:antialiased}
a{color:inherit;text-decoration:none}
.wrap{max-width:720px;margin:0 auto;padding:3rem 2rem 5rem}

.hero{margin-bottom:3rem;padding-bottom:2.5rem;border-bottom:1px solid var(--border)}
.hero-tag{font-family:'DM Mono',monospace;font-size:11px;color:var(--accent);letter-spacing:0.15em;text-transform:uppercase;margin-bottom:1rem;opacity:0.8}
.hero-name{font-family:'DM Serif Display',serif;font-size:clamp(2.4rem,6vw,3.6rem);line-height:1.05;color:var(--text);margin-bottom:0.6rem}
.hero-name em{font-style:italic;color:var(--accent)}
.hero-sub{font-size:14px;color:var(--muted);line-height:1.8;max-width:480px;margin-bottom:1.75rem}
.hero-links{display:flex;gap:10px;flex-wrap:wrap}
.pill{display:inline-flex;align-items:center;gap:6px;font-family:'DM Mono',monospace;font-size:11px;padding:7px 16px;border:1px solid var(--border);border-radius:100px;color:var(--muted);text-decoration:none;transition:all 0.2s}
.pill:hover{border-color:var(--accent);color:var(--accent)}
.pill i{font-size:14px}

.section-label{font-family:'DM Mono',monospace;font-size:10px;letter-spacing:0.2em;color:var(--muted);text-transform:uppercase;margin-bottom:1.5rem;display:flex;align-items:center;gap:12px}
.section-label::after{content:'';flex:1;height:1px;background:var(--border)}

.stats-row{display:grid;grid-template-columns:repeat(3,1fr);gap:8px;margin-bottom:3rem}
.stat{background:var(--surface);border:1px solid var(--border);border-radius:10px;padding:1.25rem;text-align:center}
.stat-num{font-family:'DM Serif Display',serif;font-size:2rem;color:var(--accent);line-height:1}
.stat-label{font-family:'DM Mono',monospace;font-size:10px;color:var(--muted);margin-top:5px;letter-spacing:0.05em}

.internship{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:1.75rem;margin-bottom:3rem;position:relative;overflow:hidden}
.internship::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;background:linear-gradient(90deg,var(--green),var(--accent2))}
.int-header{display:flex;align-items:flex-start;justify-content:space-between;margin-bottom:0.75rem;gap:12px}
.int-title{font-family:'DM Serif Display',serif;font-size:1.2rem;color:var(--text)}
.int-org{font-size:12px;color:var(--green);font-family:'DM Mono',monospace;margin-top:4px}
.int-badge{font-family:'DM Mono',monospace;font-size:9px;padding:4px 12px;border-radius:100px;border:1px solid var(--green);color:var(--green);white-space:nowrap;flex-shrink:0}
.int-desc{font-size:13px;color:var(--muted);line-height:1.8}
.int-desc strong{color:#b0a898;font-weight:500}

.projects{display:flex;flex-direction:column;gap:8px;margin-bottom:3rem}
.proj{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:1.75rem;transition:border-color 0.2s;position:relative;overflow:hidden}
.proj::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;opacity:0;transition:opacity 0.2s}
.proj:hover{border-color:#333}
.proj:hover::before{opacity:1}
.proj.featured::before{background:linear-gradient(90deg,var(--accent),#c9a96e);opacity:1}
.proj.ml::before{background:linear-gradient(90deg,var(--accent2),#7b5ea7);opacity:1}
.proj.embedded::before{background:linear-gradient(90deg,var(--green),#1a8a5e);opacity:1}
.proj.net::before{background:linear-gradient(90deg,var(--red),#c94a4a);opacity:1}
.proj.algo::before{background:linear-gradient(90deg,#a78bfa,#7c5cbf);opacity:1}
.proj.hw::before{background:linear-gradient(90deg,#fb923c,#d97706);opacity:1}

.proj-header{display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:0.75rem;gap:12px}
.proj-title{font-family:'DM Serif Display',serif;font-size:1.15rem;color:var(--text);line-height:1.2}
.proj-year{font-family:'DM Mono',monospace;font-size:10px;color:var(--muted);margin-top:4px}
.proj-badge{font-family:'DM Mono',monospace;font-size:9px;padding:4px 12px;border-radius:100px;border:1px solid;flex-shrink:0;white-space:nowrap}
.badge-featured{border-color:#c9a96e;color:#c9a96e}
.badge-research{border-color:var(--accent2);color:var(--accent2)}
.badge-iot{border-color:var(--green);color:var(--green)}
.badge-network{border-color:var(--red);color:var(--red)}
.badge-algo{border-color:#a78bfa;color:#a78bfa}
.badge-hw{border-color:#fb923c;color:#fb923c}

.proj-desc{font-size:13px;color:var(--muted);line-height:1.8;margin-bottom:1rem}
.proj-desc strong{color:#b0a898;font-weight:500}

.proj-footer{display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:8px}
.tags{display:flex;flex-wrap:wrap;gap:6px}
.tag{font-family:'DM Mono',monospace;font-size:10px;padding:3px 10px;background:var(--surface2);border:1px solid var(--border);border-radius:4px;color:var(--muted)}
.proj-link{font-family:'DM Mono',monospace;font-size:10px;color:var(--accent2);display:flex;align-items:center;gap:4px;transition:opacity 0.2s}
.proj-link:hover{opacity:0.7}

.skills-grid{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:3rem}
.skill-block{background:var(--surface);border:1px solid var(--border);border-radius:10px;padding:1.1rem}
.skill-block-label{font-family:'DM Mono',monospace;font-size:10px;color:var(--accent);letter-spacing:0.1em;margin-bottom:10px}
.skill-items{display:flex;flex-wrap:wrap;gap:6px}
.skill-item{font-size:11px;color:var(--muted);padding:4px 10px;background:var(--surface2);border-radius:4px;border:1px solid var(--border);display:inline-flex;align-items:center;gap:6px}
.skill-item i{font-size:14px}

.github-snake-section{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:1.5rem;margin-bottom:3rem;text-align:center;overflow:hidden}
.github-snake-section img{width:100%;height:auto;border-radius:6px;background:#111111;padding:10px}

.certs{display:flex;flex-direction:column;gap:6px;margin-bottom:3rem}
.cert{display:flex;align-items:center;gap:12px;background:var(--surface);border:1px solid var(--border);border-radius:8px;padding:0.85rem 1rem}
.cert-dot{width:6px;height:6px;border-radius:50%;background:var(--accent);flex-shrink:0}
.cert-name{font-size:13px;color:var(--text)}
.cert-org{font-family:'DM Mono',monospace;font-size:10px;color:var(--muted);margin-left:auto;flex-shrink:0}

.edu{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:1.75rem;margin-bottom:3rem}
.edu-name{font-family:'DM Serif Display',serif;font-size:1.15rem;color:var(--text);margin-bottom:4px}
.edu-meta{font-family:'DM Mono',monospace;font-size:11px;color:var(--accent);margin-bottom:0.75rem}
.edu-desc{font-size:13px;color:var(--muted);line-height:1.8}

.footer{text-align:center;font-family:'DM Mono',monospace;font-size:11px;color:var(--muted);padding-top:2rem;border-top:1px solid var(--border);line-height:2}

@media(max-width:500px){
  .stats-row{grid-template-columns:repeat(3,1fr)}
  .skills-grid{grid-template-columns:1fr}
  .hero-name{font-size:2rem}
  .cert-org{display:none}
}
</style>
</head>
<body>
<div class="wrap">

  <div class="hero">
    <div class="hero-tag">Portfolio — 2026</div>
    <div class="hero-name">Sumbal <em>Zehra</em></div>
    <p class="hero-sub">Computer Systems Engineering undergraduate at NED University of Engineering & Technology. Building at the intersection of machine learning, embedded AI, and real-world safety systems.</p>
    <div class="hero-links">
      <a class="pill" href="https://github.com/sumbalzehra88" target="_blank"><i class="ti ti-brand-github"></i>sumbalzehra88</a>
      <a class="pill" href="mailto:sumbalzehra88@gmail.com"><i class="ti ti-mail"></i>sumbalzehra88@gmail.com</a>
      <span class="pill"><i class="ti ti-map-pin"></i>Karachi, Pakistan</span>
    </div>
  </div>

  <div class="stats-row">
    <div class="stat"><div class="stat-num">5+</div><div class="stat-label">Projects</div></div>
    <div class="stat"><div class="stat-num">6+</div><div class="stat-label">Certifications</div></div>
    <div class="stat"><div class="stat-num">220+</div><div class="stat-label">LeetCode problems</div></div>
  </div>

  <div class="section-label">Research internship</div>

  <div class="internship">
    <div class="int-header">
      <div>
        <div class="int-title">Autonomous Vehicle Research Intern</div>
        <div class="int-org">NCAI — National Centre of Artificial Intelligence</div>
      </div>
      <div class="int-badge">Current</div>
    </div>
    <p class="int-desc">Gaining hands-on research experience in <strong>Embedded AI, Computer Vision, and Machine Learning</strong> through structured research activities. Working independently in a remote research setting — conducting literature reviews, synthesising findings, and communicating results clearly.</p>
  </div>

  <div class="section-label">Projects</div>

  <div class="projects">

    <div class="proj featured">
      <div class="proj-header">
        <div>
          <div class="proj-title">Construction_Analysis</div>
          <div class="proj-year">2025 — 2026</div>
        </div>
        <div class="proj-badge badge-featured">Featured</div>
      </div>
      <p class="proj-desc">Binary classification system predicting <strong>construction site fatalities</strong> from multi-source NYC data. Collected and merged data from NYC OpenData, OpenWeatherMap Historical API, and DOB Permit Issuance datasets to build a custom 1,253-row dataset with 27 features. Trained five ML algorithms — Logistic Regression, KNN, SVM, Naive Bayes, and ANN — with <strong>incremental learning</strong> for continuous model updates without full retraining. Applied SMOTE, IQR outlier treatment, standardisation, and geospatial fatality mapping.</p>
      <div class="proj-footer">
        <div class="tags">
          <span class="tag">Python</span><span class="tag">PyTorch</span><span class="tag">Scikit-learn</span><span class="tag">SMOTE</span><span class="tag">Incremental Learning</span><span class="tag">Folium</span>
        </div>
        <a class="proj-link" href="https://github.com/sumbalzehra88" target="_blank"><i class="ti ti-brand-github" style="font-size:13px"></i>View repo</a>
      </div>
    </div>

    <div class="proj ml">
      <div class="proj-header">
        <div>
          <div class="proj-title">ML From Scratch</div>
          <div class="proj-year">2025</div>
        </div>
        <div class="proj-badge badge-research">Research</div>
      </div>
      <p class="proj-desc">Implemented core machine learning algorithms from first principles without high-level library abstractions. Built to deeply understand the mathematical foundations of <strong>gradient descent, backpropagation, decision boundaries</strong>, and model optimisation.</p>
      <div class="proj-footer">
        <div class="tags">
          <span class="tag">Python</span><span class="tag">NumPy</span><span class="tag">Linear Algebra</span><span class="tag">Statistics</span>
        </div>
        <a class="proj-link" href="https://github.com/sumbalzehra88" target="_blank"><i class="ti ti-brand-github" style="font-size:13px"></i>View repo</a>
      </div>
    </div>

    <div class="proj embedded">
      <div class="proj-header">
        <div>
          <div class="proj-title">SAFESNIFF — Gas Leakage Detection</div>
          <div class="proj-year">2024</div>
        </div>
        <div class="proj-badge badge-iot">IoT</div>
      </div>
      <p class="proj-desc">Real-time IoT-based LPG gas leakage detection system with <strong>automated alarms and instant mobile alerts</strong> via the Blynk platform. Detects dangerous gas concentrations and notifies users immediately, designed for residential and industrial deployment.</p>
      <div class="proj-footer">
        <div class="tags">
          <span class="tag">Embedded C</span><span class="tag">ESP32</span><span class="tag">Blynk</span><span class="tag">IoT</span><span class="tag">Arduino IDE</span>
        </div>
      </div>
    </div>

    <div class="proj net">
      <div class="proj-header">
        <div>
          <div class="proj-title">SDN Firewall with End-to-End Encryption</div>
          <div class="proj-year">2024</div>
        </div>
        <div class="proj-badge badge-network">Network</div>
      </div>
      <p class="proj-desc">High-performance network security solution combining <strong>Software Defined Networking with end-to-end encryption</strong> and Zero Trust access control. Implements dynamic traffic filtering and secure communication channels at the network layer.</p>
      <div class="proj-footer">
        <div class="tags">
          <span class="tag">Python</span><span class="tag">SDN</span><span class="tag">Encryption</span><span class="tag">Zero Trust</span><span class="tag">Shell</span><span class="tag">HTML</span>
        </div>
      </div>
    </div>

    <div class="proj algo">
      <div class="proj-header">
        <div>
          <div class="proj-title">ResearchFlow — AI Research Platform</div>
          <div class="proj-year">2025</div>
        </div>
        <div class="proj-badge badge-algo">Agentic AI</div>
      </div>
      <p class="proj-desc">Built a research tool mapping citation networks as an interactive graph using a hybrid BM25 + dense retrieval pipeline, with automated, source-traceable report generation using Gemini API.</p>
      <div class="proj-footer">
        <div class="tags">
          <span class="tag">Python</span><span class="tag">Gemini API</span><span class="tag">Firebase</span><span class="tag">Chroma</span><span class="tag">LangChain</span>
        </div>
      </div>
    </div>

    <div class="proj hw">
      <div class="proj-header">
        <div>
          <div class="proj-title">Processor & Digital Logic Design</div>
          <div class="proj-year">2023 — 2024</div>
        </div>
        <div class="proj-badge badge-hw">Hardware</div>
      </div>
      <p class="proj-desc">Designed a <strong>basic processor, MIPS architecture simulation</strong>, and a world clock using logic gates and multiplexers. Built and simulated combinational and sequential circuits using Verilog HDL and Logisim.</p>
      <div class="proj-footer">
        <div class="tags">
          <span class="tag">Verilog HDL</span><span class="tag">MIPS</span><span class="tag">Logisim</span><span class="tag">DLD</span>
        </div>
      </div>
    </div>

  </div>

  <div class="section-label">Skills</div>

  <div class="skills-grid">
    <div class="skill-block">
      <div class="skill-block-label">Languages</div>
      <div class="skill-items">
        <span class="skill-item"><i class="ti ti-brand-python" style="color:#4584b6"></i>Python</span>
        <span class="skill-item"><i class="ti ti-code" style="color:#00599f"></i>C</span>
        <span class="skill-item"><i class="ti ti-code" style="color:#004482"></i>C++</span>
        <span class="skill-item"><i class="ti ti-database" style="color:#f29111"></i>SQL</span>
        <span class="skill-item"><i class="ti ti-brand-javascript" style="color:#f7df1e"></i>JavaScript</span>
        <span class="skill-item"><i class="ti ti-brand-html5" style="color:#e34f26"></i>HTML</span>
        <span class="skill-item"><i class="ti ti-brand-css3" style="color:#1572b6"></i>CSS</span>
      </div>
    </div>
    <div class="skill-block">
      <div class="skill-block-label">ML & Frameworks</div>
      <div class="skill-items">
        <span class="skill-item"><i class="ti ti-brain" style="color:#ee4c2c"></i>PyTorch</span>
        <span class="skill-item"><i class="ti ti-cpu" style="color:#ff6f00"></i>TensorFlow</span>
        <span class="skill-item"><i class="ti ti-atom" style="color:#d00000"></i>Keras</span>
        <span class="skill-item"><i class="ti ti-chart-dots" style="color:#f89939"></i>Scikit-learn</span>
        <span class="skill-item"><i class="ti ti-table" style="color:#013243"></i>NumPy</span>
        <span class="skill-item"><i class="ti ti-chart-bar" style="color:#130654"></i>Pandas</span>
      </div>
    </div>
    <div class="skill-block">
      <div class="skill-block-label">Agentic AI & LLM Tooling</div>
      <div class="skill-items">
        <span class="skill-item"><i class="ti ti-message-chatbot" style="color:#3ecf8e"></i>LangChain</span>
        <span class="skill-item"><i class="ti ti-git-fork" style="color:#4a9eff"></i>LangGraph</span>
        <span class="skill-item"><i class="ti ti-file-search" style="color:#e8d5b0"></i>RAG</span>
        <span class="skill-item"><i class="ti ti-wand" style="color:#a78bfa"></i>Prompt Eng.</span>
        <span class="skill-item"><i class="ti ti-robot" style="color:#3ecf8e"></i>AI Agents</span>
      </div>
    </div>
    <div class="skill-block">
      <div class="skill-block-label">Embedded, Tools & DevOps</div>
      <div class="skill-items">
        <span class="skill-item"><i class="ti ti-cpu" style="color:#00979d"></i>ESP32 / ESP8266</span>
        <span class="skill-item"><i class="ti ti-brand-docker" style="color:#2496ed"></i>Docker</span>
        <span class="skill-item"><i class="ti ti-brand-git" style="color:#f05032"></i>Git</span>
        <span class="skill-item"><i class="ti ti-brand-linux" style="color:#fcc624"></i>Linux</span>
        <span class="skill-item"><i class="ti ti-brand-figma" style="color:#f24e1e"></i>Figma</span>
      </div>
    </div>
  </div>

  <div class="section-label">GitHub Activity</div>
  <div class="github-snake-section">
    <img src="https://raw.githubusercontent.com/sumbalzehra88/sumbalzehra88/output/github-contribution-grid-snake.svg" alt="GitHub Contribution Snake Animation" />
  </div>

  <div class="section-label">Certifications</div>

  <div class="certs">
    <div class="cert"><div class="cert-dot"></div><span class="cert-name">AI Fundamentals</span><span class="cert-org">Google</span></div>
    <div class="cert"><div class="cert-dot"></div><span class="cert-name">Introduction to Machine Learning</span><span class="cert-org">Duke University</span></div>
    <div class="cert"><div class="cert-dot"></div><span class="cert-name">Shallow Neural Networks</span><span class="cert-org">DeepLearning Institute</span></div>
    <div class="cert"><div class="cert-dot"></div><span class="cert-name">Generative AI Explained</span><span class="cert-org">NVIDIA DLI</span></div>
    <div class="cert"><div class="cert-dot"></div><span class="cert-name">Introduction to Generative AI</span><span class="cert-org">NVIDIA DLI</span></div>
    <div class="cert"><div class="cert-dot"></div><span class="cert-name">IoT with ESP32 and ESP8266</span><span class="cert-org">NCL NEDUET</span></div>
  </div>

  <div class="section-label">Education</div>

  <div class="edu">
    <div class="edu-name">NED University of Engineering & Technology</div>
    <div class="edu-meta">BE — Computer Systems Engineering &nbsp;·&nbsp; 2023 – Present &nbsp;·&nbsp; CGPA 3.47</div>
    <p class="edu-desc">Relevant coursework: Machine Learning, Data Structures and Algorithms, Embedded Systems, Digital Logic Design, Object-Oriented Programming.</p>
  </div>

  <div class="footer">
    Sumbal Zehra &nbsp;·&nbsp; sumbalzehra88@gmail.com &nbsp;·&nbsp; github.com/sumbalzehra88<br>
    <span style="font-size:10px;opacity:0.5">© 2026</span>
  </div>

</div>
</body>
</html>
