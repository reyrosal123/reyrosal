<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Rey Rosal — GoHighLevel Expert & Automation Specialist</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet" />
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<style>
  :root {
    --black: #0f0f23;
    --dark: #15152a;
    --darker: #1a1a2e;
    --gray: #2d2d44;
    --light-gray: #525289;
    --white: #f8fafc;
    --orange: #f59e0b;
    --orange-light: #fbbf24;
    --gradient: linear-gradient(135deg, #f59e0b 0%, #ef4444 50%, #8b5cf6 100%);
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  html { scroll-behavior: smooth; scroll-padding-top: 80px; }

  body {
    font-family: 'Inter', -apple-system, sans-serif;
    background: var(--black);
    color: var(--white);
    line-height: 1.65;
    overflow-x: hidden;
  }

  /* Navigation */
  .nav {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1000;
    background: rgba(15, 15, 35, 0.95);
    backdrop-filter: blur(20px);
    border-bottom: 1px solid rgba(255,255,255,0.08);
    padding: 1rem 0;
  }

  .nav-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 2rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .logo {
    font-size: 1.5rem;
    font-weight: 700;
    background: var(--gradient);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    text-decoration: none;
  }

  .nav-menu {
    display: flex;
    list-style: none;
    gap: 2rem;
    align-items: center;
  }

  .nav-link {
    color: var(--light-gray);
    text-decoration: none;
    font-weight: 500;
    font-size: 0.95rem;
    transition: color 0.3s ease;
    position: relative;
  }

  .nav-link:hover {
    color: var(--white);
  }

  .nav-link::after {
    content: '';
    position: absolute;
    bottom: -4px;
    left: 0;
    width: 0;
    height: 2px;
    background: var(--gradient);
    transition: width 0.3s ease;
  }

  .nav-link:hover::after {
    width: 100%;
  }

  .cta-button {
    background: var(--gradient);
    color: white;
    padding: 0.75rem 1.75rem;
    border-radius: 50px;
    font-weight: 600;
    text-decoration: none;
    font-size: 0.9rem;
    transition: all 0.3s ease;
    box-shadow: 0 4px 20px rgba(245, 158, 11, 0.3);
  }

  .cta-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 30px rgba(245, 158, 11, 0.4);
  }

  /* Hero */
  .hero {
    min-height: 100vh;
    display: flex;
    align-items: center;
    padding: 120px 2rem 4rem;
    position: relative;
    overflow: hidden;
  }

  .hero::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: radial-gradient(circle at 20% 80%, rgba(245, 158, 11, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(239, 68, 68, 0.08) 0%, transparent 50%);
    pointer-events: none;
  }

  .hero-container {
    max-width: 1200px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 4rem;
    align-items: center;
  }

  .hero-badge {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    background: rgba(245, 158, 11, 0.15);
    color: var(--orange);
    padding: 0.5rem 1.25rem;
    border-radius: 50px;
    font-size: 0.85rem;
    font-weight: 600;
    letter-spacing: 0.05em;
    margin-bottom: 2rem;
    border: 1px solid rgba(245, 158, 11, 0.3);
  }

  .hero-badge i { font-size: 1rem; }

  .hero-title {
    font-size: clamp(3rem, 6vw, 5rem);
    font-weight: 800;
    line-height: 1.1;
    margin-bottom: 1.5rem;
    background: linear-gradient(135deg, var(--white) 0%, #e2e8f0 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .hero-subtitle {
    font-size: 1.25rem;
    color: var(--light-gray);
    margin-bottom: 2.5rem;
    max-width: 500px;
    font-weight: 400;
  }

  .hero-buttons {
    display: flex;
    gap: 1.5rem;
    flex-wrap: wrap;
  }

  .btn-primary {
    background: var(--gradient);
    color: white;
    padding: 1rem 2.5rem;
    border-radius: 50px;
    font-weight: 600;
    text-decoration: none;
    font-size: 1rem;
    transition: all 0.3s ease;
    box-shadow: 0 4px 20px rgba(245, 158, 11, 0.3);
    border: none;
    cursor: pointer;
  }

  .btn-primary:hover {
    transform: translateY(-3px);
    box-shadow: 0 12px 40px rgba(245, 158, 11, 0.4);
  }

  .btn-secondary {
    color: var(--white);
    padding: 1rem 2.5rem;
    border-radius: 50px;
    font-weight: 600;
    text-decoration: none;
    font-size: 1rem;
    border: 2px solid rgba(255,255,255,0.2);
    transition: all 0.3s ease;
  }

  .btn-secondary:hover {
    border-color: var(--white);
    background: rgba(255,255,255,0.1);
  }

  .hero-image {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .hero-avatar {
    width: 300px;
    height: 300px;
    border-radius: 50%;
    background: var(--gradient);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    font-size: 4rem;
    font-weight: 800;
    color: white;
    box-shadow: 0 40px 80px rgba(245, 158, 11, 0.3);
    position: relative;
    animation: float 6s ease-in-out infinite;
  }

  @keyframes float {
    0%, 100% { transform: translateY(0px); }
    50% { transform: translateY(-10px); }
  }

  /* Sections */
  .section {
    padding: 100px 2rem;
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
  }

  .section-header {
    text-align: center;
    margin-bottom: 4rem;
  }

  .section-subtitle {
    color: var(--orange);
    font-size: 0.85rem;
    font-weight: 600;
    letter-spacing: 0.1em;
    margin-bottom: 1rem;
    text-transform: uppercase;
  }

  .section-title {
    font-size: clamp(2.5rem, 5vw, 4rem);
    font-weight: 800;
    line-height: 1.1;
    margin-bottom: 1rem;
    background: linear-gradient(135deg, var(--white) 0%, #e2e8f0 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .section-desc {
    font-size: 1.2rem;
    color: var(--light-gray);
    max-width: 600px;
    margin: 0 auto;
    font-weight: 400;
  }

  /* Services */
  .services-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
    gap: 2rem;
  }

  .service-card {
    background: rgba(21, 21, 42, 0.6);
    border: 1px solid rgba(255,255,255,0.08);
    border-radius: 24px;
    padding: 2.5rem;
    transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
    position: relative;
    overflow: hidden;
  }

  .service-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 4px;
    background: var(--gradient);
    transform: scaleX(0);
    transition: transform 0.4s ease;
  }

  .service-card:hover {
    transform: translateY(-12px);
    border-color: rgba(245, 158, 11, 0.3);
    box-shadow: 0 32px 64px rgba(0,0,0,0.3);
  }

  .service-card:hover::before {
    transform: scaleX(1);
  }

  .service-icon {
    width: 64px;
    height: 64px;
    border-radius: 16px;
    background: rgba(245, 158, 11, 0.15);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.5rem;
    margin-bottom: 1.5rem;
    color: var(--orange);
  }

  .service-card h3 {
    font-size: 1.5rem;
    font-weight: 700;
    margin-bottom: 1rem;
    color: var(--white);
  }

  .service-card p {
    color: var(--light-gray);
    font-size: 1rem;
    line-height: 1.7;
    margin-bottom: 1.5rem;
  }

  .service-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
  }

  .service-tag {
    background: rgba(82, 82, 137, 0.3);
    color: var(--light-gray);
    padding: 0.25rem 1rem;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 500;
  }

  /* Portfolio */
  .portfolio-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(380px, 1fr));
    gap: 2rem;
  }

  .portfolio-card {
    border-radius: 24px;
    overflow: hidden;
    background: rgba(21, 21, 42, 0.6);
    border: 1px solid rgba(255,255,255,0.08);
    transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
    position: relative;
  }

  .portfolio-card:hover {
    transform: translateY(-8px);
    border-color: rgba(245, 158, 11, 0.3);
    box-shadow: 0 32px 64px rgba(0,0,0,0.4);
  }

  .portfolio-image {
    height: 220px;
    background: linear-gradient(135deg, var(--gray) 0%, var(--darker) 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    font-size: 4rem;
  }

  .portfolio-image::after {
    content: '';
    position: absolute;
    inset: 0;
    background: var(--gradient);
    opacity: 0.1;
  }

  .portfolio-content {
    padding: 2rem;
  }

  .portfolio-type {
    display: inline-block;
    background: rgba(245, 158, 11, 0.15);
    color: var(--orange);
    padding: 0.25rem 1rem;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 600;
    letter-spacing: 0.05em;
    margin-bottom: 1rem;
    text-transform: uppercase;
  }

  .portfolio-title {
    font-size: 1.4rem;
    font-weight: 700;
    margin-bottom: 1rem;
    color: var(--white);
  }

  .portfolio-desc {
    color: var(--light-gray);
    font-size: 0.95rem;
    line-height: 1.6;
  }

  /* Stats */
  .stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 2rem;
    margin-top: 4rem;
  }

  .stat-item {
    text-align: center;
    padding: 2rem;
  }

  .stat-number {
    font-size: 3.5rem;
    font-weight: 800;
    background: var(--gradient);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    line-height: 1;
    margin-bottom: 0.5rem;
    display: block;
  }

  .stat-label {
    color: var(--light-gray);
    font-size: 1rem;
    font-weight: 500;
  }

  /* Contact */
  .contact-section {
    background: rgba(21, 21, 42, 0.6);
    border-radius: 32px;
    padding: 4rem 2rem;
    text-align: center;
    border: 1px solid rgba(255,255,255,0.08);
  }

  .contact-links {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1.5rem;
    margin: 3rem 0;
  }

  .contact-link {
    display: flex;
    align-items: center;
    gap: 1rem;
    padding: 1.5rem;
    background: rgba(45, 45, 68, 0.4);
    border-radius: 20px;
    text-decoration: none;
    color: var(--white);
    transition: all 0.3s ease;
    border: 1px solid rgba(255,255,255,0.08);
  }

  .contact-link:hover {
    background: rgba(245, 158, 11, 0.15);
    border-color: var(--orange);
    transform: translateY(-4px);
  }

  .contact-icon {
    width: 48px;
    height: 48px;
    background: var(--gradient);
    border-radius: 12px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.2rem;
    color: white;
  }

  .contact-info h4 {
    font-size: 1rem;
    font-weight: 600;
    margin-bottom: 0.25rem;
  }

  .contact-info p {
    color: var(--light-gray);
    font-size: 0.9rem;
  }

  /* Footer */
  .footer {
    padding: 2rem;
    text-align: center;
    color: var(--light-gray);
    font-size: 0.9rem;
    border-top: 1px solid rgba(255,255,255,0.08);
  }

  /* Mobile */
  @media (max-width: 768px) {
    .nav-menu { display: none; }
    .hero-container { grid-template-columns: 1fr; text-align: center; gap: 3rem; }
    .hero-avatar { width: 250px; height: 250px; font-size: 3rem; }
    .services-grid, .portfolio-grid { grid-template-columns: 1fr; }
    .stats-grid { grid-template-columns: 1fr 1fr; }
    .contact-links { grid-template-columns: 1fr; }
  }

  /* Scroll animations */
  .reveal {
    opacity: 0;
    transform: translateY(40px);
    transition: all 0.8s cubic-bezier(0.4, 0, 0.2, 1);
  }

  .reveal.active {
    opacity: 1;
    transform: translateY(0);
  }

  /* Custom scrollbar */
  ::-webkit-scrollbar {
    width: 8px;
  }

  ::-webkit-scrollbar-track {
    background: var(--dark);
  }

  ::-webkit-scrollbar-thumb {
    background: var(--orange);
    border-radius: 4px;
  }
