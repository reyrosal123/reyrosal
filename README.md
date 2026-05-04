<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Rey Rosal — GoHighLevel Expert & Automation Specialist</title>

<link rel="icon" type="image/svg+xml" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'><defs><linearGradient id='g' x1='0%25' y1='0%25' x2='100%25' y2='100%25'><stop offset='0%25' stop-color='%23f59e0b'/><stop offset='50%25' stop-color='%23ef4444'/><stop offset='100%25' stop-color='%238b5cf6'/></linearGradient></defs><rect width='64' height='64' rx='14' fill='url(%23g)'/><text x='50%25' y='54%25' dominant-baseline='middle' text-anchor='middle' font-family='Arial Black,sans-serif' font-weight='900' font-size='26' fill='white'>RR</text></svg>" />

<link href="https://fonts.googleapis.com/css2?family=Syne:wght@700;800&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet" />
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
:root {
  --bg: #080810;
  --surface: #0e0e1a;
  --card: #12121f;
  --border: rgba(255,255,255,0.07);
  --white: #f0f0ff;
  --muted: #6b6b9a;
  --amber: #f59e0b;
  --grad: linear-gradient(135deg, #f59e0b 0%, #ef4444 55%, #8b5cf6 100%);
}
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;scroll-padding-top:72px;}
body{font-family:'DM Sans',sans-serif;background:var(--bg);color:var(--white);overflow-x:hidden;line-height:1.6;}

/* NAV */
.nav{position:fixed;top:0;left:0;right:0;z-index:999;background:rgba(8,8,16,0.92);backdrop-filter:blur(24px);border-bottom:1px solid var(--border);height:72px;display:flex;align-items:center;}
.nav-inner{width:100%;max-width:1200px;margin:0 auto;padding:0 1.5rem;display:flex;justify-content:space-between;align-items:center;}
.logo{font-family:'Syne',sans-serif;font-weight:800;font-size:1.4rem;background:var(--grad);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;text-decoration:none;}
.nav-links{display:flex;list-style:none;gap:2rem;align-items:center;}
.nav-links a{color:var(--muted);text-decoration:none;font-weight:500;font-size:0.9rem;transition:color .2s;}
.nav-links a:hover{color:var(--white);}
.nav-cta{background:var(--grad)!important;color:white!important;padding:.55rem 1.4rem;border-radius:100px;font-weight:600!important;font-size:.875rem!important;box-shadow:0 4px 20px rgba(245,158,11,.25);transition:transform .2s,box-shadow .2s!important;}
.nav-cta:hover{transform:translateY(-1px);box-shadow:0 8px 28px rgba(245,158,11,.35)!important;}

/* HAMBURGER */
.hamburger{display:none;flex-direction:column;justify-content:center;gap:5px;width:40px;height:40px;background:none;border:none;cursor:pointer;padding:6px;}
.hamburger span{display:block;width:100%;height:2px;background:var(--white);border-radius:2px;transition:all .3s ease;transform-origin:center;}
.hamburger.open span:nth-child(1){transform:translateY(7px) rotate(45deg);}
.hamburger.open span:nth-child(2){opacity:0;transform:scaleX(0);}
.hamburger.open span:nth-child(3){transform:translateY(-7px) rotate(-45deg);}

/* MOBILE MENU */
.mobile-menu{display:none;position:fixed;top:72px;left:0;right:0;bottom:0;background:rgba(8,8,16,.98);backdrop-filter:blur(24px);z-index:998;flex-direction:column;align-items:center;justify-content:center;gap:2.5rem;}
.mobile-menu.open{display:flex;}
.mobile-menu a{color:var(--white);text-decoration:none;font-family:'Syne',sans-serif;font-size:2rem;font-weight:700;transition:opacity .2s;}
.mobile-menu a:hover{opacity:.6;}
.mob-cta{background:var(--grad);padding:1rem 3rem!important;border-radius:100px;font-size:1.1rem!important;}

