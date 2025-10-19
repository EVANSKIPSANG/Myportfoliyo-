<!--
  Save this file as "index.html" and upload to a GitHub repo named "portfolio".
  For GitHub Pages: Settings → Pages → Source: main / root → Save.
  Then visit: https://your-username.github.io/portfolio/
-->

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Evans Kipsang — Portfolio</title>
  <meta name="description" content="Portfolio of Evans Kipsang — Mathematics & Computer Science graduate, ICT trainer and web developer.">

  <!-- Google Font (optional) -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    /* ---------- Reset & base ---------- */
    :root{
      --accent:#0f62fe;
      --muted:#6b7280;
      --bg:#f7fbff;
      --card:#ffffff;
      --radius:12px;
      --maxw:1100px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:"Inter",system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
      background:var(--bg);
      color:#0f1724;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.45;
    }
    a{color:var(--accent); text-decoration:none}
    img{max-width:100%;display:block}

    /* ---------- Layout ---------- */
    .wrap{max-width:var(--maxw);margin:36px auto;padding:24px;}
    header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
      margin-bottom:20px;
    }
    .brand{
      display:flex;
      gap:14px;
      align-items:center;
    }
    .logo{
      width:56px;height:56px;border-radius:12px;
      background:linear-gradient(135deg,var(--accent),#4f46e5);
      display:grid;place-items:center;color:white;font-weight:700;font-size:20px;
      box-shadow:0 6px 18px rgba(15,98,254,0.12);
    }
    nav{display:flex;gap:14px;align-items:center;}
    nav a{padding:8px 10px;border-radius:8px;font-weight:600;color:#0f1724;opacity:.85}
    nav a:hover{background:rgba(15,98,254,0.08);color:var(--accent)}

    /* ---------- Hero ---------- */
    .hero{
      display:grid;
      grid-template-columns: 1fr 360px;
      gap:28px;
      align-items:center;
      margin-bottom:28px;
    }
    .hero-card{
      background:var(--card);
      border-radius:var(--radius);
      padding:28px;
      box-shadow:0 6px 24px rgba(15,23,42,0.06);
    }
    h1{margin:0;font-size:28px;letter-spacing:-0.02em}
    .sub{color:var(--muted);margin-top:8px}

    .cta-row{margin-top:18px;display:flex;gap:12px;flex-wrap:wrap}
    .btn{
      display:inline-flex;gap:10px;align-items:center;padding:10px 14px;border-radius:10px;
      font-weight:600;background:var(--accent);color:white;border:0;cursor:pointer;
      box-shadow:0 6px 18px rgba(15,98,254,0.12);
    }
    .btn.secondary{background:transparent;color:var(--accent);border:1px solid rgba(15,98,254,0.16);box-shadow:none}

    .profile-box{
      padding:18px;background:linear-gradient(180deg,rgba(15,98,254,0.06),transparent);
      border-radius:12px;text-align:center;
    }
    .profile-photo{
      width:120px;height:120px;border-radius:18px;margin:8px auto;object-fit:cover;background:#e6f0ff;
      display:grid;place-items:center;font-weight:700;color:var(--accent);
      font-size:32px;
    }

    /* ---------- Sections ---------- */
    .grid{
      display:grid;
      grid-template-columns: 1fr 360px;
      gap:24px;
      align-items:start;
    }
    section.card{
      background:var(--card);
      border-radius:var(--radius);
      padding:20px;
      box-shadow:0 6px 18px rgba(2,6,23,0.04);
      margin-bottom:18px;
    }
    h2{margin:0 0 12px 0;color:#0b3b66;font-size:18px}
    ul.skill-list{display:flex;flex-wrap:wrap;gap:8px;list-style:none;padding:0;margin:0}
    ul.skill-list li{background:#f1f7ff;padding:8px 12px;border-radius:999px;font-weight:600;color:#064e9a;font-size:13px}

    .project{
      border-radius:10px;padding:12px;background:linear-gradient(180deg,#ffffff, #fbfdff);
      margin-bottom:12px;border:1px solid rgba(8,30,80,0.04);
    }
    .project h3{margin:0;font-size:15px}
    .project p{color:var(--muted);margin:6px 0 0 0;font-size:14px}

    .meta{font-size:13px;color:var(--muted);margin-top:8px}

    /* ---------- Contact & Footer ---------- */
    .contact-list{display:flex;flex-direction:column;gap:8px}
    .contact-card{display:flex;gap:10px;align-items:center;padding:10px;border-radius:10px;background:#fcfdff;border:1px solid rgba(8,30,80,0.03)}
    footer{margin-top:18px;padding:18px;text-align:center;color:var(--muted);font-size:14px}

    /* ---------- Responsive ---------- */
    @media (max-width:980px){
      .hero,.grid{grid-template-columns:1fr}
      nav{display:none}
      header{align-items:flex-start;flex-direction:column;gap:12px}
      .profile-box{order: -1}
    }
    @media (max-width:480px){
      .wrap{padding:16px}
      h1{font-size:22px}
      .logo{width:48px;height:48px;font-size:18px}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">EK</div>
        <div>
          <div style="font-weight:700">Evans Kipsang</div>
          <div style="font-size:13px;color:var(--muted)">Mathematics & Computer Science • ICT Trainer • Web Dev</div>
        </div>
      </div>

      <nav aria-label="Main navigation">
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <!-- HERO -->
    <main class="hero">
      <div class="hero-card">
        <h1>Hi — I'm Evans. I build learning tools and teach ICT.</h1>
        <p class="sub">
          Mathematics & Computer Science graduate from Kirinyaga University, with practical attachment experience at Chepsirei Technical College.
          I design web apps, manage educational resources, and deliver hands-on computer training.
        </p>

        <div class="cta-row">
          <a class="btn" href="#projects">View Projects</a>
          <a class="btn secondary" href="mailto:evansrotich269@gmail.com">Contact Me</a>
        </div>

        <section class="card" style="margin-top:18px">
          <h2>Quick Overview</h2>
          <p class="meta">
            • Experienced with PHP & MySQL, front-end (HTML/CSS/JS), and basic Python for data tasks.<br>
            • Built an Online Learning Platform & Resource Management System during university attachments.<br>
            • Strong in lesson planning, ICT training, and classroom technology support.
          </p>
        </section>
      </div>

      <aside class="profile-box">
        <div class="profile-photo" aria-hidden="true">EK</div>
        <div style="font-weight:700">Evans Kipsang</div>
        <div class="meta">Kutus, Kirinyaga • +254 768 551 090</div>

        <div style="margin-top:12px;display:flex;gap:8px;justify-content:center">
          <a class="btn" href="https://github.com/EVANSKIPSANG" target="_blank">GitHub</a>
          <a class="btn secondary" href="https://www.linkedin.com/in/evans-rotich-761616363/" target="_blank">LinkedIn</a>
        </div>
      </aside>
    </main>

    <!-- GRID: main + sidebar -->
    <div class="grid" role="region" aria-label="Portfolio content">
      <div>
        <section id="about" class="card">
          <h2>About Me</h2>
          <p class="meta">
            I am a dedicated and detail-oriented Mathematics & Computer Science graduate with practical attachment experience at Chepsirei Technical College.
            I enjoy turning course materials into interactive learning systems, automating resource workflows, and teaching computer fundamentals to students and staff.
          </p>
        </section>

        <section id="skills" class="card">
          <h2>Skills</h2>
          <ul class="skill-list" aria-hidden="false">
            <li>HTML & CSS</li>
            <li>JavaScript (vanilla)</li>
            <li>PHP & MySQL</li>
            <li>Basic Python & Excel</li>
            <li>Responsive Design</li>
            <li>ICT Training & Lesson Planning</li>
          </ul>
        </section>

        <section id="projects" class="card">
          <h2>Selected Projects</h2>

          <article class="project" aria-labelledby="p1">
            <h3 id="p1">Online Learning Platform</h3>
            <p>
              Full-stack learning platform (PHP/MySQL) that supports user registration, role-based access (students/teachers), resource uploads, and progress tracking.
            </p>
            <p class="meta">Technologies: PHP, MySQL, HTML/CSS, JavaScript</p>
            <p style="margin-top:10px"><a href="#" aria-label="View project details">View code on GitHub →</a></p>
          </article>

          <article class="project" aria-labelledby="p2">
            <h3 id="p2">Resource Management System</h3>
            <p>
              A lightweight system for uploading and sharing PDFs/Word docs with download tracking and search filters — designed for a college resource center.
            </p>
            <p class="meta">Technologies: PHP, MySQL, Bootstrap (optional)</p>
            <p style="margin-top:10px"><a href="#" aria-label="View project details">View code on GitHub →</a></p>
          </article>

          <article class="project" aria-labelledby="p3">
            <h3 id="p3">Student Profile & Dashboard</h3>
            <p>
              Personalized student dashboard showing enrolled resources and recommended materials based on class assignments and progress.
            </p>
            <p class="meta">Technologies: PHP, MySQL, JavaScript</p>
          </article>
        </section>

        <section class="card">
          <h2>Certificates & Achievements</h2>
          <ul>
            <li style="margin-bottom:6px">Certificate: ICT Training Facilitation — Chepsirei Technical College (2024)</li>
            <li style="margin-bottom:6px">Project: Online Learning Platform — Final Year Project (2025)</li>
            <li style="margin-bottom:6px">EF SET English Assessment — B1 Intermediate</li>
          </ul>
        </section>
      </div>

      <aside>
        <section id="contact" class="card">
          <h2>Contact</h2>
          <div class="contact-list">
            <div class="contact-card">
              <strong>Email</strong>
              <div style="margin-left:auto"><a href="mailto:evansrotich269@gmail.com">evansrotich269@gmail.com</a></div>
            </div>

            <div class="contact-card">
              <strong>Phone</strong>
              <div style="margin-left:auto">+254 768 551 090</div>
            </div>

            <div class="contact-card">
              <strong>Location</strong>
              <div style="margin-left:auto">Kutus, Kirinyaga, Kenya</div>
            </div>
          </div>
        </section>

        <section class="card" aria-label="Quick links">
          <h2>Quick Links</h2>
          <div style="display:flex;flex-direction:column;gap:8px">
            <a class="contact-card" href="https://github.com/EVANSKIPSANG" target="_blank"><strong>GitHub</strong><span style="margin-left:auto">View repositories →</span></a>
            <a class="contact-card" href="https://www.linkedin.com/in/evans-rotich-761616363/" target="_blank"><strong>LinkedIn</strong><span style="margin-left:auto">Connect →</span></a>
            <a class="contact-card" href="#" download><strong>Download CV</strong><span style="margin-left:auto">PDF</span></a>
          </div>
        </section>
      </aside>
    </div>

    <footer>
      © <span id="year"></span> Evans Kipsang — Built with HTML & CSS • Hosted on GitHub Pages
    </footer>
  </div>

  <script>
    // small helpers
    document.getElementById('year').textContent = new Date().getFullYear();

    // Optional: simple smooth scroll for in-page links
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', e=>{
        const target = document.querySelector(a.getAttribute('href'));
        if(target){ e.preventDefault(); target.scrollIntoView({behavior:'smooth', block:'start'}); }
      });
    });
  </script>
</body>
</html>
