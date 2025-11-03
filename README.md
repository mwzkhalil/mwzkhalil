<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Muhammad Mahwiz Khalil — Typewriter Resume</title>
  <style>
    /* Simple, adorable typewriter theme */
    :root{
      --bg:#f7f3ef; /* warm paper */
      --ink:#222;
      --accent:#d87f6a; /* soft coral */
      --muted:#6b6b6b;
      --paper-shadow: 0 6px 30px rgba(0,0,0,0.06);
    }
    html,body{height:100%;}
    body{
      margin:0; font-family: 'Courier New', Courier, monospace; background:linear-gradient(180deg,var(--bg),#fff); color:var(--ink);
      display:flex; align-items:center; justify-content:center; padding:32px;
    }
    .card{
      width:900px; max-width:96vw; background:linear-gradient(180deg,#fff, #fffbf8); border-radius:12px; box-shadow:var(--paper-shadow); padding:28px; border:1px solid rgba(0,0,0,0.04);
    }
    .header{display:flex; gap:20px; align-items:center;}
    .avatar{
      width:110px; height:110px; background:linear-gradient(135deg,var(--accent),#f3b2a0); border-radius:10px; display:flex; align-items:center; justify-content:center; color:white; font-weight:700; font-size:28px;
      box-shadow:0 8px 20px rgba(216,127,106,0.12);
    }
    h1{margin:0; font-size:28px; letter-spacing:1px}
    .meta{color:var(--muted); font-size:13px; margin-top:6px}
    .badges{margin-top:10px}
    .two-col{display:grid; grid-template-columns:1fr 1fr; gap:18px; margin-top:20px}
    .section{background:rgba(0,0,0,0.01); padding:14px; border-radius:8px;}
    .section h3{margin:0 0 8px 0; font-size:15px}
    ul{margin:6px 0 0 18px}
    .skills{display:flex; flex-wrap:wrap; gap:8px}
    .pill{font-family:inherit; font-size:12px; padding:6px 8px; border-radius:6px; border:1px dashed rgba(0,0,0,0.08); background:transparent}
    .projects{display:grid; gap:10px}
    .project{padding:10px; border-radius:6px; border-left:4px solid var(--accent); background:linear-gradient(180deg,rgba(0,0,0,0.01),transparent)}
    .footer{margin-top:18px; display:flex; justify-content:space-between; align-items:center; font-size:13px; color:var(--muted)}
    /* Typewriter cursor for name */
    .typewriter{display:inline-block; white-space:nowrap; overflow:hidden; border-right:3px solid var(--ink); animation:caret 1s steps(1) infinite;}
    @keyframes caret{50%{border-color:transparent}}
    /* small responsive tweaks */
    @media(max-width:720px){.two-col{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <div class="card">
    <div class="header">
      <div class="avatar">MM</div>
      <div>
        <h1><span class="typewriter">Muhammad Mahwiz Khalil</span></h1>
        <div class="meta">AI Systems Engineer — Karachi, Pakistan • +92 333 0214897 • khalilmahwiz@gmail.com</div>
        <div class="badges">
          <span class="pill">AI Systems</span>
          <span class="pill">MLOps</span>
          <span class="pill">NLP & Speech</span>
          <span class="pill">Low-resource languages</span>
        </div>
      </div>
    </div>

    <div class="two-col">
      <div class="section">
        <h3>Professional Summary</h3>
        <p style="margin:6px 0 0; font-size:14px">2+ years building production NLP & multimodal systems. Focused on transformer architectures, distributed training, and reliable MLOps — optimized for latency and cost.</p>

        <h3 style="margin-top:12px">Key Metrics</h3>
        <ul>
          <li>60% inference latency reduction (Kubernetes optimizations)</li>
          <li>25% infra cost savings (quantization & orchestration)</li>
          <li>100k+ daily requests served (Urdu STT/TTS)</li>
        </ul>

        <h3 style="margin-top:12px">Technical Skills</h3>
        <div class="skills" style="margin-top:8px">
          <div class="pill">Python</div>
          <div class="pill">PyTorch</div>
          <div class="pill">Whisper / ASR</div>
          <div class="pill">Kubernetes</div>
          <div class="pill">AWS</div>
          <div class="pill">FastAPI / Flask</div>
          <div class="pill">FAISS / Chroma</div>
        </div>
      </div>

      <div class="section">
        <h3>Experience</h3>
        <div style="margin-top:8px">
          <strong>AI Engineer — Nova Tech</strong><br>
          <small class="meta">Dubai, UAE (Remote) • Jun 2025 – Present</small>
          <p style="margin:8px 0 0">Architected multi-agent trading system; reduced latency 60%; built governance for regulated trading.</p>
        </div>

        <div style="margin-top:12px">
          <strong>NLP Engineer — Proxima AI</strong><br>
          <small class="meta">Pakistan • Aug 2023 – Present</small>
          <p style="margin:8px 0 0">Built Urdu STT/TTS production stack (100K+ daily), optimized costs, and led a team of 5 engineers.</p>
        </div>

        <div style="margin-top:12px">
          <strong>Data Research Analyst — Technexia</strong><br>
          <small class="meta">Pakistan • Jan 2023 – Jun 2023</small>
          <p style="margin:8px 0 0">Designed ingestion pipelines and real-time dashboards for C-suite decisioning.</p>
        </div>
      </div>
    </div>

    <div style="margin-top:18px" class="section">
      <h3>Featured Projects</h3>
      <div class="projects" style="margin-top:8px">
        <div class="project">
          <strong>TinyGemma-Urdu</strong> — 0.96M param Urdu LLM. 12% BLEU↑ vs mT5-small. Custom tokenizer and DDP training.
        </div>
        <div class="project">
          <strong>Whisper-Urdu-PyTorch</strong> — Optimized Urdu ASR: 9.1% WER, 3× inference speedup, ONNX + CUDA kernels.
        </div>
        <div class="project">
          <strong>AI HR Copilot</strong> — RAG-based automation, 90% routine query automation, FastAPI + FAISS.
        </div>
      </div>
    </div>

    <div class="two-col" style="margin-top:14px">
      <div class="section">
        <h3>Education & Certifications</h3>
        <p style="margin:6px 0 0"><strong>BSc Computer Science</strong> — University of Karachi (expected Aug 2028)</p>
        <p style="margin:6px 0 0"><strong>Diploma</strong> — Aligarh Institute of Technology (2023)</p>
        <div style="margin-top:8px" class="skills">
          <div class="pill">AWS — Production ML</div>
          <div class="pill">Google Cloud — Transformers</div>
          <div class="pill">IBM — Deep Learning</div>
        </div>
      </div>

      <div class="section">
        <h3>Open Source & Talks</h3>
        <ul>
          <li>Published 10+ models on Hugging Face (2Damnwav)</li>
          <li>Top 1% on Kaggle with LLM notebooks</li>
          <li>Speaker: SMIU AI Conference 2025 — "Scaling Transformers for Low-Resource Languages"</li>
        </ul>
      </div>
    </div>

    <div class="footer">
      <div>Available for roles in AI Systems, MLOps & Research — Q1 2026</div>
      <div style="text-align:right">Last updated: Nov 3, 2025</div>
    </div>
  </div>
</body>
</html>
