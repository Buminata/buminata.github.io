<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Buminata | Data Analyst & Data Science</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="description" content="Portfolio of Buminata - Data Analyst & Data Science Professional" />

  <!-- Google Font -->
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet" />

  <style>
    :root {
      --bg: #050816;
      --bg-alt: #0b1020;
      --accent: #38bdf8;
      --accent-soft: rgba(56, 189, 248, 0.12);
      --text: #e5e7eb;
      --muted: #9ca3af;
      --border: #1f2937;
      --card-bg: #0b1120;
      --radius-lg: 18px;
      --radius-md: 12px;
      --shadow-soft: 0 18px 45px rgba(15, 23, 42, 0.65);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: "Inter", system-ui, -apple-system, BlinkMacSystemFont, sans-serif;
      background: radial-gradient(circle at top, #1f2937 0, #020617 40%, #000 100%);
      color: var(--text);
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
    }

    a {
      color: var(--accent);
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    .page {
      max-width: 1040px;
      margin: 0 auto;
      padding: 32px 20px 64px;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 32px;
      gap: 16px;
    }

    .logo-text {
      font-weight: 700;
      letter-spacing: 0.08em;
      font-size: 0.85rem;
      text-transform: uppercase;
      color: var(--muted);
    }

    .pill {
      border-radius: 999px;
      padding: 6px 12px;
      border: 1px solid var(--border);
      background: rgba(15, 23, 42, 0.8);
      font-size: 0.75rem;
      display: inline-flex;
      align-items: center;
      gap: 8px;
    }

    .dot {
      width: 8px;
      height: 8px;
      border-radius: 999px;
      background: #22c55e;
      box-shadow: 0 0 10px #22c55e;
    }

    main {
      display: flex;
      flex-direction: column;
      gap: 32px;
    }

    /* Hero */
    .hero {
      display: grid;
      grid-template-columns: minmax(0, 2.1fr) minmax(0, 1.6fr);
      gap: 28px;
      align-items: center;
    }

    @media (max-width: 840px) {
      .hero {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    .hero-card {
      background: linear-gradient(145deg, rgba(15, 23, 42, 0.95), rgba(15, 23, 42, 0.9));
      border-radius: 22px;
      padding: 24px 24px 26px;
      border: 1px solid rgba(148, 163, 184, 0.2);
      box-shadow: var(--shadow-soft);
      position: relative;
      overflow: hidden;
    }

    .hero-card::before {
      content: "";
      position: absolute;
      inset: 0;
      background: radial-gradient(circle at top left, rgba(56, 189, 248, 0.18), transparent 55%);
      opacity: 0.9;
      pointer-events: none;
    }

    .hero-role {
      font-size: 0.85rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--accent);
      margin-bottom: 8px;
    }

    .hero-title {
      font-size: 2.1rem;
      font-weight: 700;
      margin-bottom: 8px;
    }

    .hero-subtitle {
      font-size: 1rem;
      color: var(--muted);
      margin-bottom: 16px;
      max-width: 520px;
    }

    .hero-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-bottom: 20px;
    }

    .hero-tag {
      background: var(--accent-soft);
      color: var(--accent);
      border-radius: 999px;
      border: 1px solid rgba(56, 189, 248, 0.35);
      padding: 6px 12px;
      font-size: 0.8rem;
    }

    .hero-footer {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      flex-wrap: wrap;
      font-size: 0.83rem;
      color: var(--muted);
    }

    .hero-links {
      display: flex;
      gap: 10px;
      flex-wrap: wrap;
    }

    .btn {
      border-radius: 999px;
      padding: 8px 14px;
      font-size: 0.82rem;
      border: 1px solid rgba(148, 163, 184, 0.45);
      background: rgba(15, 23, 42, 0.9);
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      text-decoration: none;
    }

    .btn-primary {
      background: linear-gradient(135deg, #38bdf8, #0ea5e9);
      border-color: transparent;
      color: #0b1220;
      font-weight: 600;
    }

    .btn-primary:hover {
      filter: brightness(1.05);
      text-decoration: none;
    }

    .btn:hover {
      border-color: var(--accent);
      text-decoration: none;
    }

    /* Side card */
    .side-card {
      background: rgba(15, 23, 42, 0.96);
      border-radius: 22px;
      border: 1px solid rgba(31, 41, 55, 0.9);
      padding: 18px 18px 20px;
      position: relative;
      overflow: hidden;
    }

    .avatar {
      width: 64px;
      height: 64px;
      border-radius: 18px;
      background: radial-gradient(circle at top left, #38bdf8, #1f2937);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2.2rem;
      font-weight: 700;
      color: #e5e7eb;
      margin-bottom: 12px;
    }

    .side-name {
      font-weight: 600;
      margin-bottom: 2px;
      font-size: 1rem;
    }

    .side-role {
      font-size: 0.85rem;
      color: var(--muted);
      margin-bottom: 10px;
    }

    .side-meta {
      font-size: 0.8rem;
      color: var(--muted);
      display: flex;
      flex-direction: column;
      gap: 3px;
      margin-bottom: 14px;
    }

    .side-meta span {
      display: inline-flex;
      align-items: center;
      gap: 8px;
    }

    .badge-row {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-bottom: 10px;
    }

    .mini-badge {
      font-size: 0.7rem;
      border-radius: 999px;
      padding: 4px 9px;
      border: 1px solid rgba(55, 65, 81, 0.9);
      background: #020617;
      color: var(--muted);
    }

    .stat-row {
      display: flex;
      gap: 10px;
      font-size: 0.78rem;
      color: var(--muted);
    }

    .stat-chip {
      border-radius: 999px;
      padding: 4px 9px;
      background: rgba(15, 23, 42, 0.9);
      border: 1px solid rgba(31, 41, 55, 0.9);
    }

    /* Sections */
    section {
      background: rgba(10, 15, 30, 0.95);
      border-radius: var(--radius-lg);
      border: 1px solid rgba(31, 41, 55, 0.95);
      padding: 22px 20px 20px;
      box-shadow: 0 16px 40px rgba(15, 23, 42, 0.7);
    }

    .section-title {
      font-size: 0.95rem;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      color: var(--muted);
      margin-bottom: 14px;
    }

    .section-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 14px;
    }

    .pill-tag {
      border-radius: 999px;
      padding: 4px 10px;
      font-size: 0.78rem;
      background: #020617;
      color: var(--muted);
      border: 1px solid rgba(31, 41, 55, 0.9);
    }

    .project-card {
      background: #020617;
      border-radius: var(--radius-md);
      border: 1px solid rgba(31, 41, 55, 0.95);
      padding: 12px 12px 13px;
      display: flex;
      flex-direction: column;
      gap: 4px;
    }

    .project-title {
      font-size: 0.95rem;
      font-weight: 600;
    }

    .project-desc {
      font-size: 0.78rem;
      color: var(--muted);
    }

    .project-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      margin-top: 6px;
    }

    .project-tag {
      font-size: 0.7rem;
      padding: 3px 8px;
      border-radius: 999px;
      border: 1px solid rgba(55, 65, 81, 0.9);
      color: var(--muted);
      background: #020617;
    }

    .contact-row {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      font-size: 0.85rem;
      color: var(--muted);
    }

    footer {
      margin-top: 18px;
      font-size: 0.75rem;
      color: #6b7280;
      text-align: center;
    }
  </style>
</head>
<body>
  <div class="page">
    <header>
      <div>
        <div class="logo-text">BUMINATA</div>
      </div>
      <div class="pill">
        <span class="dot"></span>
        Open for interesting data problems
      </div>
    </header>

    <main>
      <!-- HERO -->
      <section class="hero">
        <div class="hero-card">
          <div class="hero-role">Data Analyst & Data Science</div>
          <h1 class="hero-title">Building reliable, data-driven systems.</h1>
          <p class="hero-subtitle">
            I design and implement analytics pipelines, predictive models, and ML systems that turn noisy data into
            clear, actionable decisions.
          </p>

          <div class="hero-tags">
            <span class="hero-tag">Machine Learning</span>
            <span class="hero-tag">LLMs & NLP</span>
            <span class="hero-tag">MLOps & Automation</span>
            <span class="hero-tag">AWS & Cloud</span>
          </div>

          <div class="hero-footer">
            <div>
              <span style="color:#9ca3af;">Currently:</span>
              <span>Exploring applied ML, LLMs, and AI agents.</span>
            </div>
            <div class="hero-links">
              <a class="btn btn-primary" href="https://github.com/buminata" target="_blank" rel="noopener noreferrer">
                View GitHub
              </a>
              <a class="btn" href="https://www.linkedin.com/in/mohammad-satria-arya-buminata" target="_blank" rel="noopener noreferrer">
                LinkedIn
              </a>
            </div>
          </div>
        </div>

        <!-- SIDE CARD -->
        <aside class="side-card">
          <div class="avatar">B</div>
          <div class="side-name">Buminata</div>
          <div class="side-role">Data Analyst & Data Science Professional</div>

          <div class="side-meta">
            <span>📍 BSD, Tangerang Selatan</span>
            <span>📧 <a href="mailto:natalfiana@gmail.com">natalfiana@gmail.com</a></span>
          </div>

          <div class="badge-row">
            <span class="mini-badge">Python · SQL · R</span>
            <span class="mini-badge">ML · DL · NLP</span>
            <span class="mini-badge">Docker · Airflow · MLflow</span>
            <span class="mini-badge">AWS · Terraform</span>
          </div>

          <div class="stat-row">
            <span class="stat-chip">Data & ML Systems</span>
            <span class="stat-chip">Model Reliability</span>
          </div>
        </aside>
      </section>

      <!-- SKILLS -->
      <section>
        <div class="section-title">Tech Stack</div>
        <div class="section-grid">
          <div>
            <p style="font-size:0.85rem; color:#9ca3af; margin-bottom:6px;">Languages</p>
            <div class="pill-tag">Python (Pandas, PySpark, Scikit-learn)</div>
            <div class="pill-tag" style="margin-top:6px;">SQL · R</div>
          </div>
          <div>
            <p style="font-size:0.85rem; color:#9ca3af; margin-bottom:6px;">ML / AI</p>
            <div class="pill-tag">Machine Learning · Deep Learning</div>
            <div class="pill-tag" style="margin-top:6px;">NLP · Transformers · RAG</div>
          </div>
          <div>
            <p style="font-size:0.85rem; color:#9ca3af; margin-bottom:6px;">MLOps & Infra</p>
            <div class="pill-tag">Docker · Airflow · FastAPI · MLflow</div>
            <div class="pill-tag" style="margin-top:6px;">AWS (Lambda, EC2, ECS) · Terraform</div>
          </div>
          <div>
            <p style="font-size:0.85rem; color:#9ca3af; margin-bottom:6px;">Data</p>
            <div class="pill-tag">PostgreSQL · Elasticsearch</div>
          </div>
        </div>
      </section>

      <!-- PROJECTS -->
      <section>
        <div class="section-title">Selected Work</div>
        <div class="section-grid">
          <div class="project-card">
            <div class="project-title">Predictive Analytics Pipeline</div>
            <p class="project-desc">
              End-to-end ML workflow with experiment tracking, model evaluation, and deployment-ready structure.
            </p>
            <div class="project-tags">
              <span class="project-tag">Python</span>
              <span class="project-tag">Scikit-learn</span>
              <span class="project-tag">MLflow</span>
            </div>
          </div>

          <div class="project-card">
            <div class="project-title">NLP Text Classification</div>
            <p class="project-desc">
              Transformer-based text classifier wrapped in a FastAPI service for real-time inference.
            </p>
            <div class="project-tags">
              <span class="project-tag">Transformers</span>
              <span class="project-tag">NLP</span>
              <span class="project-tag">FastAPI</span>
            </div>
          </div>

          <div class="project-card">
            <div class="project-title">ETL & Data Engineering</div>
            <p class="project-desc">
              Automated batch pipeline for ingestion, cleaning, and aggregation using PySpark and Airflow.
            </p>
            <div class="project-tags">
              <span class="project-tag">PySpark</span>
              <span class="project-tag">Airflow</span>
              <span class="project-tag">ETL</span>
            </div>
          </div>

          <div class="project-card">
            <div class="project-title">Analytics Dashboards</div>
            <p class="project-desc">
              Clear, decision-focused dashboards turning raw metrics into business-friendly insights.
            </p>
            <div class="project-tags">
              <span class="project-tag">Python</span>
              <span class="project-tag">Data Viz</span>
              <span class="project-tag">SQL</span>
            </div>
          </div>
        </div>
      </section>

      <!-- CONTACT -->
      <section>
        <div class="section-title">Contact</div>
        <div class="contact-row">
          <span>📧 <a href="mailto:natalfiana@gmail.com">natalfiana@gmail.com</a></span>
          <span>📍 BSD, Tangerang Selatan</span>
          <span>🔗 <a href="https://github.com/buminata" target="_blank">GitHub</a></span>
          <span>🔗 <a href="https://www.linkedin.com/in/mohammad-satria-arya-buminata" target="_blank" rel="noopener noreferrer">LinkedIn</a></span>
        </div>
      </section>

      <footer>
        © 2025 Buminata — Built with GitHub Pages
      </footer>
    </main>
  </div>
</body>
</html>