</style>
</head>
<body>
  <!-- Navigation -->
  <nav class="nav">
    <div class="nav-container">
      <a href="#" class="logo">ReyRosal</a>
      <ul class="nav-menu">
        <li><a href="#services" class="nav-link">Services</a></li>
        <li><a href="#portfolio" class="nav-link">Work</a></li>
        <li><a href="#stats" class="nav-link">Stats</a></li>
        <li><a href="#contact" class="nav-link">Contact</a></li>
<li><a href="mailto:rosalrey143@gmail.com" class="cta-button">Get Started</a></li>      </ul>
    </div>
  </nav>

<!-- Hero -->
<section class="hero">
  <div class="hero-container">
    <div>
      <div class="hero-badge">
        <i class="fas fa-circle-check"></i>
        Available Now
      </div>
      <h1 class="hero-title">GoHighLevel Expert<br>Automation Specialist</h1>
      <p class="hero-subtitle">
        I build conversion-focused GHL funnels, automated workflows, and client systems 
        that scales your business without the technical complexity.
      </p>
      <div class="hero-buttons">
        <a href="#contact" class="btn-primary">Start Your Project</a>
        <a href="#portfolio" class="btn-secondary">View My Work</a>
      </div>
    </div>
    <div class="hero-image">
      <div class="hero-avatar">
        <img 
          src="https://raw.githubusercontent.com/reyrosal123/reyrosal/930fd61035b6461478c04e118419ae3265e82847/image.png" 
          alt="Rey Rosal" 
          style="width: 100%; height: 100%; object-fit: cover; border-radius: inherit;"
        />
      </div>
    </div>
  </div>