/* HERO */
.hero{min-height:100vh;display:flex;align-items:center;padding:100px 1.5rem 60px;position:relative;overflow:hidden;}
.hero-glow-1{position:absolute;width:600px;height:600px;border-radius:50%;background:radial-gradient(circle,rgba(245,158,11,.12) 0%,transparent 70%);top:-100px;left:-100px;pointer-events:none;}
.hero-glow-2{position:absolute;width:500px;height:500px;border-radius:50%;background:radial-gradient(circle,rgba(139,92,246,.1) 0%,transparent 70%);bottom:-50px;right:-50px;pointer-events:none;}
.hero-inner{max-width:1200px;margin:0 auto;width:100%;display:grid;grid-template-columns:1fr 420px;gap:4rem;align-items:center;position:relative;z-index:1;}
.hero-badge{display:inline-flex;align-items:center;gap:.5rem;background:rgba(245,158,11,.1);border:1px solid rgba(245,158,11,.25);color:var(--amber);padding:.45rem 1rem;border-radius:100px;font-size:.8rem;font-weight:600;letter-spacing:.06em;text-transform:uppercase;margin-bottom:1.75rem;}
.hero-badge .dot{width:7px;height:7px;border-radius:50%;background:var(--amber);animation:pulse 2s infinite;}
@keyframes pulse{0%,100%{box-shadow:0 0 0 0 rgba(245,158,11,.4);}50%{box-shadow:0 0 0 6px rgba(245,158,11,0);}}
.hero-title{font-family:'Syne',sans-serif;font-size:clamp(2.6rem,5.5vw,4.5rem);font-weight:800;line-height:1.05;letter-spacing:-.03em;margin-bottom:1.5rem;color:var(--white);}
.hero-title span{background:var(--grad);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;}
.hero-sub{font-size:1.1rem;color:var(--muted);max-width:480px;margin-bottom:2.5rem;font-weight:400;line-height:1.75;}
.hero-btns{display:flex;gap:1rem;flex-wrap:wrap;}
.btn-primary{background:var(--grad);color:white;padding:.9rem 2.2rem;border-radius:100px;font-weight:600;text-decoration:none;font-size:.95rem;transition:transform .2s,box-shadow .2s;box-shadow:0 6px 24px rgba(245,158,11,.3);white-space:nowrap;}
.btn-primary:hover{transform:translateY(-2px);box-shadow:0 12px 32px rgba(245,158,11,.4);}
.btn-ghost{color:var(--white);padding:.9rem 2.2rem;border-radius:100px;font-weight:600;text-decoration:none;font-size:.95rem;border:1.5px solid var(--border);transition:border-color .2s,background .2s;white-space:nowrap;}
.btn-ghost:hover{border-color:rgba(255,255,255,.25);background:rgba(255,255,255,.05);}

