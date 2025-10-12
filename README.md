# All of AI

[Wiki](https://github.com/Math-AI-Institute/AI/wiki)

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>AI World — Visual for README</title>
  <style>
    :root{
      --bg1:#0f1724; /* deep navy */
      --bg2:#071126; /* darker */
      --accent1:#7c3aed;
      --accent2:#06b6d4;
      --glass: rgba(255,255,255,0.06);
      --card: rgba(255,255,255,0.03);
      --muted: rgba(255,255,255,0.6);
      --fw-sans: -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial;
    }
    *{box-sizing:border-box}
    body{font-family:var(--fw-sans);margin:0;background:linear-gradient(135deg,var(--bg1),var(--bg2));color:#e6eef8;-webkit-font-smoothing:antialiased}

    .wrap{max-width:980px;margin:48px auto;padding:28px;border-radius:18px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));box-shadow:0 10px 40px rgba(2,6,23,0.6);backdrop-filter: blur(6px)}

    .hero{display:flex;gap:22px;align-items:center}
    .logo{
      width:132px;height:132px;border-radius:18px;display:flex;align-items:center;justify-content:center;background:linear-gradient(135deg,var(--accent1),var(--accent2));box-shadow:0 8px 30px rgba(12,15,30,0.6);flex-shrink:0;position:relative;overflow:hidden
    }
    .logo svg{width:84px;height:84px;filter:drop-shadow(0 6px 18px rgba(12,15,30,0.6))}
    h1{margin:0;font-size:28px}
    p.lead{margin:6px 0 0;color:var(--muted)}

    .badges{margin-top:14px;display:flex;gap:8px;flex-wrap:wrap}
    .badge{font-size:12px;padding:6px 10px;background:var(--glass);border-radius:999px;color:#dbeafe}

    .controls{margin-left:auto;display:flex;gap:8px;align-items:center}
    .btn{background:linear-gradient(90deg,rgba(255,255,255,0.04),rgba(255,255,255,0.02));border:1px solid rgba(255,255,255,0.04);padding:8px 12px;border-radius:10px;color:#eaf2ff;font-weight:600;font-size:13px;cursor:pointer}
    .btn.ghost{background:transparent;border:1px dashed rgba(255,255,255,0.04)}

    .search{margin-top:18px;display:flex;gap:8px}
    .search input{flex:1;padding:12px 14px;border-radius:12px;border:1px solid rgba(255,255,255,0.04);background:rgba(255,255,255,0.02);color:inherit}

    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:22px}
    .card{background:var(--card);padding:12px;border-radius:12px;border:1px solid rgba(255,255,255,0.02);min-height:96px}

    .card h3{margin:0;font-size:14px}
    .card p{margin:8px 0 0;font-size:13px;color:var(--muted)}

    .timeline{margin-top:26px;padding:12px;border-radius:12px;background:linear-gradient(180deg, rgba(0,0,0,0.04), rgba(255,255,255,0.01));border:1px solid rgba(255,255,255,0.02)}
    .event{display:flex;gap:12px;align-items:flex-start;padding:10px 6px;border-radius:8px}
    .dot{width:12px;height:12px;border-radius:50%;background:linear-gradient(135deg,var(--accent1),var(--accent2));flex-shrink:0;margin-top:6px}
    .meta{font-size:13px;color:var(--muted)}
    .meta strong{color:#fff}

    /* small screens */
    @media (max-width:860px){.grid{grid-template-columns:repeat(2,1fr)}.hero{flex-direction:row} .controls{margin-left:0}}
    @media (max-width:560px){.wrap{margin:18px;padding:18px}.grid{grid-template-columns:1fr}.hero{flex-direction:row;gap:14px}}

    /* subtle animated background lines */
    .bg-lines{position:absolute;inset:0;pointer-events:none;z-index:0;opacity:0.06}
    .glow{position:absolute;right:-60px;top:-80px;width:320px;height:320px;border-radius:50%;filter:blur(60px);background:radial-gradient(circle at 30% 30%, rgba(124,58,237,0.65), transparent 30%), radial-gradient(circle at 70% 70%, rgba(6,182,212,0.55), transparent 35%);mix-blend-mode:screen}

    /* small footer */
    .footer{margin-top:20px;color:var(--muted);font-size:13px;display:flex;justify-content:space-between;align-items:center}
    .links a{color:inherit;text-decoration:none;border-bottom:1px dashed rgba(255,255,255,0.02);padding-bottom:2px}

  </style>
</head>
<body>
  <div class="wrap">
    <div class="bg-lines" aria-hidden>
      <div class="glow"></div>
    </div>

    <div class="hero">
      <div class="logo" aria-hidden>
        <!-- simple abstract neural / globe mark -->
        <svg viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg">
          <circle cx="32" cy="32" r="30" stroke="rgba(255,255,255,0.18)" stroke-width="1" />
          <path d="M8 34c6-6 12-8 24-8s18 2 28 8" stroke="white" stroke-opacity="0.12" stroke-width="1" stroke-linecap="round"/>
          <g transform="translate(12,12)" fill="white" opacity="0.95">
            <circle cx="8" cy="8" r="3" fill-opacity="0.95"/>
            <circle cx="24" cy="16" r="2.2" fill-opacity="0.95"/>
            <circle cx="36" cy="6" r="2.8" fill-opacity="0.95"/>
            <path d="M6 18c8-6 20-6 30 0" stroke="rgba(255,255,255,0.06)" stroke-width="1.6" fill="none" stroke-linecap="round"/>
          </g>
        </svg>
      </div>

      <div>
        <h1>AI World
          <div style="font-size:12px;color:var(--muted);font-weight:600;display:inline-block;margin-left:10px">— curated map of AI advances</div>
        </h1>
        <p class="lead">Papers, projects and notable demos across large models, generative systems, agents, and more — curated and linked.</p>

        <div class="badges">
          <div class="badge">⭐ Curated</div>
          <div class="badge">📚 Papers</div>
          <div class="badge">🧪 Projects</div>
          <div class="badge">🔁 Updated</div>
        </div>

        <div class="search">
          <input placeholder="Search by title, author, tag — works in README when linked to a search script" />
          <button class="btn">Quick filter</button>
        </div>
      </div>

      <div class="controls">
        <button class="btn">Add entry</button>
        <button class="btn ghost">Contribute</button>
      </div>
    </div>

    <div class="grid" role="list">
      <div class="card" role="listitem">
        <h3>Large Language Models</h3>
        <p>Key papers, model cards and notable demos — evolution of scaling and instruction tuning.</p>
      </div>
      <div class="card">
        <h3>Generative Vision & Diffusion</h3>
        <p>Diffusion, latent models, and text-to-image project links with sample galleries.</p>
      </div>
      <div class="card">
        <h3>Agents & Tooling</h3>
        <p>Agents, tool-using LLMs, orchestration frameworks, and benchmarks.</p>
      </div>
      <div class="card">
        <h3>Reinforcement & Control</h3>
        <p>Learning to act: model-based, model-free, sim2real projects and notable environments.</p>
      </div>
      <div class="card">
        <h3>Foundations & Theory</h3>
        <p>Optimization, generalization, implicit biases, and theoretical progress.</p>
      </div>
      <div class="card">
        <h3>Tools & Datasets</h3>
        <p>Useful toolkits, dataset links, evaluation harnesses and leaderboards.</p>
      </div>
    </div>

    <div class="timeline" aria-label="recent updates">
      <div style="display:flex;justify-content:space-between;align-items:center">
        <strong>Latest additions</strong>
        <div style="font-size:13px;color:var(--muted)">Auto-updates possible via GitHub Actions</div>
      </div>

      <div style="margin-top:12px">
        <div class="event">
          <div class="dot" aria-hidden></div>
          <div>
            <div class="meta"><strong>2025-10-05</strong> — New paper: "Progressive Diffusion for Fast Sampling"</div>
            <div style="font-size:13px;color:var(--muted);margin-top:6px">Short note: improved sampling speed using progressive denoising schedules. <a href="#" style="color:inherit;text-decoration:underline">link</a></div>
          </div>
        </div>

        <div class="event">
          <div class="dot"></div>
          <div>
            <div class="meta"><strong>2025-09-01</strong> — Project added: Agent-Playground (tool-using agents)</div>
            <div style="font-size:13px;color:var(--muted);margin-top:6px">Includes demo and how-to. <a href="#" style="color:inherit;text-decoration:underline">link</a></div>
          </div>
        </div>
      </div>
    </div>

    <div class="footer">
      <div class="links">Use this block in <code>README.md</code> — simply paste the HTML into your Markdown file where HTML is supported.</div>
      <div style="font-size:13px;color:var(--muted)">Made for <strong>AI World</strong></div>
    </div>
  </div>
</body>
</html>