</section>

  <!-- Services -->
  <section id="services" class="section reveal">
    <div class="container">
      <div class="section-header">
        <div class="section-subtitle">What I Do</div>
        <h2 class="section-title">Services That Convert</h2>
        <p class="section-desc">End-to-end solutions for agencies and businesses using GoHighLevel and modern automation tools.</p>
      </div>
      <div class="services-grid">
        <div class="service-card reveal">
          <div class="service-icon">
            <i class="fas fa-rocket"></i>
          </div>
          <h3>GHL Funnel Systems</h3>
          <p>Complete funnel builds including landing pages, upsells, order forms, and payment integrations that turn traffic into revenue.</p>
          <div class="service-tags">
            <span class="service-tag">Sales Funnels</span>
            <span class="service-tag">A/B Testing</span>
            <span class="service-tag">Stripe Integration</span>
          </div>
        </div>
        <div class="service-card reveal">
          <div class="service-icon">
            <i class="fas fa-cogs"></i>
          </div>
          <h3>Workflow Automation</h3>
          <p>Smart automations with GHL, n8n, and Pabbly Connect. SMS sequences, email nurturing, and multi-platform integrations.</p>
          <div class="service-tags">
            <span class="service-tag">n8n Workflows</span>
            <span class="service-tag">Pabbly Connect</span>
            <span class="service-tag">Lead Routing</span>
          </div>
        </div>
        <div class="service-card reveal">
          <div class="service-icon">
            <i class="fas fa-globe"></i>
          </div>
          <h3>Client Portals</h3>
          <p>SuiteDash and Lawcus implementations for seamless client onboarding, document management, and communication hubs.</p>
          <div class="service-tags">
            <span class="service-tag">SuiteDash</span>
            <span class="service-tag">Lawcus CRM</span>
            <span class="service-tag">White Label</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Portfolio -->
  <section id="portfolio" class="section reveal">
    <div class="container">
      <div class="section-header">
        <div class="section-subtitle">Featured Projects</div>
        <h2 class="section-title">Real Results</h2>
        <p class="section-desc">Recent work for agencies, coaches, and professional services across multiple industries.</p>
      </div>
      <div class="portfolio-grid">
        <div class="portfolio-card reveal">
          <div class="portfolio-image">
            <i class="fas fa-dumbbell"></i>
          </div>
          <div class="portfolio-content">
            <div class="portfolio-type">GHL Sales Funnel</div>
            <h3>Fitness Coaching Funnel</h3>
            <p>Complete GHL funnel with quiz, video sales letter, 2-step tripwire, and 7-day nurture sequence. Generated 247 qualified leads in first month.</p>
          </div>
        </div>
        <div class="portfolio-card reveal">
          <div class="portfolio-image">
            <i class="fas fa-balance-scale"></i>
          </div>
          <div class="portfolio-content">
            <div class="portfolio-type">Lawcus Portal</div>
            <h3>Law Firm Client Portal</h3>
            <p>Custom Lawcus implementation with automated intake forms, document signing, and client communication dashboard.</p>
          </div>
        </div>
        <div class="portfolio-card reveal">
          <div class="portfolio-image">
            <i class="fas fa-home"></i>
          </div>
          <div class="portfolio-content">
            <div class="portfolio-type">WordPress + GHL</div>
            <h3>Real Estate Lead System</h3>
            <p>Custom WordPress site integrated with GHL calendars, forms, and automated lead distribution to agent teams.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Stats -->
  <section id="stats" class="section reveal">
    <div class="container">
      <div class="stats-grid">
        <div class="stat-item reveal">
          <span class="stat-number">24</span>
          <div class="stat-label">Projects Delivered</div>
        </div>
        <div class="stat-item reveal">
          <span class="stat-number">100%</span>
          <div class="stat-label">Client Satisfaction</div>
        </div>
        <div class="stat-item reveal">
          <span class="stat-number">48h</span>
          <div class="stat-label">Response Time</div>
        </div>
        <div class="stat-item reveal">
          <span class="stat-number">2+</span>
          <div class="stat-label">Years Experience</div>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact" class="section">
    <div class="container">
      <div class="contact-section reveal">
        <div class="section-header">
          <div class="section-subtitle">Let's Build</div>
          <h2 class="section-title">Ready to Get Started?</h2>
          <p class="section-desc">Whether you need a full GHL setup or targeted automation, I'm ready to deliver results.</p>
        </div>
        <div class="contact-links">
          <a href="mailto:rosalrey143@gmail.com" class="contact-link">
            <div class="contact-icon">
              <i class="fas fa-envelope"></i>
            </div>
            <div class="contact-info">
              <h4>Email Me</h4>
              <p>rosalrey143@gmail.com</p>
            </div>
          </a>
          <a href="tel:09533881141" class="contact-link">
            <div class="contact-icon">
              <i class="fas fa-phone"></i>
            </div>
            <div class="contact-info">
              <h4>Phone/WhatsApp</h4>
              <p>+63 953 3881 141</p>
            </div>
          </a>
          <a href="https://github.com/reyrosal" class="contact-link" target="_blank">
            <div class="contact-icon">
              <i class="fab fa-github"></i>
            </div>
            <div class="contact-info">
              <h4>GitHub</h4>
              <p>github.com/reyrosal</p>
            </div>
          </a>
        </div>
        <a href="mailto:rosalrey143@gmail.com" class="btn-primary">Send Message</a>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <p>&copy; 2025 Rey Rosal — GoHighLevel Expert. Dapitan City, Philippines.</p>
  </footer>

  <script>
    // Smooth scrolling
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
          target.scrollIntoView({
            behavior: 'smooth',
            block: 'start'
          });
        }
      });
    });

    // Scroll animations
    const observerOptions = {
      threshold: 0.1,
      rootMargin: '0px 0px -50px 0px'
    };

    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('active');
        }
      });
    }, observerOptions);

    document.querySelectorAll('.reveal').forEach(el => {
      observer.observe(el);
    });
  </script>
</body>
</html>