/* HERO PHOTO */
.hero-photo-wrap{position:relative;display:flex;justify-content:center;align-items:center;}
.hero-photo-ring{position:relative;width:340px;height:340px;}
.hero-photo-ring::before{content:'';position:absolute;inset:-3px;border-radius:50%;background:var(--grad);animation:spin 8s linear infinite;z-index:0;}
@keyframes spin{to{transform:rotate(360deg);}}
.hero-photo-ring::after{content:'';position:absolute;inset:2px;border-radius:50%;background:var(--bg);z-index:1;}
.hero-photo{position:absolute;inset:8px;border-radius:50%;overflow:hidden;z-index:2;animation:floaty 6s ease-in-out infinite;}
.hero-photo img{width:100%;height:100%;object-fit:cover;display:block;}
@keyframes floaty{0%,100%{transform:translateY(0);}50%{transform:translateY(-12px);}}
.hero-badge-float{position:absolute;z-index:3;background:var(--card);border:1px solid var(--border);border-radius:16px;padding:.75rem 1.1rem;display:flex;align-items:center;gap:.6rem;font-size:.82rem;font-weight:600;backdrop-filter:blur(12px);box-shadow:0 8px 32px rgba(0,0,0,.4);white-space:nowrap;}
.badge-f1{bottom:10px;left:-30px;color:var(--amber);}
.badge-f2{top:20px;right:-20px;color:#34d399;}

/* SECTIONS */
.section{padding:90px 1.5rem;}
.container{max-width:1200px;margin:0 auto;}
.section-eyebrow{color:var(--amber);font-size:.78rem;font-weight:600;letter-spacing:.12em;text-transform:uppercase;margin-bottom:.75rem;}
.section-title{font-family:'Syne',sans-serif;font-size:clamp(2rem,4vw,3rem);font-weight:800;letter-spacing:-.025em;line-height:1.1;margin-bottom:1rem;color:var(--white);}
.section-desc{color:var(--muted);font-size:1.05rem;max-width:520px;line-height:1.75;}
.section-head-center{text-align:center;margin-bottom:4rem;}
.section-head-center .section-desc{margin:0 auto;}

/* SERVICES */
.services-bg{background:var(--surface);}
.services-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1.5rem;margin-top:3.5rem;}
.svc-card{background:var(--card);border:1px solid var(--border);border-radius:20px;padding:2.25rem;transition:transform .3s,border-color .3s,box-shadow .3s;position:relative;overflow:hidden;}
.svc-card::after{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:var(--grad);transform:scaleX(0);transform-origin:left;transition:transform .3s;}
.svc-card:hover{transform:translateY(-8px);border-color:rgba(245,158,11,.2);box-shadow:0 24px 48px rgba(0,0,0,.35);}
.svc-card:hover::after{transform:scaleX(1);}
.svc-icon{width:56px;height:56px;border-radius:14px;background:rgba(245,158,11,.1);display:flex;align-items:center;justify-content:center;font-size:1.4rem;color:var(--amber);margin-bottom:1.5rem;}
.svc-card h3{font-family:'Syne',sans-serif;font-size:1.2rem;font-weight:700;margin-bottom:.75rem;color:var(--white);}
.svc-card p{color:var(--muted);font-size:.92rem;line-height:1.7;margin-bottom:1.5rem;}
.tags{display:flex;flex-wrap:wrap;gap:.4rem;}
.tag{background:rgba(139,92,246,.1);color:#a78bfa;padding:.2rem .8rem;border-radius:100px;font-size:.75rem;font-weight:500;}

/* PORTFOLIO */
.portfolio-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1.5rem;margin-top:3.5rem;}
.port-card{background:var(--card);border:1px solid var(--border);border-radius:20px;overflow:hidden;transition:transform .3s,box-shadow .3s,border-color .3s;}
.port-card:hover{transform:translateY(-6px);box-shadow:0 24px 48px rgba(0,0,0,.4);border-color:rgba(245,158,11,.2);}
.port-thumb{height:180px;display:flex;align-items:center;justify-content:center;font-size:3rem;position:relative;background:linear-gradient(135deg,#12121f 0%,#1a1a30 100%);}
.port-thumb-overlay{position:absolute;inset:0;background:var(--grad);opacity:.07;}
.port-body{padding:1.75rem;}
.port-badge{display:inline-block;background:rgba(245,158,11,.1);color:var(--amber);font-size:.72rem;font-weight:600;letter-spacing:.07em;text-transform:uppercase;padding:.25rem .85rem;border-radius:100px;margin-bottom:.85rem;border:1px solid rgba(245,158,11,.2);}
.port-body h3{font-family:'Syne',sans-serif;font-size:1.1rem;font-weight:700;margin-bottom:.6rem;color:var(--white);}
.port-body p{color:var(--muted);font-size:.88rem;line-height:1.65;}

/* STATS */
.stats-section{background:var(--surface);}
.stats-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:1.5rem;}
.stat-card{background:var(--card);border:1px solid var(--border);border-radius:20px;padding:2.5rem 1.5rem;text-align:center;transition:transform .3s,border-color .3s;}
.stat-card:hover{transform:translateY(-4px);border-color:rgba(245,158,11,.2);}
.stat-num{font-family:'Syne',sans-serif;font-size:3rem;font-weight:800;line-height:1;margin-bottom:.5rem;background:var(--grad);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;}
.stat-label{color:var(--muted);font-size:.9rem;font-weight:500;}

/* CONTACT */
.contact-wrap{background:var(--card);border:1px solid var(--border);border-radius:28px;padding:4rem 3rem;position:relative;overflow:hidden;}
.contact-wrap::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;background:var(--grad);}
.contact-glow{position:absolute;width:400px;height:400px;background:radial-gradient(circle,rgba(245,158,11,.06) 0%,transparent 70%);top:-100px;right:-100px;pointer-events:none;}
.contact-inner{display:grid;grid-template-columns:1fr 1fr;gap:4rem;align-items:start;position:relative;z-index:1;}
.contact-left .section-desc{margin-bottom:2rem;}
.contact-cards{display:flex;flex-direction:column;gap:1rem;}
.contact-card{display:flex;align-items:center;gap:1rem;padding:1.25rem 1.5rem;background:rgba(255,255,255,.03);border:1px solid var(--border);border-radius:16px;text-decoration:none;color:var(--white);transition:all .25s;}
.contact-card:hover{background:rgba(245,158,11,.08);border-color:rgba(245,158,11,.25);transform:translateX(4px);}
.cc-icon{width:44px;height:44px;border-radius:12px;background:var(--grad);display:flex;align-items:center;justify-content:center;font-size:1.1rem;color:white;flex-shrink:0;}
.cc-text h4{font-size:.9rem;font-weight:600;margin-bottom:.15rem;}
.cc-text p{color:var(--muted);font-size:.82rem;}
.contact-right{display:flex;flex-direction:column;gap:1rem;}
.form-group{display:flex;flex-direction:column;gap:.5rem;}
.form-group label{font-size:.82rem;font-weight:500;color:var(--muted);}
.form-group input,.form-group textarea{background:rgba(255,255,255,.04);border:1px solid var(--border);border-radius:12px;padding:.85rem 1.1rem;color:var(--white);font-family:'DM Sans',sans-serif;font-size:.92rem;transition:border-color .2s,background .2s;outline:none;resize:none;}
.form-group input:focus,.form-group textarea:focus{border-color:rgba(245,158,11,.4);background:rgba(245,158,11,.04);}
.form-group input::placeholder,.form-group textarea::placeholder{color:var(--muted);}
.form-submit{background:var(--grad);color:white;border:none;cursor:pointer;padding:1rem;border-radius:12px;font-family:'DM Sans',sans-serif;font-size:.95rem;font-weight:600;transition:transform .2s,box-shadow .2s;box-shadow:0 4px 20px rgba(245,158,11,.25);}
.form-submit:hover{transform:translateY(-2px);box-shadow:0 8px 28px rgba(245,158,11,.35);}

