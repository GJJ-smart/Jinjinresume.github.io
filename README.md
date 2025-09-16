# Jinjinresume.github.io
Welcome to visit my world
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>JINJIN GUO — Resume</title>
  <meta name="description" content="Online resume of JINJIN GUO — Signal Processing & Machine Learning." />
  <link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='0.9em' font-size='90'>💼</text></svg>">
  <style>
    /* ===== Design tokens ===== */
    :root{
      --bg:#0b0c0f; --panel:#111319; --text:#e8ecf1; --muted:#a7b0bd; --chip:#1a1e27; --border:#222631; --shadow:0 10px 30px rgba(0,0,0,.35);
      --brand:#82b1ff; --accent:#72e0a9; --link:#9ec1ff;
    }
    .light:root{ --bg:#f7f9fc; --panel:#ffffff; --text:#0f172a; --muted:#475569; --chip:#eef2f7; --border:#e5e9f2; --shadow:0 10px 24px rgba(2,6,23,.08); --link:#1d4ed8; }

    /* ===== Base ===== */
    *{box-sizing:border-box}
    html,body{height:100%}
    body{margin:0; font:400 16px/1.6 system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, "Helvetica Neue", Arial; color:var(--text); background:radial-gradient(1200px 700px at 10% -10%, rgba(130,177,255,.10), transparent 60%), var(--bg);} 
    a{color:var(--link); text-underline-offset:2px}

    .container{max-width:1024px; margin:0 auto; padding:24px}
    header.nav{position:sticky; top:0; z-index:50; backdrop-filter:saturate(180%) blur(8px); background:color-mix(in hsl, var(--bg), transparent 35%); border-bottom:1px solid var(--border);} 
    .nav-inner{display:flex; align-items:center; justify-content:space-between; gap:16px; padding:12px 24px; max-width:1100px; margin:0 auto;}
    .brand{display:flex; align-items:center; gap:12px}
    .logo{width:36px; height:36px; border-radius:8px; background:linear-gradient(135deg, var(--brand), var(--accent)); display:grid; place-items:center; color:#0b1020; font-weight:800}
    .brand h1{font-size:18px; margin:0}

    nav ul{list-style:none; display:flex; gap:16px; padding:0; margin:0; flex-wrap:wrap}
    nav a{color:var(--text); text-decoration:none; padding:8px 10px; border-radius:8px}
    nav a:hover{background:var(--chip); border:1px solid var(--border)}

    .toggle{border:1px solid var(--border); background:var(--panel); color:var(--text); border-radius:10px; padding:8px 12px; cursor:pointer}

    .hero{background:linear-gradient(180deg, rgba(130,177,255,.12), rgba(114,224,169,.10)); border:1px solid var(--border); border-radius:18px; box-shadow:var(--shadow); padding:28px; margin:24px auto; max-width:1100px}
    .title{display:flex; gap:18px; align-items:center; flex-wrap:wrap}
    .avatar{width:84px; height:84px; border-radius:50%; background:var(--chip); display:grid; place-items:center; font-weight:700; color:#0b1020; border:2px solid var(--border); background-image:linear-gradient(135deg, var(--brand), var(--accent))}
    .name{font-size:clamp(26px,4.5vw,36px); margin:0}
    .role{margin:2px 0 0; color:var(--muted); font-weight:500}
    .contact{display:flex; flex-wrap:wrap; gap:10px; margin-top:14px}
    .contact a{text-decoration:none; color:var(--text); background:var(--chip); border:1px solid var(--border); padding:8px 10px; border-radius:10px; display:inline-flex; align-items:center; gap:8px}

    .grid{display:grid; grid-template-columns:1.1fr .9fr; gap:24px; margin-top:24px}
    @media (max-width:860px){ .grid{grid-template-columns:1fr} }

    .card{background:var(--panel); border:1px solid var(--border); border-radius:16px; padding:22px; box-shadow:var(--shadow)}
    h2{margin:0 0 10px; font-size:18px}
    .muted{color:var(--muted)}

    .timeline{display:flex; flex-direction:column; gap:18px}
    .item{display:grid; grid-template-columns:1fr auto; align-items:baseline; gap:8px}
    .item h3{margin:0; font-size:16px}
    .item .where{color:var(--muted); font-weight:500}
    .item .when{color:var(--muted); font-size:13px}
    .item ul{margin:8px 0 0 18px; padding:0}

    .chips{display:flex; flex-wrap:wrap; gap:8px}
    .chip{background:var(--chip); border:1px solid var(--border); padding:6px 10px; border-radius:999px; font-size:13px}
    .project{border:1px solid var(--border); background:linear-gradient(180deg, rgba(114,224,169,.05), transparent 60%); padding:14px; border-radius:12px}

    .foot{text-align:center; color:var(--muted); font-size:12px; margin:22px 0}

    @media print{ body{background:#fff} header.nav{display:none} .hero,.card{box-shadow:none} .chip{background:#f6f8fa; border-color:#e6e9ee} .container{padding:0} }
  </style>
</head>
<body>
  <header class="nav" aria-label="Top navigation">
    <div class="nav-inner">
      <div class="brand">
        <div class="logo">JG</div>
        <h1>JINJIN GUO</h1>
      </div>
      <nav>
        <ul>
          <li><a href="#about">About</a></li>
          <li><a href="#experience">Experience</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#skills">Skills</a></li>
          <li><a href="#education">Education</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
      <button class="toggle" id="themeToggle" aria-label="Toggle theme">🌗 Theme</button>
    </div>
  </header>

  <main class="container">
    <!-- Hero -->
    <section class="hero" id="about">
      <div class="title">
        <div class="avatar" aria-hidden="true">JG</div>
        <div>
          <h2 class="name" style="margin-bottom:6px">JINJIN GUO</h2>
          <div class="role">Signal Processing & Machine Learning · Singapore</div>
        </div>
      </div>
      <div class="contact" style="margin-top:12px">
        <a href="mailto:JINJIN002@e.ntu.edu.sg">✉️ JINJIN002@e.ntu.edu.sg</a>
        <a href="tel:+6592305756">📱 +65 9230 5756</a>
        <a href="https://linkedin.com" target="_blank" rel="noopener">🔗 LinkedIn</a>
        <a href="https://github.com" target="_blank" rel="noopener">💻 GitHub</a>
      </div>
      <p class="muted" style="margin-top:12px">Graduate student at NTU (CGPA 4.25/5) focusing on signal processing and machine learning. Experience across medical AI (ICU intervention prediction, ECG analysis) and embedded systems (STM32, AD9837). IEEE JBHI publication; multiple competition awards.</p>
    </section>

    <!-- Content -->
    <section class="grid">
      <div>
        <article class="card" id="experience">
          <h2>Experience</h2>
          <div class="timeline">
            <div class="item">
              <div>
                <h3>Wireless Testing Intern — <span class="where">Shenzhen GrenTech Communication Co., Ltd.</span></h3>
                <ul>
                  <li>Set up & verified base stations; configured virtual testbeds.</li>
                  <li>Applied wireless comms/5G fundamentals in routine testing.</li>
                </ul>
              </div>
              <div class="when">Jul 2022 — Aug 2022</div>
            </div>
          </div>
        </article>

        <article class="card" id="projects" style="margin-top:24px">
          <h2>Projects & Publications</h2>
          <div class="project">
            <h3 style="margin:0 0 6px">ICU Interventions Prediction · <span class="muted">Multivariate TS‑GCN</span></h3>
            <p>Co‑authored <em>IEEE JBHI</em> (Vol.28, No.6, 2024): transparent decision‑support model for ICU interventions from EHR time series; led data processing & tuning; reached <strong>91.9% accuracy</strong>.</p>
          </div>
          <div class="project" style="margin-top:12px">
            <h3 style="margin:0 0 6px">Single‑Cell Extraction Machine · <span class="muted">STM32F103 · Keil · Python · AD9837</span></h3>
            <p>Developing code & hardware enabling single‑cell detection and micro‑titration; solved inter‑module communication and built control circuitry (A*STAR, 2025– ).</p>
          </div>
          <div class="project" style="margin-top:12px">
            <h3 style="margin:0 0 6px">Alzheimer’s Detection from DTI · <span class="muted">FSL · MATLAB · PARAFAC2</span></h3>
            <p>Preprocessed MRI with FSL; trained PARAFAC2 tensor model; engineered per‑region features; authored final paper (2023–2024).</p>
          </div>
          <div class="project" style="margin-top:12px">
            <h3 style="margin:0 0 6px">AI‑based ECG Analysis · <span class="muted">PyTorch</span></h3>
            <p>Processed 6,877 CPSC2018 ECG records; improved baseline CNN to <strong>86.3%</strong> with Deform‑CNN.</p>
          </div>
        </article>
      </div>

      <aside>
        <section class="card" id="skills">
          <h2>Skills</h2>
          <div class="chips">
            <span class="chip">Python</span>
            <span class="chip">MATLAB</span>
            <span class="chip">C++</span>
            <span class="chip">Signal Processing</span>
            <span class="chip">Machine Learning</span>
            <span class="chip">STM32 / Embedded</span>
            <span class="chip">Microsoft Office</span>
          </div>
        </section>

        <section class="card" id="education" style="margin-top:24px">
          <h2>Education</h2>
          <div class="item">
            <div>
              <h3>Master of Signal Processing & Machine Learning</h3>
              <div class="where">Nanyang Technological University, Singapore · CGPA 4.25/5</div>
            </div>
            <div class="when">Aug 2024 — Jan 2026</div>
          </div>
          <div class="item" style="margin-top:10px">
            <div>
              <h3>Bachelor of Communication Engineering</h3>
              <div class="where">University of Electronic Science and Technology of China</div>
            </div>
            <div class="when">Sep 2020 — Jun 2024</div>
          </div>
        </section>

        <section class="card" id="contact" style="margin-top:24px">
          <h2>Awards & Certifications</h2>
          <ul>
            <li>Ashtanga Yoga Instructor Certification (Jul 2024)</li>
            <li>First Prize, Vocal Group — 7th China University Student Art Exhibition (Jun 2024)</li>
            <li>Outstanding Social Practice Individual — UESTC (Jul 2021)</li>
            <li>Bronze — China International College Students’ “Internet+” Competition</li>
            <li>Second Prize — 2022 Sichuan Biomedical Engineering Innovation & Design</li>
          </ul>
        </section>
      </aside>
    </section>

    <p class="foot">© 2025 · Built for GitHub Pages · Print this page as PDF (File → Print → Save as PDF)</p>
  </main>

  <script>
    // ===== Light/Dark theme toggle with localStorage =====
    (function(){
      const key = 'jjg-theme';
      const root = document.documentElement;
      const saved = localStorage.getItem(key);
      if(saved === 'light'){ root.classList.add('light'); }
      document.getElementById('themeToggle').addEventListener('click', () => {
        root.classList.toggle('light');
        localStorage.setItem(key, root.classList.contains('light') ? 'light' : 'dark');
      });
    })();
  </script>
</body>
</html>
