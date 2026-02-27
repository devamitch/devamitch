<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Amit Chakraborty — GitHub Profile</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;700&family=Inter:wght@400;500;600;700&display=swap');

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    background: #0D1117;
    color: #E6EDF3;
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
    line-height: 1.7;
    padding: 0;
  }

  .container {
    max-width: 900px;
    margin: 0 auto;
    padding: 40px 32px;
  }

  /* ─── Header ─── */
  .header {
    text-align: center;
    padding: 48px 0 24px;
  }

  .header h1 {
    font-family: 'JetBrains Mono', monospace;
    font-size: 36px;
    font-weight: 700;
    color: #C9A84C;
    letter-spacing: 1px;
    margin-bottom: 4px;
  }

  .header .subtitle {
    font-family: 'JetBrains Mono', monospace;
    font-size: 16px;
    color: #8B949E;
    margin-bottom: 24px;
  }

  .terminal-box {
    background: #161B22;
    border: 1px solid #30363D;
    border-radius: 8px;
    padding: 16px 24px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 14px;
    color: #E6EDF3;
    display: inline-block;
    margin: 16px 0 24px;
    text-align: center;
    line-height: 1.8;
  }

  .terminal-box .gold { color: #C9A84C; }

  /* ─── Badges ─── */
  .badges {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    justify-content: center;
    margin: 20px 0;
  }

  .badge {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 8px 16px;
    border-radius: 6px;
    font-size: 13px;
    font-weight: 600;
    text-decoration: none;
    color: #fff;
    transition: transform 0.2s, box-shadow 0.2s;
  }

  .badge:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(0,0,0,0.4);
  }

  .badge svg { width: 16px; height: 16px; fill: currentColor; }

  .badge-portfolio { background: #C9A84C; }
  .badge-linkedin { background: #0A66C2; }
  .badge-medium { background: #292929; }
  .badge-x { background: #1a1a1a; border: 1px solid #333; }
  .badge-email { background: #EA4335; }
  .badge-github { background: #333; }

  .quote {
    font-style: italic;
    color: #8B949E;
    font-size: 15px;
    margin: 20px 0 8px;
    text-align: center;
  }

  /* ─── Sections ─── */
  hr {
    border: none;
    border-top: 1px solid #21262D;
    margin: 32px 0;
  }

  h2 {
    font-size: 22px;
    color: #E6EDF3;
    margin-bottom: 16px;
    display: flex;
    align-items: center;
    gap: 8px;
  }

  h3 {
    font-size: 17px;
    color: #C9A84C;
    margin: 20px 0 8px;
  }

  p { margin-bottom: 12px; color: #C9D1D9; font-size: 15px; }

  strong { color: #E6EDF3; }

  /* ─── Code Block ─── */
  .code-block {
    background: #161B22;
    border: 1px solid #30363D;
    border-radius: 8px;
    padding: 20px 24px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 13px;
    line-height: 1.8;
    overflow-x: auto;
    margin: 16px 0;
  }

  .code-block .keyword { color: #FF7B72; }
  .code-block .const { color: #79C0FF; }
  .code-block .string { color: #A5D6FF; }
  .code-block .prop { color: #D2A8FF; }
  .code-block .comment { color: #8B949E; }
  .code-block .bracket { color: #E6EDF3; }
  .code-block .gold { color: #C9A84C; }

  /* ─── Stats Grid ─── */
  .stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 12px;
    margin: 20px 0;
  }

  .stat-card {
    background: #161B22;
    border: 1px solid #30363D;
    border-radius: 10px;
    padding: 20px;
    text-align: center;
    transition: border-color 0.3s, transform 0.2s;
  }

  .stat-card:hover {
    border-color: #C9A84C;
    transform: translateY(-2px);
  }

  .stat-card .value {
    font-family: 'JetBrains Mono', monospace;
    font-size: 28px;
    font-weight: 700;
    color: #C9A84C;
  }

  .stat-card .label {
    font-size: 12px;
    color: #8B949E;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-top: 4px;
  }

  /* ─── Experience Cards ─── */
  .exp-card {
    background: #161B22;
    border: 1px solid #30363D;
    border-radius: 12px;
    padding: 24px;
    margin: 16px 0;
    border-left: 3px solid #C9A84C;
  }

  .exp-card .role {
    font-size: 17px;
    font-weight: 700;
    color: #E6EDF3;
  }

  .exp-card .company {
    color: #C9A84C;
    font-weight: 600;
  }

  .exp-card .meta {
    font-size: 13px;
    color: #8B949E;
    margin: 4px 0 12px;
  }

  .exp-card ul {
    padding-left: 20px;
    margin: 8px 0;
  }

  .exp-card li {
    font-size: 14px;
    color: #C9D1D9;
    margin-bottom: 6px;
    line-height: 1.6;
  }

  .deliverable-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 8px;
    margin: 12px 0;
  }

  .deliverable {
    background: #0D1117;
    border: 1px solid #30363D;
    border-radius: 8px;
    padding: 12px 16px;
  }

  .deliverable .d-label {
    font-size: 12px;
    font-weight: 700;
    color: #C9A84C;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }

  .deliverable .d-detail {
    font-size: 13px;
    color: #8B949E;
    margin-top: 4px;
  }

  /* ─── Tech Tags ─── */
  .tech-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
    margin: 12px 0;
  }

  .tech-tag {
    background: rgba(201, 168, 76, 0.1);
    border: 1px solid rgba(201, 168, 76, 0.25);
    color: #C9A84C;
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    padding: 4px 10px;
    border-radius: 20px;
  }

  /* ─── Project Cards ─── */
  .projects-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
    margin: 16px 0;
  }

  .project-card {
    background: #161B22;
    border: 1px solid #30363D;
    border-radius: 10px;
    padding: 20px;
    transition: border-color 0.3s, transform 0.2s;
  }

  .project-card:hover {
    border-color: #C9A84C;
    transform: translateY(-2px);
  }

  .project-card .p-badge {
    font-size: 10px;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 1px;
    padding: 3px 8px;
    border-radius: 4px;
    display: inline-block;
    margin-bottom: 8px;
  }

  .project-card .p-name {
    font-size: 16px;
    font-weight: 700;
    color: #E6EDF3;
    margin-bottom: 4px;
  }

  .project-card .p-desc {
    font-size: 13px;
    color: #8B949E;
    margin-bottom: 10px;
    line-height: 1.5;
  }

  .project-card .p-links a {
    font-size: 12px;
    color: #58A6FF;
    text-decoration: none;
    margin-right: 12px;
  }

  .project-card .p-links a:hover { text-decoration: underline; }

  /* ─── Tech Arsenal Section ─── */
  .arsenal-section {
    margin: 16px 0;
  }

  .arsenal-category {
    margin-bottom: 16px;
  }

  .arsenal-category h4 {
    font-size: 13px;
    color: #8B949E;
    text-transform: uppercase;
    letter-spacing: 1.5px;
    margin-bottom: 10px;
    font-weight: 600;
  }

  .arsenal-badges {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }

  .a-badge {
    display: inline-flex;
    align-items: center;
    gap: 5px;
    padding: 5px 12px;
    border-radius: 5px;
    font-size: 12px;
    font-weight: 500;
    color: #fff;
  }

  .a-badge img { height: 14px; }

  /* ─── GitHub Stats ─── */
  .github-stats {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
    justify-content: center;
    margin: 20px 0;
  }

  .github-stats img {
    border-radius: 8px;
    max-width: 100%;
  }

  /* ─── Testimonials ─── */
  .testimonial {
    background: #161B22;
    border: 1px solid #30363D;
    border-radius: 10px;
    padding: 20px 24px;
    margin: 12px 0;
    position: relative;
  }

  .testimonial::before {
    content: '"';
    font-size: 48px;
    color: #C9A84C;
    font-family: Georgia, serif;
    position: absolute;
    top: 8px;
    left: 16px;
    opacity: 0.4;
  }

  .testimonial .t-text {
    font-size: 14px;
    color: #C9D1D9;
    font-style: italic;
    padding-left: 24px;
    line-height: 1.7;
  }

  .testimonial .t-author {
    font-size: 13px;
    color: #C9A84C;
    font-weight: 600;
    margin-top: 8px;
    padding-left: 24px;
  }

  .testimonial .t-role {
    font-size: 12px;
    color: #8B949E;
    padding-left: 24px;
  }

  /* ─── Timeline ─── */
  .timeline {
    position: relative;
    padding-left: 32px;
    margin: 20px 0;
  }

  .timeline::before {
    content: '';
    position: absolute;
    left: 8px;
    top: 0;
    bottom: 0;
    width: 2px;
    background: linear-gradient(180deg, #C9A84C, #F5C842, #DAA520, #B8860B, #C9A84C, #F5C842);
  }

  .timeline-item {
    position: relative;
    margin-bottom: 24px;
  }

  .timeline-item::before {
    content: '';
    position: absolute;
    left: -28px;
    top: 6px;
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background: #C9A84C;
    border: 2px solid #0D1117;
  }

  .timeline-item .t-year {
    font-family: 'JetBrains Mono', monospace;
    font-size: 14px;
    color: #C9A84C;
    font-weight: 700;
  }

  .timeline-item .t-title {
    font-size: 16px;
    font-weight: 700;
    color: #E6EDF3;
    margin: 2px 0;
  }

  .timeline-item .t-desc {
    font-size: 13px;
    color: #8B949E;
    line-height: 1.5;
  }

  /* ─── Services Table ─── */
  .services-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 12px;
    margin: 20px 0;
  }

  .service-card {
    background: #161B22;
    border: 1px solid #30363D;
    border-radius: 10px;
    padding: 24px;
    text-align: center;
    transition: border-color 0.3s;
  }

  .service-card:hover { border-color: #C9A84C; }

  .service-card .s-icon { font-size: 32px; margin-bottom: 12px; }
  .service-card .s-title { font-size: 16px; font-weight: 700; color: #E6EDF3; margin-bottom: 4px; }
  .service-card .s-desc { font-size: 13px; color: #8B949E; margin-bottom: 8px; line-height: 1.5; }
  .service-card .s-price { font-family: 'JetBrains Mono', monospace; font-size: 13px; color: #C9A84C; font-weight: 700; }

  /* ─── CTA Box ─── */
  .cta-box {
    background: linear-gradient(135deg, rgba(201,168,76,0.08), rgba(201,168,76,0.02));
    border: 1px solid rgba(201,168,76,0.3);
    border-radius: 12px;
    padding: 32px;
    text-align: center;
    margin: 24px 0;
  }

  .cta-box p {
    color: #E6EDF3;
    font-size: 16px;
    margin-bottom: 16px;
  }

  .cta-buttons {
    display: flex;
    gap: 12px;
    justify-content: center;
    flex-wrap: wrap;
  }

  .cta-btn {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 10px 24px;
    border-radius: 8px;
    font-size: 14px;
    font-weight: 600;
    text-decoration: none;
    color: #fff;
    transition: transform 0.2s, box-shadow 0.2s;
  }

  .cta-btn:hover { transform: translateY(-2px); box-shadow: 0 4px 16px rgba(0,0,0,0.4); }

  .cta-btn-gold { background: #C9A84C; color: #000; }
  .cta-btn-blue { background: #0A66C2; }
  .cta-btn-dark { background: #333; }

  /* ─── Blog Cards ─── */
  .blog-list { margin: 16px 0; }

  .blog-item {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 12px 16px;
    background: #161B22;
    border: 1px solid #30363D;
    border-radius: 8px;
    margin-bottom: 8px;
    text-decoration: none;
    transition: border-color 0.2s;
  }

  .blog-item:hover { border-color: #C9A84C; }

  .blog-item .b-emoji { font-size: 24px; }
  .blog-item .b-title { font-size: 14px; color: #E6EDF3; font-weight: 500; }
  .blog-item .b-cat { font-size: 11px; color: #C9A84C; }

  /* ─── Collab Box ─── */
  .collab-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
    margin: 16px 0;
  }

  .collab-item {
    background: #161B22;
    border: 1px solid #30363D;
    border-radius: 8px;
    padding: 16px;
  }

  .collab-item .c-icon { font-size: 20px; margin-bottom: 6px; }
  .collab-item .c-title { font-size: 14px; font-weight: 700; color: #E6EDF3; margin-bottom: 4px; }
  .collab-item .c-desc { font-size: 12px; color: #8B949E; line-height: 1.5; }

  /* ─── Education ─── */
  .edu-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
    margin: 16px 0;
  }

  .edu-card {
    background: #161B22;
    border: 1px solid #30363D;
    border-radius: 8px;
    padding: 16px;
  }

  .edu-card .e-degree { font-size: 15px; font-weight: 700; color: #E6EDF3; }
  .edu-card .e-school { font-size: 13px; color: #8B949E; }
  .edu-card .e-score { font-family: 'JetBrains Mono', monospace; font-size: 14px; color: #C9A84C; margin-top: 4px; }
  .edu-card .e-year { font-size: 12px; color: #8B949E; }

  .cert-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
    margin: 12px 0;
  }

  .cert-tag {
    background: rgba(88, 166, 255, 0.1);
    border: 1px solid rgba(88, 166, 255, 0.25);
    color: #58A6FF;
    font-size: 12px;
    padding: 4px 12px;
    border-radius: 20px;
  }

  .profile-views {
    text-align: center;
    margin-top: 32px;
    padding: 16px;
    font-size: 13px;
    color: #8B949E;
  }

  .footer-line {
    text-align: center;
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    color: #30363D;
    margin-top: 32px;
    padding: 16px;
  }

  @media (max-width: 640px) {
    .projects-grid, .services-grid, .collab-grid, .edu-grid, .deliverable-grid {
      grid-template-columns: 1fr;
    }
    .stats-grid { grid-template-columns: repeat(2, 1fr); }
  }
</style>
</head>
<body>

<div class="container">

  <!-- ═══ HEADER ═══ -->
  <div class="header">
    <h1>Amit Chakraborty</h1>
    <div class="subtitle">Principal Architect &nbsp;·&nbsp; Founding Engineer</div>

    <div class="terminal-box">
      <span class="gold">╔══════════════════════════════════════════════════════════╗</span><br/>
      <span class="gold">║</span>&nbsp; 8 Years &nbsp;·&nbsp; 18+ Apps Shipped &nbsp;·&nbsp; Zero Outsourced Decisions &nbsp;<span class="gold">║</span><br/>
      <span class="gold">║</span>&nbsp; I architect systems that outlast the hype. &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="gold">║</span><br/>
      <span class="gold">╚══════════════════════════════════════════════════════════╝</span>
    </div>

    <div class="badges">
      <a class="badge badge-portfolio" href="https://devamit.co.in">🌐 devamit.co.in</a>
      <a class="badge badge-linkedin" href="https://linkedin.com/in/devamitch">💼 LinkedIn</a>
      <a class="badge badge-medium" href="https://devamitch.medium.com">✍️ Medium</a>
      <a class="badge badge-x" href="https://x.com/devamitch">𝕏 @devamitch</a>
      <a class="badge badge-email" href="mailto:amit98ch@gmail.com">📧 Email</a>
      <a class="badge badge-github" href="https://github.com/devamitch">⚡ GitHub</a>
    </div>

    <div class="quote">"Before AI could write a line of code, I was building production systems."</div>
  </div>

  <hr/>

  <!-- ═══ WHO AM I ═══ -->
  <h2>🧬 Who Am I</h2>
  <p>I'm a <strong>Principal Architect & Founding Engineer</strong> from Kolkata, India — building production systems since 2017.</p>
  <p>I don't just write code. I build <strong>entire technical universes from nothing</strong> — game engines, AI pipelines, computer vision systems, blockchain architectures, and the teams that run them. My work spans <strong>HealthTech, FinTech, Web3, GovTech, and Gaming</strong>.</p>

  <div class="code-block">
    <span class="keyword">const</span> <span class="const">amit</span> <span class="bracket">= {</span><br/>
    &nbsp;&nbsp;<span class="prop">location</span>: <span class="string">"Kolkata, India"</span>,<br/>
    &nbsp;&nbsp;<span class="prop">timezone</span>: <span class="string">"IST (UTC+5:30)"</span>,<br/>
    &nbsp;&nbsp;<span class="prop">available</span>: <span class="string">"Open for high-impact collaborations & contract roles"</span>,<br/>
    &nbsp;&nbsp;<span class="prop">experience</span>: <span class="string">"8+ years"</span>,<br/>
    &nbsp;&nbsp;<span class="prop">shipped</span>: <span class="string">"18+ production applications"</span>,<br/>
    &nbsp;&nbsp;<span class="prop">philosophy</span>: <span class="string">"Every system I architect ships to production."</span>,<br/>
    <br/>
    &nbsp;&nbsp;<span class="prop">currently</span>: <span class="bracket">{</span><br/>
    &nbsp;&nbsp;&nbsp;&nbsp;<span class="prop">building</span>: <span class="string">"SaaS products & developer tools"</span>,<br/>
    &nbsp;&nbsp;&nbsp;&nbsp;<span class="prop">learning</span>: [<span class="string">"Rust"</span>, <span class="string">"Anchor Framework"</span>, <span class="string">"Solana on-chain"</span>],<br/>
    &nbsp;&nbsp;&nbsp;&nbsp;<span class="prop">writing</span>: <span class="string">"Technical articles on Medium"</span>,<br/>
    &nbsp;&nbsp;&nbsp;&nbsp;<span class="prop">mentoring</span>: <span class="string">"Junior → Senior engineers"</span>,<br/>
    &nbsp;&nbsp;<span class="bracket">}</span>,<br/>
    <span class="bracket">};</span>
  </div>

  <hr/>

  <!-- ═══ STATS ═══ -->
  <h2>⚡ The Numbers</h2>
  <div class="stats-grid">
    <div class="stat-card"><div class="value">8+</div><div class="label">Years in Production</div></div>
    <div class="stat-card"><div class="value">18+</div><div class="label">Apps Shipped</div></div>
    <div class="stat-card"><div class="value">21</div><div class="label">Largest Team Led</div></div>
    <div class="stat-card"><div class="value">15+</div><div class="label">0-to-1 Builds</div></div>
    <div class="stat-card"><div class="value">13+</div><div class="label">Gov Projects Secured</div></div>
    <div class="stat-card"><div class="value">55+</div><div class="label">Open Source Repos</div></div>
  </div>

  <hr/>

  <!-- ═══ EXPERIENCE ═══ -->
  <h2>🏗️ Production Architecture</h2>

  <!-- Synapsis -->
  <div class="exp-card">
    <div class="role">Principal Mobile Architect & Technical Lead</div>
    <div class="company">Synapsis Medical Technologies — Founding Engineer</div>
    <div class="meta">Edmonton, Canada (Remote) · Jan 2025 – Feb 2026 · HealthTech AI Startup</div>
    <p style="font-size:14px; color:#8B949E;">Retained to execute the complete <strong style="color:#C9A84C;">0-to-1 technical build</strong> of a HealthTech AI startup. Built the entire engineering foundation from absolute zero.</p>

    <div class="deliverable-grid">
      <div class="deliverable">
        <div class="d-label">🎮 Proprietary Game Engine</div>
        <div class="d-detail">Built from scratch — C++/Swift/Kotlin bridgeless modules, zero external deps. LLM-based dynamic task generation + XP progression.</div>
      </div>
      <div class="deliverable">
        <div class="d-label">🤖 Aura AI</div>
        <div class="d-detail">Custom prompt-engineered AI assistant for clinical workflows, patient engagement & automated triage.</div>
      </div>
      <div class="deliverable">
        <div class="d-label">🧠 RAG Pipelines</div>
        <div class="d-detail">HIPAA-compliant retrieval-augmented generation for medical data. 99.9% uptime.</div>
      </div>
      <div class="deliverable">
        <div class="d-label">👁️ Computer Vision</div>
        <div class="d-detail">MediaPipe for real-time retina analysis & luminance tracking on consumer mobile hardware.</div>
      </div>
      <div class="deliverable">
        <div class="d-label">👥 21-Person Team</div>
        <div class="d-detail">Recruited, trained & onboarded. Built CI/CD infrastructure from zero.</div>
      </div>
      <div class="deliverable">
        <div class="d-label">🚀 5 Production Apps</div>
        <div class="d-detail">iOS + Android + Web + AI + Desktop. Initial funding secured. Clean handoff.</div>
      </div>
    </div>

    <div class="tech-tags">
      <span class="tech-tag">React Native</span>
      <span class="tech-tag">Next.js</span>
      <span class="tech-tag">NestJS</span>
      <span class="tech-tag">AWS</span>
      <span class="tech-tag">C++</span>
      <span class="tech-tag">Swift</span>
      <span class="tech-tag">Kotlin</span>
      <span class="tech-tag">TensorFlow</span>
      <span class="tech-tag">MediaPipe</span>
      <span class="tech-tag">Pinecone</span>
      <span class="tech-tag">Docker</span>
      <span class="tech-tag">Kubernetes</span>
      <span class="tech-tag">PostgreSQL</span>
      <span class="tech-tag">Electron</span>
    </div>
  </div>

  <!-- NonceBlox -->
  <div class="exp-card">
    <div class="role">Lead Mobile Architect & Senior Full-Stack Engineer</div>
    <div class="company">NonceBlox Pvt. Ltd. — 3+ Years</div>
    <div class="meta">Dubai (Remote) · Oct 2021 – Jan 2025 · FinTech / Web3 / Gaming</div>
    <p style="font-size:14px; color:#8B949E;">Owned end-to-end technical leadership shipping <strong>13+ production applications</strong> across FinTech, Web3, and Gaming sectors.</p>
  </div>

  <!-- Deployed Projects -->
  <h3>📱 Deployed & Live</h3>
  <div class="projects-grid">
    <div class="project-card">
      <span class="p-badge" style="background:rgba(255,107,53,0.15); color:#FF6B35;">SPORTS · FINTECH</span>
      <div class="p-name">Vulcan Eleven</div>
      <div class="p-desc">Fantasy sports platform. 60fps React Native with C++ native modules. Razorpay + Binance Pay.</div>
      <div class="tech-tags" style="margin:8px 0;">
        <span class="tech-tag">React Native</span>
        <span class="tech-tag">C++</span>
        <span class="tech-tag">Razorpay</span>
        <span class="tech-tag">Binance Pay</span>
      </div>
      <div class="p-links">
        <a href="https://apps.apple.com/ua/app/vulcan-eleven/id6462420052">📱 iOS</a>
        <a href="https://play.google.com/store/apps/details?id=com.vulcaneleven">🤖 Android</a>
      </div>
    </div>
    <div class="project-card">
      <span class="p-badge" style="background:rgba(0,245,212,0.12); color:#00F5D4;">PROPTECH</span>
      <div class="p-name">Housezy</div>
      <div class="p-desc">Subscription-based housing app. GraphQL APIs, Socket.io real-time, PayU + Google Pay.</div>
      <div class="tech-tags" style="margin:8px 0;">
        <span class="tech-tag">Expo</span>
        <span class="tech-tag">GraphQL</span>
        <span class="tech-tag">Socket.io</span>
        <span class="tech-tag">PayU</span>
      </div>
      <div class="p-links">
        <a href="https://apps.apple.com/us/app/housezy/id6471949955">📱 iOS</a>
        <a href="https://play.google.com/store/apps/details?id=com.nonceblox.housezy">🤖 Android</a>
      </div>
    </div>
    <div class="project-card">
      <span class="p-badge" style="background:rgba(155,93,229,0.15); color:#9B5DE5;">WEB3 · MUSIC</span>
      <div class="p-name">MusicX</div>
      <div class="p-desc">Music competition with blockchain royalties. Native C++ modules, 60fps animations, Spotify + Twitter API.</div>
      <div class="tech-tags" style="margin:8px 0;">
        <span class="tech-tag">React Native</span>
        <span class="tech-tag">C++ Modules</span>
        <span class="tech-tag">Blockchain</span>
      </div>
      <div class="p-links">
        <a href="https://apps.apple.com/us/app/music-x/id6475713772">📱 iOS</a>
      </div>
    </div>
    <div class="project-card">
      <span class="p-badge" style="background:rgba(201,168,76,0.15); color:#C9A84C;">DEFI · WEB3</span>
      <div class="p-name">DeFi11</div>
      <div class="p-desc">Fully on-chain fantasy sports. Smart contract prize pools, NFT marketplace on Ethereum.</div>
      <div class="tech-tags" style="margin:8px 0;">
        <span class="tech-tag">Solidity</span>
        <span class="tech-tag">Web3.js</span>
        <span class="tech-tag">Ethereum</span>
        <span class="tech-tag">NFTs</span>
      </div>
      <div class="p-links">
        <a href="https://apps.apple.com/app/defi11-fantasy-sports-app/id1608967244">📱 iOS</a>
      </div>
    </div>
  </div>

  <!-- More projects -->
  <div class="exp-card" style="border-left-color: #F5C842;">
    <div class="role" style="font-size:15px;">More Shipped Applications</div>
    <ul>
      <li><strong>Memr</strong> — Web3 whale tracker MVP. Next.js 15, Wagmi/Viem, WalletConnect, PayPal + Fiat.</li>
      <li><strong>Be4You</strong> — Dating app MVP. WebRTC video, Socket.io chat, PostGIS geolocation. Client secured seed funding in 90 days.</li>
      <li><strong>WeFoU</strong> — Proximity-based social networking with live maps & real-time activity.</li>
      <li><strong>CryptoCoffeeTales</strong> — Blockchain news with IPFS storage. <a href="https://play.google.com/store/apps/details?id=com.nonceblox.cryptocoffetales" style="color:#58A6FF;">Android</a></li>
      <li><strong>HRMS</strong> — Desktop employee management with Electron + live monitoring.</li>
    </ul>
  </div>

  <!-- Early Career -->
  <div class="exp-card" style="border-left-color: #DAA520;">
    <div class="role">Senior Full-Stack Engineer</div>
    <div class="company">TechProMind & WebSkitters — Foundation Years</div>
    <div class="meta">Kolkata, India · May 2017 – Oct 2021 · GovTech / Enterprise</div>
    <ul>
      <li>Secured & restructured <strong>13+ government projects</strong> — enterprise-grade SQL injection/XSS hardening.</li>
      <li>Architected <strong>GST Ecosystem</strong> from scratch (Merchant Portal + Retailer Software + Android App).</li>
      <li>Migrated legacy PHP → Angular/REST; improved system efficiency by 40%.</li>
      <li>Designed Oracle/MySQL data pipelines for government-scale processing.</li>
    </ul>
  </div>

  <hr/>

  <!-- ═══ TECH ARSENAL ═══ -->
  <h2>🛠️ Technical Arsenal</h2>
  <div class="arsenal-section">
    <div class="arsenal-category">
      <h4>📱 Mobile Architecture</h4>
      <div class="arsenal-badges">
        <span class="a-badge" style="background:#20232A;">⚛️ React Native (Expert)</span>
        <span class="a-badge" style="background:#1C1E24;">📦 Expo</span>
        <span class="a-badge" style="background:#3178C6;">TS TypeScript</span>
        <span class="a-badge" style="background:#00599C;">C++ Native Modules</span>
        <span class="a-badge" style="background:#FA7343;">🐦 Swift</span>
        <span class="a-badge" style="background:#7F52FF;">K Kotlin</span>
        <span class="a-badge" style="background:#333;">🍎 iOS</span>
        <span class="a-badge" style="background:#3DDC84; color:#000;">🤖 Android</span>
      </div>
    </div>
    <div class="arsenal-category">
      <h4>🧠 AI & Machine Learning</h4>
      <div class="arsenal-badges">
        <span class="a-badge" style="background:#412991;">🤖 LLM (OpenAI/Claude)</span>
        <span class="a-badge" style="background:#C9A84C; color:#000;">✨ Aura AI (Custom)</span>
        <span class="a-badge" style="background:#FF6F00;">🔥 TensorFlow</span>
        <span class="a-badge" style="background:#4285F4;">👁️ MediaPipe</span>
        <span class="a-badge" style="background:#333;">📌 Pinecone</span>
        <span class="a-badge" style="background:#34D399; color:#000;">🔗 RAG Pipelines</span>
        <span class="a-badge" style="background:#C084FC; color:#000;">🤖 Agentic AI</span>
      </div>
    </div>
    <div class="arsenal-category">
      <h4>⛓️ Web3 & Blockchain</h4>
      <div class="arsenal-badges">
        <span class="a-badge" style="background:#363636;">◆ Solidity</span>
        <span class="a-badge" style="background:#3C3C3D;">◇ Ethereum</span>
        <span class="a-badge" style="background:#9945FF;">◈ Solana</span>
        <span class="a-badge" style="background:#B7410E;">🦀 Rust (Learning)</span>
        <span class="a-badge" style="background:#F16822;">🌐 Web3.js</span>
        <span class="a-badge" style="background:#333;">⚡ Ethers.js / Viem</span>
        <span class="a-badge" style="background:#65C2CB; color:#000;">📦 IPFS</span>
      </div>
    </div>
    <div class="arsenal-category">
      <h4>⚙️ Backend & APIs</h4>
      <div class="arsenal-badges">
        <span class="a-badge" style="background:#E0234E;">🐈 NestJS</span>
        <span class="a-badge" style="background:#339933;">🟢 Node.js</span>
        <span class="a-badge" style="background:#E10098;">◈ GraphQL</span>
        <span class="a-badge" style="background:#092E20;">🐍 Django</span>
        <span class="a-badge" style="background:#010101;">🔌 Socket.io</span>
        <span class="a-badge" style="background:#333;">📹 WebRTC</span>
      </div>
    </div>
    <div class="arsenal-category">
      <h4>🎨 Frontend</h4>
      <div class="arsenal-badges">
        <span class="a-badge" style="background:#20232A;">⚛️ React.js</span>
        <span class="a-badge" style="background:#111;">▲ Next.js 15</span>
        <span class="a-badge" style="background:#764ABC;">🔄 Redux</span>
        <span class="a-badge" style="background:#06B6D4; color:#000;">🌊 Tailwind CSS</span>
        <span class="a-badge" style="background:#0055FF;">🎞️ Framer Motion</span>
        <span class="a-badge" style="background:#88CE02; color:#000;">🟢 GSAP</span>
        <span class="a-badge" style="background:#47848F;">⚡ Electron</span>
      </div>
    </div>
    <div class="arsenal-category">
      <h4>🗄️ Databases</h4>
      <div class="arsenal-badges">
        <span class="a-badge" style="background:#4169E1;">🐘 PostgreSQL</span>
        <span class="a-badge" style="background:#47A248;">🍃 MongoDB</span>
        <span class="a-badge" style="background:#DC382D;">⚡ Redis</span>
        <span class="a-badge" style="background:#FFCA28; color:#000;">🔥 Firebase</span>
        <span class="a-badge" style="background:#4479A1;">🐬 MySQL</span>
      </div>
    </div>
    <div class="arsenal-category">
      <h4>☁️ Cloud & DevOps</h4>
      <div class="arsenal-badges">
        <span class="a-badge" style="background:#232F3E;">☁️ AWS</span>
        <span class="a-badge" style="background:#2496ED;">🐳 Docker</span>
        <span class="a-badge" style="background:#326CE5;">☸️ Kubernetes</span>
        <span class="a-badge" style="background:#2088FF;">⚙️ GitHub Actions</span>
        <span class="a-badge" style="background:#00F200; color:#000;">🚀 Fastlane</span>
        <span class="a-badge" style="background:#3FCF8E; color:#000;">⚡ Supabase</span>
      </div>
    </div>
    <div class="arsenal-category">
      <h4>💳 Payments & FinTech</h4>
      <div class="arsenal-badges">
        <span class="a-badge" style="background:#008CDD;">💳 Stripe</span>
        <span class="a-badge" style="background:#003087;">🅿️ PayPal</span>
        <span class="a-badge" style="background:#0C2451;">₹ Razorpay</span>
        <span class="a-badge" style="background:#F0B90B; color:#000;">₿ Binance Pay</span>
      </div>
    </div>
  </div>

  <hr/>

  <!-- ═══ GITHUB STATS ═══ -->
  <h2>📊 GitHub Activity</h2>
  <div class="github-stats">
    <img src="https://github-readme-stats.vercel.app/api?username=devamitch&show_icons=true&theme=dark&hide_border=true&bg_color=0D1117&title_color=C9A84C&icon_color=C9A84C&text_color=FFFFFF&ring_color=C9A84C" width="48%" />
    <img src="https://github-readme-streak-stats.herokuapp.com?user=devamitch&theme=dark&hide_border=true&background=0D1117&ring=C9A84C&fire=F5C842&currStreakLabel=C9A84C&sideLabels=C9A84C" width="48%" />
  </div>
  <div class="github-stats">
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=devamitch&layout=compact&theme=dark&hide_border=true&bg_color=0D1117&title_color=C9A84C&text_color=FFFFFF&langs_count=12" width="48%" />
  </div>
  <div class="github-stats" style="margin-top:8px;">
    <img src="https://github-readme-activity-graph.vercel.app/graph?username=devamitch&theme=github-dark&hide_border=true&bg_color=0D1117&color=C9A84C&line=F5C842&point=FFFFFF&area=true&area_color=C9A84C" width="96%" />
  </div>

  <hr/>

  <!-- ═══ BLOG ═══ -->
  <h2>✍️ Latest Blog Posts</h2>
  <div class="blog-list">
    <a class="blog-item" href="https://devamitch.medium.com/say-goodbye-to-git-woes-become-a-git-wizard-today-c6f6e7c10b7a">
      <span class="b-emoji">🧙‍♂️</span>
      <div><div class="b-title">Say Goodbye to Git Woes: Become a Git Wizard Today!</div><div class="b-cat">DevOps / Git · Jan 2025</div></div>
    </a>
    <a class="blog-item" href="https://devamitch.medium.com/lets-build-your-first-electron-app-the-magical-feed-app-7d8e9f2a1b3c">
      <span class="b-emoji">🪄</span>
      <div><div class="b-title">Let's Build Your First Electron App: The Magical Feed App!</div><div class="b-cat">Desktop / Electron · Nov 2024</div></div>
    </a>
    <a class="blog-item" href="https://devamitch.medium.com/from-typescript-to-rust-go-day-3-mastering-functions-and-error-handling-c2d1e4f5a6b7">
      <span class="b-emoji">🦀</span>
      <div><div class="b-title">From TypeScript to Rust & Go — Day 3: Mastering Functions</div><div class="b-cat">Rust & Go · Nov 2024</div></div>
    </a>
    <a class="blog-item" href="https://devamitch.medium.com/expo-vs-bare-react-native-which-should-you-use-and-when-f2b3c4d5e6f7">
      <span class="b-emoji">📱</span>
      <div><div class="b-title">Expo vs. Bare React Native: Which Should You Use and When?</div><div class="b-cat">Mobile / React Native · Oct 2024</div></div>
    </a>
    <a class="blog-item" href="https://devamitch.medium.com/understanding-type-vs-interface-in-typescript-a-guide-for-junior-developers-a1b2c3d4e5f6">
      <span class="b-emoji">🔷</span>
      <div><div class="b-title">Understanding Type vs. Interface in TypeScript</div><div class="b-cat">TypeScript · Sep 2024</div></div>
    </a>
  </div>

  <hr/>

  <!-- ═══ TESTIMONIALS ═══ -->
  <h2>📜 Testimonials</h2>
  <div class="testimonial">
    <div class="t-text">I had the pleasure of working with Amit for three years and witnessed his impressive growth from Front-End Developer to Front-End Lead. His expertise and dedication make him a valuable asset to any team.</div>
    <div class="t-author">Kartik Kalia</div>
    <div class="t-role">Full Stack Developer · AWS · NonceBlox (Direct Manager, 3 years)</div>
  </div>
  <div class="testimonial">
    <div class="t-text">Amit had been an amicable and diligent developer, one of the most dependable Engineers when it comes to delivery or urgent closures. His capability to rebuild any project from scratch is remarkable.</div>
    <div class="t-author">Neha Goel</div>
    <div class="t-role">HR Professional · 15+ Years · NonceBlox (Senior Leadership)</div>
  </div>
  <div class="testimonial">
    <div class="t-text">Amit played a pivotal role in mentoring me, sharing his profound knowledge of Redux, React Native, and frontend concepts. His enthusiasm for coding and pursuit for perfection are truly inspiring.</div>
    <div class="t-author">Varun Chodha</div>
    <div class="t-role">Senior Full-Stack · MERN · NonceBlox (Grew under Amit's guidance)</div>
  </div>

  <hr/>

  <!-- ═══ JOURNEY ═══ -->
  <h2>🗺️ The Journey</h2>
  <div class="timeline">
    <div class="timeline-item">
      <div class="t-year">2017</div>
      <div class="t-title">The Origin</div>
      <div class="t-desc">PHP developer. Government projects. 13 secured and shipped. Built GST portals, Android apps, and retailer software from zero.</div>
    </div>
    <div class="timeline-item">
      <div class="t-year">2019</div>
      <div class="t-title">MCA & Upskilling</div>
      <div class="t-desc">Master's in Computer Applications. 8.61 CGPA. React, React Native, Web3 foundations running in parallel.</div>
    </div>
    <div class="timeline-item">
      <div class="t-year">2021</div>
      <div class="t-title">Web3 & Blockchain</div>
      <div class="t-desc">Joined NonceBlox. Deep-dived into Solidity, DeFi, NFTs. Built DeFi11 — fully decentralized fantasy sports.</div>
    </div>
    <div class="timeline-item">
      <div class="t-year">2023</div>
      <div class="t-title">The Lead Role</div>
      <div class="t-desc">Lead Mobile Developer. Owned architecture for MusicX, Housezy, Vulcan Eleven. C++ Native Modules. Razorpay + Binance Pay.</div>
    </div>
    <div class="timeline-item">
      <div class="t-year">2025</div>
      <div class="t-title">AI + HealthTech</div>
      <div class="t-desc">Proprietary game engine from scratch. RAG pipelines. Aura AI. Computer vision. 21-person team. VP-level operations.</div>
    </div>
    <div class="timeline-item" style="margin-bottom:0;">
      <div class="t-year">Now</div>
      <div class="t-title">Building What's Next</div>
      <div class="t-desc">Open for the right mission. Building my own products. The title matters less than the impact.</div>
    </div>
  </div>

  <hr/>

  <!-- ═══ EDUCATION ═══ -->
  <h2>🎓 Education & Certifications</h2>
  <div class="edu-grid">
    <div class="edu-card">
      <div class="e-degree">Master of Computer Applications (MCA)</div>
      <div class="e-school">Techno Main Salt Lake, Kolkata</div>
      <div class="e-score">8.61 CGPA</div>
      <div class="e-year">2018 – 2021</div>
    </div>
    <div class="edu-card">
      <div class="e-degree">Bachelor of Computer Applications (BCA)</div>
      <div class="e-school">The Heritage Academy, Kolkata</div>
      <div class="e-score">7.3 DGPA</div>
      <div class="e-year">2014 – 2017</div>
    </div>
  </div>
  <div class="cert-tags">
    <span class="cert-tag">Blockchain Development (Udemy)</span>
    <span class="cert-tag">DevOps: CI/CD, Docker, K8s (LinkedIn)</span>
    <span class="cert-tag">Solana Blockchain (Udemy)</span>
    <span class="cert-tag">DeFi Development (Coursera)</span>
    <span class="cert-tag">HackerRank: React, Java, Python</span>
    <span class="cert-tag">🏆 Cognizant Hackathon 2021 — Quarterfinalist</span>
  </div>

  <hr/>

  <!-- ═══ SERVICES ═══ -->
  <h2>💡 Services</h2>
  <div class="services-grid">
    <div class="service-card">
      <div class="s-icon">🎯</div>
      <div class="s-title">Pitch Your Idea</div>
      <div class="s-desc">Technical feasibility, MVP scope, architecture blueprint, timeline & cost estimate.</div>
      <div class="s-price">Free discovery call</div>
    </div>
    <div class="service-card">
      <div class="s-icon">🔍</div>
      <div class="s-title">Consulting</div>
      <div class="s-desc">Architecture reviews, code audits, team advisory, 1:1 mentorship sessions.</div>
      <div class="s-price">From $150/hr</div>
    </div>
    <div class="service-card">
      <div class="s-icon">🚀</div>
      <div class="s-title">End-to-End Build</div>
      <div class="s-desc">Full 0-to-1 product build with team setup and post-launch support.</div>
      <div class="s-price">Fixed scope</div>
    </div>
  </div>

  <hr/>

  <!-- ═══ COLLABORATION ═══ -->
  <h2>🤝 Open for Collaboration</h2>
  <div class="collab-grid">
    <div class="collab-item">
      <div class="c-icon">🚀</div>
      <div class="c-title">0-to-1 Execution</div>
      <div class="c-desc">15+ products from napkin sketch to production. I know what breaks and what ships.</div>
    </div>
    <div class="collab-item">
      <div class="c-icon">🏗️</div>
      <div class="c-title">Architecture That Scales</div>
      <div class="c-desc">Game engines, HIPAA AI pipelines, on-chain smart contracts — systems that survive reality.</div>
    </div>
    <div class="collab-item">
      <div class="c-icon">👥</div>
      <div class="c-title">Team Building</div>
      <div class="c-desc">I recruit, mentor, and build engineering cultures from scratch. Not just code.</div>
    </div>
    <div class="collab-item">
      <div class="c-icon">🧠</div>
      <div class="c-title">Founder Mindset</div>
      <div class="c-desc">I treat every product like my own company. Full ownership, full accountability.</div>
    </div>
  </div>

  <div class="cta-box">
    <p><strong>💼 Contract · Full-Time · Fractional CTO</strong><br/>
    🌍 Remote Worldwide (IST, flexible overlap) &nbsp;·&nbsp; ⚡ Available immediately</p>
    <div class="cta-buttons">
      <a class="cta-btn cta-btn-gold" href="https://devamit.co.in">🌐 devamit.co.in</a>
      <a class="cta-btn cta-btn-blue" href="https://linkedin.com/in/devamitch">💼 Let's Connect</a>
      <a class="cta-btn cta-btn-dark" href="mailto:amit98ch@gmail.com">📧 amit98ch@gmail.com</a>
    </div>
  </div>

  <div class="profile-views">
    <strong style="color:#E6EDF3;">If you're building something ambitious and need someone who won't quit until it ships — let's talk.</strong>
  </div>

  <div class="footer-line">
    Built with conviction. Shipped with pride. — Amit Chakraborty, 2026
  </div>

</div>

</body>
</html>