/* FOOTER */
.footer{padding:2rem 1.5rem;border-top:1px solid var(--border);display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:1rem;max-width:100%;}
.footer p{color:var(--muted);font-size:.85rem;}
.footer-socials{display:flex;gap:1rem;}
.footer-socials a{width:36px;height:36px;border-radius:10px;background:var(--card);border:1px solid var(--border);display:flex;align-items:center;justify-content:center;color:var(--muted);font-size:.9rem;text-decoration:none;transition:all .2s;}
.footer-socials a:hover{color:var(--amber);border-color:rgba(245,158,11,.3);}

/* REVEAL */
.reveal{opacity:0;transform:translateY(32px);transition:opacity .7s ease,transform .7s ease;}
.reveal.active{opacity:1;transform:translateY(0);}

/* SCROLLBAR */
::-webkit-scrollbar{width:6px;}
::-webkit-scrollbar-track{background:var(--bg);}
::-webkit-scrollbar-thumb{background:var(--amber);border-radius:3px;}

/* ── TABLET ── */
@media(max-width:1024px){
  .services-grid,.portfolio-grid{grid-template-columns:1fr 1fr;}
  .stats-grid{grid-template-columns:1fr 1fr;}
  .contact-inner{grid-template-columns:1fr;gap:2.5rem;}
  .hero-photo-ring{width:280px;height:280px;}
  .badge-f1{left:-10px;}
  .badge-f2{right:-10px;}
}

