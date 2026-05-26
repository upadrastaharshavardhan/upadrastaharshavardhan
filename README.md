<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Upadrasta Harsha Vardhan — AI Engineer</title>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=Syne:wght@400;700;800&family=JetBrains+Mono:wght@300;400;500&display=swap" rel="stylesheet"/>
<style>
  :root {
    --black: #020408;
    --surface: #080d14;
    --surface2: #0d1520;
    --surface3: #111d2b;
    --cyan: #00d4ff;
    --cyan-dim: rgba(0,212,255,0.15);
    --cyan-glow: rgba(0,212,255,0.06);
    --gold: #f0a500;
    --gold-dim: rgba(240,165,0,0.12);
    --violet: #7c3aed;
    --violet-dim: rgba(124,58,237,0.12);
    --green: #10ffa0;
    --green-dim: rgba(16,255,160,0.1);
    --text: #e8edf5;
    --text2: #8899aa;
    --text3: #445566;
    --border: rgba(255,255,255,0.06);
    --border-bright: rgba(0,212,255,0.25);
  }
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  html { scroll-behavior: smooth; }
  body {
    background: var(--black);
    color: var(--text);
    font-family: 'Space Grotesk', sans-serif;
    overflow-x: hidden;
    line-height: 1.6;
  }

  /* ── NOISE OVERLAY ── */
  body::before {
    content: '';
    position: fixed; inset: 0; z-index: 0; pointer-events: none;
    background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.04'/%3E%3C/svg%3E");
    opacity: 0.4;
  }

  /* ── GRID BG ── */
  body::after {
    content: '';
    position: fixed; inset: 0; z-index: 0; pointer-events: none;
    background-image:
      linear-gradient(rgba(0,212,255,0.025) 1px, transparent 1px),
      linear-gradient(90deg, rgba(0,212,255,0.025) 1px, transparent 1px);
    background-size: 60px 60px;
  }

  main { position: relative; z-index: 1; max-width: 900px; margin: 0 auto; padding: 0 24px 80px; }

  /* ── HERO ── */
  .hero {
    padding: 80px 0 60px;
    position: relative;
  }
  .hero-eyebrow {
    font-family: 'JetBrains Mono', monospace;
    font-size: 12px;
    color: var(--cyan);
    letter-spacing: 0.2em;
    text-transform: uppercase;
    margin-bottom: 20px;
    display: flex;
    align-items: center;
    gap: 12px;
  }
  .hero-eyebrow::before {
    content: '';
    display: block;
    width: 32px; height: 1px;
    background: var(--cyan);
    opacity: 0.6;
  }
  .hero-name {
    font-family: 'Syne', sans-serif;
    font-size: clamp(42px, 8vw, 76px);
    font-weight: 800;
    line-height: 1;
    letter-spacing: -0.03em;
    color: #fff;
    margin-bottom: 8px;
  }
  .hero-name span {
    background: linear-gradient(135deg, var(--cyan) 0%, #7c3aed 60%, var(--gold) 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }
  .hero-role {
    font-size: 16px;
    color: var(--text2);
    margin-bottom: 32px;
    font-weight: 300;
    letter-spacing: 0.05em;
  }
  .hero-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-bottom: 48px;
  }
  .tag {
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    padding: 6px 14px;
    border-radius: 4px;
    border: 1px solid;
    letter-spacing: 0.1em;
    text-transform: uppercase;
  }
  .tag-cyan { border-color: rgba(0,212,255,0.3); color: var(--cyan); background: var(--cyan-glow); }
  .tag-gold { border-color: rgba(240,165,0,0.3); color: var(--gold); background: var(--gold-dim); }
  .tag-violet { border-color: rgba(124,58,237,0.3); color: #a78bfa; background: var(--violet-dim); }
  .tag-green { border-color: rgba(16,255,160,0.25); color: var(--green); background: var(--green-dim); }

  .hero-cta {
    display: flex;
    gap: 16px;
    flex-wrap: wrap;
  }
  .btn {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 12px 24px;
    border-radius: 6px;
    font-size: 13px;
    font-weight: 600;
    cursor: pointer;
    text-decoration: none;
    letter-spacing: 0.05em;
    transition: all 0.2s;
    border: 1px solid transparent;
  }
  .btn-primary {
    background: var(--cyan);
    color: #000;
    border-color: var(--cyan);
  }
  .btn-primary:hover { box-shadow: 0 0 28px rgba(0,212,255,0.4); transform: translateY(-1px); }
  .btn-ghost {
    background: transparent;
    color: var(--text);
    border-color: var(--border-bright);
  }
  .btn-ghost:hover { background: var(--cyan-dim); border-color: var(--cyan); color: var(--cyan); transform: translateY(-1px); }
  .btn-resume {
    background: transparent;
    color: var(--gold);
    border-color: rgba(240,165,0,0.35);
  }
  .btn-resume:hover { background: var(--gold-dim); border-color: var(--gold); box-shadow: 0 0 22px rgba(240,165,0,0.25); transform: translateY(-1px); }

  /* ── IMPACT METRICS ── */
  .metrics {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1px;
    background: var(--border);
    border: 1px solid var(--border);
    border-radius: 12px;
    overflow: hidden;
    margin-bottom: 80px;
  }
  .metric {
    background: var(--surface);
    padding: 28px 20px;
    text-align: center;
    position: relative;
    overflow: hidden;
    transition: background 0.3s;
  }
  .metric:hover { background: var(--surface2); }
  .metric::after {
    content: '';
    position: absolute;
    bottom: 0; left: 0; right: 0;
    height: 2px;
  }
  .metric:nth-child(1)::after { background: var(--cyan); }
  .metric:nth-child(2)::after { background: var(--gold); }
  .metric:nth-child(3)::after { background: #7c3aed; }
  .metric:nth-child(4)::after { background: var(--green); }
  .metric-num {
    font-family: 'Syne', sans-serif;
    font-size: 40px;
    font-weight: 800;
    line-height: 1;
    margin-bottom: 8px;
  }
  .metric:nth-child(1) .metric-num { color: var(--cyan); }
  .metric:nth-child(2) .metric-num { color: var(--gold); }
  .metric:nth-child(3) .metric-num { color: #a78bfa; }
  .metric:nth-child(4) .metric-num { color: var(--green); }
  .metric-label { font-size: 11px; color: var(--text2); text-transform: uppercase; letter-spacing: 0.12em; line-height: 1.4; }

  /* ── SECTION ── */
  .section { margin-bottom: 80px; }
  .section-header {
    display: flex;
    align-items: center;
    gap: 16px;
    margin-bottom: 32px;
  }
  .section-title {
    font-family: 'Syne', sans-serif;
    font-size: 22px;
    font-weight: 700;
    color: #fff;
  }
  .section-line {
    flex: 1; height: 1px;
    background: linear-gradient(90deg, var(--border-bright), transparent);
  }
  .section-num {
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    color: var(--cyan);
    opacity: 0.5;
    letter-spacing: 0.1em;
  }

  /* ── AI ZONE GRID ── */
  .ai-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 16px;
  }
  .ai-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 24px;
    position: relative;
    overflow: hidden;
    transition: all 0.3s;
    cursor: default;
  }
  .ai-card::before {
    content: '';
    position: absolute;
    top: -1px; left: -1px; right: -1px;
    height: 2px;
    border-radius: 10px 10px 0 0;
    opacity: 0;
    transition: opacity 0.3s;
  }
  .ai-card:hover::before { opacity: 1; }
  .ai-card:hover { background: var(--surface2); border-color: rgba(255,255,255,0.12); transform: translateY(-2px); }
  .ai-card-1::before { background: linear-gradient(90deg, var(--cyan), #7c3aed); }
  .ai-card-2::before { background: linear-gradient(90deg, var(--gold), #f87171); }
  .ai-card-3::before { background: linear-gradient(90deg, var(--green), var(--cyan)); }
  .ai-card-4::before { background: linear-gradient(90deg, #a78bfa, var(--gold)); }
  .ai-card-icon {
    font-size: 28px;
    margin-bottom: 12px;
    display: block;
  }
  .ai-card-title {
    font-size: 14px;
    font-weight: 600;
    color: #fff;
    margin-bottom: 6px;
    letter-spacing: 0.02em;
  }
  .ai-card-desc { font-size: 13px; color: var(--text2); line-height: 1.6; }

  /* ── PROJECTS ── */
  .projects { display: flex; flex-direction: column; gap: 20px; }
  .project-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 28px;
    display: grid;
    grid-template-columns: 1fr auto;
    gap: 16px;
    align-items: start;
    transition: all 0.3s;
    position: relative;
    overflow: hidden;
  }
  .project-card::before {
    content: '';
    position: absolute;
    left: 0; top: 0; bottom: 0;
    width: 3px;
  }
  .project-card:nth-child(1)::before { background: var(--cyan); }
  .project-card:nth-child(2)::before { background: var(--gold); }
  .project-card:nth-child(3)::before { background: #a78bfa; }
  .project-card:nth-child(4)::before { background: var(--green); }
  .project-card:hover { background: var(--surface2); border-color: rgba(255,255,255,0.1); transform: translateX(4px); }
  .project-header {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 10px;
  }
  .project-icon { font-size: 20px; }
  .project-name { font-size: 16px; font-weight: 600; color: #fff; }
  .project-desc { font-size: 13px; color: var(--text2); line-height: 1.7; margin-bottom: 14px; }
  .project-badges { display: flex; flex-wrap: wrap; gap: 8px; }
  .badge {
    font-family: 'JetBrains Mono', monospace;
    font-size: 10px;
    padding: 4px 10px;
    border-radius: 3px;
    border: 1px solid;
    text-transform: uppercase;
    letter-spacing: 0.08em;
  }
  .badge-cyan { border-color: rgba(0,212,255,0.25); color: var(--cyan); background: rgba(0,212,255,0.06); }
  .badge-gold { border-color: rgba(240,165,0,0.25); color: var(--gold); background: rgba(240,165,0,0.06); }
  .badge-violet { border-color: rgba(124,58,237,0.25); color: #a78bfa; background: rgba(124,58,237,0.06); }
  .badge-green { border-color: rgba(16,255,160,0.2); color: var(--green); background: rgba(16,255,160,0.05); }
  .project-stat {
    text-align: right;
    white-space: nowrap;
  }
  .stat-num {
    font-family: 'Syne', sans-serif;
    font-size: 28px;
    font-weight: 800;
    display: block;
    line-height: 1;
  }
  .project-card:nth-child(1) .stat-num { color: var(--cyan); }
  .project-card:nth-child(2) .stat-num { color: var(--gold); }
  .project-card:nth-child(3) .stat-num { color: #a78bfa; }
  .project-card:nth-child(4) .stat-num { color: var(--green); }
  .stat-label { font-size: 10px; color: var(--text3); text-transform: uppercase; letter-spacing: 0.1em; }

  /* ── TECH STACK ── */
  .tech-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
    gap: 10px;
  }
  .tech-item {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 14px 12px;
    text-align: center;
    font-size: 12px;
    color: var(--text2);
    font-family: 'JetBrains Mono', monospace;
    transition: all 0.2s;
    cursor: default;
  }
  .tech-item:hover { border-color: var(--border-bright); color: var(--cyan); background: var(--cyan-glow); transform: translateY(-2px); }
  .tech-item-icon { font-size: 22px; display: block; margin-bottom: 8px; }

  /* ── PRODUCTS ── */
  .products { display: grid; grid-template-columns: repeat(3, 1fr); gap: 16px; }
  .product-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 24px;
    text-align: center;
    transition: all 0.3s;
  }
  .product-card:hover { background: var(--surface2); border-color: rgba(255,255,255,0.1); transform: translateY(-3px); }
  .product-emoji { font-size: 36px; display: block; margin-bottom: 12px; }
  .product-name { font-weight: 700; font-size: 15px; color: #fff; margin-bottom: 6px; }
  .product-desc { font-size: 12px; color: var(--text2); line-height: 1.6; }

  /* ── CONNECT ── */
  .connect-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 12px;
  }
  .connect-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 20px 16px;
    text-align: center;
    text-decoration: none;
    transition: all 0.3s;
    display: block;
  }
  .connect-card:hover { transform: translateY(-3px); }
  .connect-card.email:hover { border-color: #f87171; background: rgba(248,113,113,0.08); }
  .connect-card.linkedin:hover { border-color: #0ea5e9; background: rgba(14,165,233,0.08); }
  .connect-card.github:hover { border-color: #e2e8f0; background: rgba(226,232,240,0.06); }
  .connect-card.portfolio:hover { border-color: var(--gold); background: var(--gold-dim); }
  .connect-icon { font-size: 26px; display: block; margin-bottom: 10px; }
  .connect-label { font-size: 11px; color: var(--text2); text-transform: uppercase; letter-spacing: 0.1em; font-family: 'JetBrains Mono', monospace; }

  /* ── QUOTE ── */
  .quote-block {
    border: 1px solid var(--border-bright);
    border-radius: 12px;
    padding: 36px 40px;
    background: var(--surface);
    position: relative;
    overflow: hidden;
    margin-bottom: 80px;
  }
  .quote-block::before {
    content: '"';
    position: absolute;
    top: -20px; left: 20px;
    font-family: 'Syne', sans-serif;
    font-size: 160px;
    font-weight: 800;
    color: var(--cyan);
    opacity: 0.04;
    line-height: 1;
    pointer-events: none;
  }
  .quote-text {
    font-family: 'Syne', sans-serif;
    font-size: 20px;
    font-weight: 700;
    color: #fff;
    line-height: 1.5;
    margin-bottom: 16px;
  }
  .quote-sub { font-size: 13px; color: var(--text2); font-family: 'JetBrains Mono', monospace; }

  /* ── TERMINAL STATUS ── */
  .terminal {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 10px;
    overflow: hidden;
    margin-bottom: 80px;
  }
  .terminal-bar {
    background: var(--surface2);
    padding: 12px 16px;
    display: flex;
    align-items: center;
    gap: 8px;
    border-bottom: 1px solid var(--border);
  }
  .dot { width: 10px; height: 10px; border-radius: 50%; }
  .dot-red { background: #f87171; }
  .dot-yellow { background: var(--gold); }
  .dot-green { background: var(--green); }
  .terminal-title { font-family: 'JetBrains Mono', monospace; font-size: 11px; color: var(--text2); margin-left: auto; }
  .terminal-body { padding: 20px 24px; }
  .terminal-line {
    font-family: 'JetBrains Mono', monospace;
    font-size: 13px;
    line-height: 2;
    color: var(--text2);
  }
  .terminal-line .prompt { color: var(--cyan); margin-right: 8px; }
  .terminal-line .cmd { color: var(--text); }
  .terminal-line .out { color: var(--text2); display: block; padding-left: 24px; margin-bottom: 4px; }
  .terminal-line .hi { color: var(--green); }
  .terminal-line .wa { color: var(--gold); }
  .terminal-line .inf { color: #a78bfa; }
  .cursor {
    display: inline-block;
    width: 8px; height: 14px;
    background: var(--cyan);
    animation: blink 1s step-end infinite;
    vertical-align: middle;
    margin-left: 4px;
  }
  @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }

  /* ── FOCUS SECTION ── */
  .focus-list {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 12px;
  }
  .focus-item {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 18px 20px;
    display: flex;
    align-items: center;
    gap: 14px;
    font-size: 14px;
    color: var(--text2);
    transition: all 0.2s;
  }
  .focus-item:hover { border-color: rgba(255,255,255,0.1); color: var(--text); background: var(--surface2); }
  .focus-dot { width: 8px; height: 8px; border-radius: 50%; flex-shrink: 0; }

  /* ── FOOTER ── */
  .footer {
    border-top: 1px solid var(--border);
    padding-top: 40px;
    text-align: center;
  }
  .footer-brand {
    font-family: 'Syne', sans-serif;
    font-size: 13px;
    font-weight: 700;
    color: var(--text3);
    letter-spacing: 0.2em;
    text-transform: uppercase;
  }
  .footer-brand span { color: var(--cyan); }

  /* ── ANIMATIONS ── */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }
  .hero { animation: fadeUp 0.7s ease both; }
  .metrics { animation: fadeUp 0.7s 0.1s ease both; }
  .section { animation: fadeUp 0.7s 0.15s ease both; }

  /* ── RESPONSIVE ── */
  @media (max-width: 640px) {
    .metrics { grid-template-columns: repeat(2, 1fr); }
    .ai-grid { grid-template-columns: 1fr; }
    .products { grid-template-columns: 1fr; }
    .connect-grid { grid-template-columns: repeat(2, 1fr); }
    .focus-list { grid-template-columns: 1fr; }
    .project-card { grid-template-columns: 1fr; }
  }
</style>
</head>
<body>
<main>

  <!-- ══ HERO ══ -->
  <section class="hero">
    <div class="hero-eyebrow">AI Engineer · GenAI Builder · Automation Architect</div>
    <h1 class="hero-name">Upadrasta<br><span>Harsha Vardhan</span></h1>
    <p class="hero-role">Building AI systems where intelligence becomes part of engineering.</p>
    <div class="hero-tags">
      <span class="tag tag-cyan">Azure OpenAI</span>
      <span class="tag tag-violet">Copilot Studio</span>
      <span class="tag tag-gold">AI Agents</span>
      <span class="tag tag-green">RAG Systems</span>
      <span class="tag tag-cyan">DevOps CI/CD</span>
      <span class="tag tag-violet">LLMs</span>
      <span class="tag tag-gold">QA Automation</span>
    </div>
    <div class="hero-cta">
      <a href="mailto:upadrastaharsha09@gmail.com" class="btn btn-primary">📩 Get in touch</a>
      <a href="https://upadrastaharshavardhan.github.io/Harshavardhan/index.html" class="btn btn-ghost">View Portfolio ↗</a>
      <a href="https://github.com/upadrastaharshavardhan/upadrastaharshavardhan/blob/main/Harsha%20Vardhan%20Upadrasta%20Resume%202026.pdf" class="btn btn-resume" target="_blank" rel="noopener">⬇ Resume 2026</a>
    </div>
  </section>

  <!-- ══ METRICS ══ -->
  <div class="metrics">
    <div class="metric">
      <div class="metric-num">60%</div>
      <div class="metric-label">Reduction in manual test effort</div>
    </div>
    <div class="metric">
      <div class="metric-num">55%</div>
      <div class="metric-label">Increase in regression coverage</div>
    </div>
    <div class="metric">
      <div class="metric-num">45%</div>
      <div class="metric-label">Faster release validation</div>
    </div>
    <div class="metric">
      <div class="metric-num">30%</div>
      <div class="metric-label">Drop in production defects</div>
    </div>
  </div>

  <!-- ══ AI ENGINEERING ZONE ══ -->
  <section class="section">
    <div class="section-header">
      <span class="section-num">01</span>
      <h2 class="section-title">AI Engineering Zone</h2>
      <div class="section-line"></div>
    </div>
    <div class="ai-grid">
      <div class="ai-card ai-card-1">
        <span class="ai-card-icon">🧠</span>
        <div class="ai-card-title">Large Language Models</div>
        <div class="ai-card-desc">GPT · Claude · Gemini — prompt engineering, evaluation, fine-tuning pipelines for production QA automation.</div>
      </div>
      <div class="ai-card ai-card-2">
        <span class="ai-card-icon">🔗</span>
        <div class="ai-card-title">RAG Systems</div>
        <div class="ai-card-desc">Context-aware AI with retrieval-augmented generation — documentation ingestion, vector stores, semantic search.</div>
      </div>
      <div class="ai-card ai-card-3">
        <span class="ai-card-icon">🤖</span>
        <div class="ai-card-title">AI Agents</div>
        <div class="ai-card-desc">Copilot Studio + Azure OpenAI multi-agent architectures — agentic task orchestration at scale.</div>
      </div>
      <div class="ai-card ai-card-4">
        <span class="ai-card-icon">⚡</span>
        <div class="ai-card-title">AI-Powered Pipelines</div>
        <div class="ai-card-desc">AI-generated test suites integrated into DevOps CI/CD — self-healing automation that ships quality faster.</div>
      </div>
    </div>
  </section>

  <!-- ══ PROJECTS ══ -->
  <section class="section">
    <div class="section-header">
      <span class="section-num">02</span>
      <h2 class="section-title">Real-World AI Projects</h2>
      <div class="section-line"></div>
    </div>
    <div class="projects">
      <div class="project-card">
        <div>
          <div class="project-header">
            <span class="project-icon">🧪</span>
            <span class="project-name">AI Test Case Generator</span>
          </div>
          <p class="project-desc">Converts plain English requirements into PyTest / BDD test suites. Integrated deep inside DevOps pipelines — the automation writes itself while your team ships features.</p>
          <div class="project-badges">
            <span class="badge badge-cyan">Azure OpenAI</span>
            <span class="badge badge-gold">PyTest / BDD</span>
            <span class="badge badge-violet">DevOps</span>
          </div>
        </div>
        <div class="project-stat">
          <span class="stat-num">60%</span>
          <span class="stat-label">Faster</span>
        </div>
      </div>
      <div class="project-card">
        <div>
          <div class="project-header">
            <span class="project-icon">📊</span>
            <span class="project-name">MongoDB AI Query Agent</span>
          </div>
          <p class="project-desc">Natural language to optimized MongoDB queries — non-technical users interact with databases through conversation. Built-in query optimization and execution planning.</p>
          <div class="project-badges">
            <span class="badge badge-gold">NLP</span>
            <span class="badge badge-cyan">MongoDB</span>
            <span class="badge badge-green">RAG</span>
          </div>
        </div>
        <div class="project-stat">
          <span class="stat-num">0→1</span>
          <span class="stat-label">DB Access</span>
        </div>
      </div>
      <div class="project-card">
        <div>
          <div class="project-header">
            <span class="project-icon">🌐</span>
            <span class="project-name">API Creation Agent</span>
          </div>
          <p class="project-desc">Generate fully-functional APIs from plain English specifications. Security policies, rate limiting, and traffic rules included. What took days now takes hours.</p>
          <div class="project-badges">
            <span class="badge badge-violet">Agents</span>
            <span class="badge badge-cyan">FastAPI</span>
            <span class="badge badge-gold">Security</span>
          </div>
        </div>
        <div class="project-stat">
          <span class="stat-num">days→hrs</span>
          <span class="stat-label">Delivery</span>
        </div>
      </div>
      <div class="project-card">
        <div>
          <div class="project-header">
            <span class="project-icon">📄</span>
            <span class="project-name">Docs → Automation Agent</span>
          </div>
          <p class="project-desc">RAG-powered system that reads documentation and continuously generates test cases and scripts. Stays in sync as docs evolve — tests that write themselves.</p>
          <div class="project-badges">
            <span class="badge badge-green">RAG</span>
            <span class="badge badge-violet">Automation</span>
            <span class="badge badge-cyan">Continuous</span>
          </div>
        </div>
        <div class="project-stat">
          <span class="stat-num">∞</span>
          <span class="stat-label">Auto-sync</span>
        </div>
      </div>
    </div>
  </section>

  <!-- ══ TERMINAL ══ -->
  <div class="terminal">
    <div class="terminal-bar">
      <div class="dot dot-red"></div>
      <div class="dot dot-yellow"></div>
      <div class="dot dot-green"></div>
      <span class="terminal-title">harsha@ai-engineering ~ current-status</span>
    </div>
    <div class="terminal-body">
      <div class="terminal-line">
        <span class="prompt">❯</span><span class="cmd">whoami</span>
        <span class="out"><span class="hi">Upadrasta Harsha Vardhan</span> — Assistant Manager, AI Automation QA Engineer</span>
      </div>
      <div class="terminal-line">
        <span class="prompt">❯</span><span class="cmd">cat current_focus.txt</span>
        <span class="out"><span class="inf">→</span> Advanced Agentic AI Systems architecture</span>
        <span class="out"><span class="inf">→</span> AI-native QA frameworks at enterprise scale</span>
        <span class="out"><span class="inf">→</span> AI + Cybersecurity convergence</span>
      </div>
      <div class="terminal-line">
        <span class="prompt">❯</span><span class="cmd">git log --oneline -3</span>
        <span class="out"><span class="wa">f3a91bc</span> feat: deploy multi-agent test orchestration layer</span>
        <span class="out"><span class="wa">9e2d487</span> feat: add RAG pipeline to docs-to-automation agent</span>
        <span class="out"><span class="wa">2c84f1a</span> chore: reduce production defect rate by 30%</span>
      </div>
      <div class="terminal-line">
        <span class="prompt">❯</span><span class="cmd">status<span class="cursor"></span></span>
      </div>
    </div>
  </div>

  <!-- ══ TECH STACK ══ -->
  <section class="section">
    <div class="section-header">
      <span class="section-num">03</span>
      <h2 class="section-title">Tech Stack</h2>
      <div class="section-line"></div>
    </div>
    <div class="tech-grid">
      <div class="tech-item"><span class="tech-item-icon">🐍</span>Python</div>
      <div class="tech-item"><span class="tech-item-icon">☁️</span>Azure OpenAI</div>
      <div class="tech-item"><span class="tech-item-icon">🤖</span>Copilot Studio</div>
      <div class="tech-item"><span class="tech-item-icon">⚛️</span>React</div>
      <div class="tech-item"><span class="tech-item-icon">🟩</span>Node.js</div>
      <div class="tech-item"><span class="tech-item-icon">🚀</span>FastAPI</div>
      <div class="tech-item"><span class="tech-item-icon">🍃</span>MongoDB</div>
      <div class="tech-item"><span class="tech-item-icon">🐳</span>Docker</div>
      <div class="tech-item"><span class="tech-item-icon">⚙️</span>GitHub Actions</div>
      <div class="tech-item"><span class="tech-item-icon">☁️</span>AWS</div>
      <div class="tech-item"><span class="tech-item-icon">🔵</span>Azure</div>
      <div class="tech-item"><span class="tech-item-icon">🔗</span>LangChain</div>
    </div>
  </section>

  <!-- ══ PRODUCTS ══ -->
  <section class="section">
    <div class="section-header">
      <span class="section-num">04</span>
      <h2 class="section-title">Products Built</h2>
      <div class="section-line"></div>
    </div>
    <div class="products">
      <div class="product-card">
        <span class="product-emoji">🚀</span>
        <div class="product-name">Insight Trove</div>
        <div class="product-desc">AI-powered learning platform. Personalized intelligence meets structured knowledge.</div>
      </div>
      <div class="product-card">
        <span class="product-emoji">💍</span>
        <div class="product-name">Rutvik</div>
        <div class="product-desc">Smart Purohit booking system. Digitizing sacred traditions with intelligent scheduling.</div>
      </div>
      <div class="product-card">
        <span class="product-emoji">🎓</span>
        <div class="product-name">Vidya4U</div>
        <div class="product-desc">Career + learning ecosystem. End-to-end platform bridging education to employment.</div>
      </div>
    </div>
  </section>

  <!-- ══ CURRENT FOCUS ══ -->
  <section class="section">
    <div class="section-header">
      <span class="section-num">05</span>
      <h2 class="section-title">Currently Focused On</h2>
      <div class="section-line"></div>
    </div>
    <div class="focus-list">
      <div class="focus-item">
        <div class="focus-dot" style="background:var(--cyan)"></div>
        Advanced Agentic AI Systems
      </div>
      <div class="focus-item">
        <div class="focus-dot" style="background:var(--gold)"></div>
        AI System Design & Architecture
      </div>
      <div class="focus-item">
        <div class="focus-dot" style="background:#a78bfa"></div>
        Scalable Automation Frameworks
      </div>
      <div class="focus-item">
        <div class="focus-dot" style="background:var(--green)"></div>
        AI + Cybersecurity Convergence
      </div>
    </div>
  </section>

  <!-- ══ QUOTE ══ -->
  <div class="quote-block">
    <div class="quote-text">"I don't just use AI tools. I build systems where AI becomes part of engineering itself."</div>
    <div class="quote-sub">— Upadrasta Harsha Vardhan · AI Engineer · GenAI Builder</div>
  </div>

  <!-- ══ CONNECT ══ -->
  <section class="section">
    <div class="section-header">
      <span class="section-num">06</span>
      <h2 class="section-title">Connect</h2>
      <div class="section-line"></div>
    </div>
    <div class="connect-grid">
      <a href="mailto:upadrastaharsha09@gmail.com" class="connect-card email">
        <span class="connect-icon">📧</span>
        <span class="connect-label">Email</span>
      </a>
      <a href="https://www.linkedin.com/in/harsha-upadrasta-a33a461a2" class="connect-card linkedin">
        <span class="connect-icon">💼</span>
        <span class="connect-label">LinkedIn</span>
      </a>
      <a href="https://github.com/upadrastaharshavardhan" class="connect-card github">
        <span class="connect-icon">🐙</span>
        <span class="connect-label">GitHub</span>
      </a>
      <a href="https://upadrastaharshavardhan.github.io/Harshavardhan/index.html" class="connect-card portfolio">
        <span class="connect-icon">🌐</span>
        <span class="connect-label">Portfolio</span>
      </a>
    </div>
  </section>

  <!-- ══ FOOTER ══ -->
  <footer class="footer">
    <div class="footer-brand">🔥 <span>AI</span> · Automation · <span>Innovation</span> 🔥</div>
  </footer>

</main>
</body>
</html>