/* ── MOBILE ── */
@media(max-width:768px){
  .nav-links{display:none;}
  .hamburger{display:flex;}

  .hero{padding:90px 1.25rem 50px;min-height:auto;}
  .hero-inner{grid-template-columns:1fr;text-align:center;gap:2.5rem;}
  .hero-sub{margin:0 auto 2.5rem;}
  .hero-btns{justify-content:center;}
  .hero-photo-wrap{order:-1;}
  .hero-photo-ring{width:220px;height:220px;}
  .badge-f1{bottom:-5px;left:0;font-size:.72rem;padding:.45rem .8rem;}
  .badge-f2{top:5px;right:0;font-size:.72rem;padding:.45rem .8rem;}

  .section{padding:60px 1.25rem;}
  .section-head-center{margin-bottom:2.5rem;}
  .services-grid,.portfolio-grid{grid-template-columns:1fr;gap:1rem;}
  .stats-grid{grid-template-columns:1fr 1fr;gap:1rem;}

  .contact-wrap{padding:2rem 1.25rem;}
  .contact-inner{grid-template-columns:1fr;gap:2rem;}

  .footer{flex-direction:column;text-align:center;}
  .stat-card{padding:1.75rem 1rem;}
  .stat-num{font-size:2.4rem;}
}

@media(max-width:400px){
  .hero-title{font-size:2.2rem;}
  .btn-primary,.btn-ghost{padding:.8rem 1.6rem;font-size:.88rem;}
  .hero-photo-ring{width:190px;height:190px;}
  .badge-f1,.badge-f2{display:none;}
}
</style>
</head>
<body>

<nav class="nav">
  <div class="nav-inner">
    <a href="#" class="logo">ReyRosal</a>
    <ul class="nav-links">
      <li><a href="#services">Services</a></li>
      <li><a href="#portfolio">Work</a></li>
      <li><a href="#stats">Results</a></li>
      <li><a href="#contact">Contact</a></li>
      <li><a href="mailto:rosalrey143@gmail.com" class="nav-cta">Hire Me</a></li>
    </ul>
    <button class="hamburger" id="hamburger" aria-label="Menu">
      <span></span><span></span><span></span>
    </button>
  </div>
</nav>

<div class="mobile-menu" id="mobileMenu">
  <a href="#services" class="mob-link">Services</a>
  <a href="#portfolio" class="mob-link">Work</a>
  <a href="#stats" class="mob-link">Results</a>
  <a href="#contact" class="mob-link">Contact</a>
  <a href="mailto:rosalrey143@gmail.com" class="mob-cta mob-link">Hire Me →</a>
</div>

<section class="hero">
  <div class="hero-glow-1"></div>
  <div class="hero-glow-2"></div>
  <div class="hero-inner">
    <div>
      <div class="hero-badge">
        <span class="dot"></span>
        Available for Projects
      </div>
      <h1 class="hero-title">
        GoHighLevel<br>
        <span>Expert &</span><br>
        Automation Pro
      </h1>
      <p class="hero-sub">
        I build conversion-focused GHL funnels, automated workflows, and client systems that scale your business — without the technical headache.
      </p>
      <div class="hero-btns">
        <a href="#contact" class="btn-primary">Start Your Project →</a>
        <a href="#portfolio" class="btn-ghost">See My Work</a>
      </div>
    </div>
    <div class="hero-photo-wrap">
      <div class="hero-photo-ring">
        <div class="hero-photo">
          <img src="https://raw.githubusercontent.com/reyrosal123/reyrosal/930fd61035b6461478c04e118419ae3265e82847/image.png" alt="Rey Rosal" />
        </div>
      </div>
      <div class="hero-badge-float badge-f2">
        <i class="fas fa-star"></i> 99.9% Satisfaction
      </div>
    </div>
  </div>
</section>

<section id="services" class="section services-bg">
  <div class="container">
    <div class="section-head-center reveal">
      <div class="section-eyebrow">What I Do</div>
      <h2 class="section-title">Services That Convert</h2>
      <p class="section-desc">End-to-end solutions for agencies and businesses using GoHighLevel and modern automation tools.</p>
    </div>
    <div class="services-grid">
      <div class="svc-card reveal">
        <div class="svc-icon"><i class="fas fa-rocket"></i></div>
        <h3>GHL Funnel Systems</h3>
        <p>Complete funnel builds — landing pages, upsells, order forms, and payment integrations that turn traffic into revenue.</p>
        <div class="tags"><span class="tag">Sales Funnels</span><span class="tag">A/B Testing</span><span class="tag">Stripe</span></div>
      </div>
      <div class="svc-card reveal">
        <div class="svc-icon"><i class="fas fa-cogs"></i></div>
        <h3>Workflow Automation</h3>
        <p>Smart automations with GHL, n8n, and Pabbly Connect — SMS sequences, email nurturing, and multi-platform integrations.</p>
        <div class="tags"><span class="tag">n8n</span><span class="tag">Pabbly</span><span class="tag">Lead Routing</span></div>
      </div>
      <div class="svc-card reveal">
        <div class="svc-icon"><i class="fas fa-globe"></i></div>
        <h3>Client Portals</h3>
        <p>SuiteDash and Lawcus implementations for seamless onboarding, document management, and client communication hubs.</p>
        <div class="tags"><span class="tag">SuiteDash</span><span class="tag">Lawcus CRM</span><span class="tag">White Label</span></div>
      </div>
    </div>
  </div>
</section>

<section id="portfolio" class="section">
  <div class="container">
    <div class="section-head-center reveal">
      <div class="section-eyebrow">Featured Projects</div>
      <h2 class="section-title">Real Results</h2>
      <p class="section-desc">Recent work for agencies, coaches, and professional services across multiple industries.</p>
    </div>
    <div class="portfolio-grid">
      <div class="port-card reveal">
        <div class="port-thumb"><i class="fas fa-dumbbell"></i><div class="port-thumb-overlay"></div></div>
        <div class="port-body">
          <div class="port-badge">GHL Sales Funnel</div>
          <h3>Fitness Coaching Funnel</h3>
          <p>Complete GHL funnel with quiz, VSL, 2-step tripwire, and 7-day nurture sequence — 247 qualified leads in the first month.</p>
        </div>
      </div>
      <div class="port-card reveal">
        <div class="port-thumb"><i class="fas fa-balance-scale"></i><div class="port-thumb-overlay"></div></div>
        <div class="port-body">
          <div class="port-badge">Lawcus Portal</div>
          <h3>Law Firm Client Portal</h3>
          <p>Custom Lawcus implementation with automated intake forms, document signing, and client communication dashboard.</p>
        </div>
      </div>
      <div class="port-card reveal">
        <div class="port-thumb"><i class="fas fa-home"></i><div class="port-thumb-overlay"></div></div>
        <div class="port-body">
          <div class="port-badge">WordPress + GHL</div>
          <h3>Real Estate Lead System</h3>
          <p>WordPress site integrated with GHL calendars, forms, and automated lead distribution to agent teams.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="stats" class="section stats-section">
  <div class="container">
    <div class="stats-grid">
      <div class="stat-card reveal"><div class="stat-num">24</div><div class="stat-label">Projects Delivered</div></div>
      <div class="stat-card reveal"><div class="stat-num">99.9%</div><div class="stat-label">Client Satisfaction</div></div>
      <div class="stat-card reveal"><div class="stat-num">48h</div><div class="stat-label">Avg. Response Time</div></div>
      <div class="stat-card reveal"><div class="stat-num">2+</div><div class="stat-label">Years Experience</div></div>
    </div>
  </div>
</section>

<section id="contact" class="section">
  <div class="container">
    <div class="contact-wrap reveal">
      <div class="contact-glow"></div>
      <div class="contact-inner">
        <div class="contact-left">
          <div class="section-eyebrow">Let's Build</div>
          <h2 class="section-title">Ready to Scale?</h2>
          <p class="section-desc">Whether you need a full GHL setup or targeted automation, I deliver results fast.</p>
          <br>
          <div class="contact-cards">
            <a href="mailto:rosalrey143@gmail.com" class="contact-card">
              <div class="cc-icon"><i class="fas fa-envelope"></i></div>
              <div class="cc-text"><h4>Email Me</h4><p>rosalrey143@gmail.com</p></div>
            </a>
            <a href="tel:+639533881141" class="contact-card">
              <div class="cc-icon"><i class="fab fa-whatsapp"></i></div>
              <div class="cc-text"><h4>WhatsApp / Call</h4><p>+63 953 388 1141</p></div>
            </a>
            <a href="https://github.com/reyrosal" class="contact-card" target="_blank">
              <div class="cc-icon"><i class="fab fa-github"></i></div>
              <div class="cc-text"><h4>GitHub</h4><p>github.com/reyrosal</p></div>
            </a>
          </div>
        </div>
        <div class="contact-right">
          <div class="form-group"><label>Your Name</label><input type="text" placeholder="John Smith" /></div>
          <div class="form-group"><label>Email Address</label><input type="email" placeholder="john@example.com" /></div>
          <div class="form-group"><label>What do you need?</label><input type="text" placeholder="GHL Funnel, Automation, Portal..." /></div>
          <div class="form-group"><label>Message</label><textarea rows="4" placeholder="Tell me about your project..."></textarea></div>
          <button class="form-submit" onclick="window.location.href='mailto:rosalrey143@gmail.com'">Send Message →</button>
        </div>
      </div>
    </div>
  </div>
</section>

<footer class="footer">
  <p>© 2025 Rey Rosal — GoHighLevel Expert · Dapitan City, Philippines</p>
  <div class="footer-socials">
    <a href="mailto:rosalrey143@gmail.com"><i class="fas fa-envelope"></i></a>
    <a href="tel:+639533881141"><i class="fab fa-whatsapp"></i></a>
    <a href="https://github.com/reyrosal" target="_blank"><i class="fab fa-github"></i></a>
  </div>
</footer>

<script>
const ham = document.getElementById('hamburger');
const mob = document.getElementById('mobileMenu');

ham.addEventListener('click', () => {
  ham.classList.toggle('open');
  mob.classList.toggle('open');
  document.body.style.overflow = mob.classList.contains('open') ? 'hidden' : '';
});

document.querySelectorAll('.mob-link').forEach(link => {
  link.addEventListener('click', () => {
    ham.classList.remove('open');
    mob.classList.remove('open');
    document.body.style.overflow = '';
  });
});

document.querySelectorAll('a[href^="#"]').forEach(a => {
  a.addEventListener('click', e => {
    e.preventDefault();
    const t = document.querySelector(a.getAttribute('href'));
    if (t) t.scrollIntoView({ behavior: 'smooth', block: 'start' });
  });
});

const io = new IntersectionObserver(entries => {
  entries.forEach(e => { if (e.isIntersecting) e.target.classList.add('active'); });
}, { threshold: 0.1, rootMargin: '0px 0px -40px 0px' });

document.querySelectorAll('.reveal').forEach(el => io.observe(el));
</script>
</body>
</html>
