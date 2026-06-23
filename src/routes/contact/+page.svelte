<script>

</script>


<!-- src/routes/contact/+page.svelte -->
<svelte:head>
  <meta name="description" content="Connect with us. Email, phone, or LinkedIn." />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />
</svelte:head>

<div class="page">
  <!-- Background Elements -->
  <div class="bg-glow"></div>
  <div class="bg-grid"></div>

  <!-- Main Content -->
  <main class="content">
    <!-- Header -->
    <header class="header">
      <p class="overline">Contact</p>
      <h1 class="title">Let's <span class="accent">Connect</span></h1>
      <p class="subtitle">
        Reach out through any channel. We look forward to hearing from you.
      </p>
    </header>

    <!-- Contact Cards -->
    <div class="cards">
      <!-- Email -->
      <a href="mailto:hello@company.com" class="card">
        <div class="card-inner">
          <div class="icon-wrap email">
            <i class="fa-solid fa-at"></i>
          </div>
          <div class="card-body">
            <span class="card-label">Email</span>
            <span class="card-value">hello@admin05.com</span>
          </div>
          <div class="card-arrow">
            <i class="fa-solid fa-arrow-up-right"></i>
          </div>
        </div>
        <div class="card-shine"></div>
      </a>

      <!-- Phone -->
      <a href="tel:+15551234567" class="card">
        <div class="card-inner">
          <div class="icon-wrap phone">
            <i class="fa-solid fa-phone"></i>
          </div>
          <div class="card-body">
            <span class="card-label">Phone</span>
            <span class="card-value">+1 (555) 123-4567</span>
          </div>
          <div class="card-arrow">
            <i class="fa-solid fa-arrow-up-right"></i>
          </div>
        </div>
        <div class="card-shine"></div>
      </a>

      <!-- LinkedIn -->
      <a href="https://linkedin.com/company/yourcompany" target="_blank" rel="noopener noreferrer" class="card">
        <div class="card-inner">
          <div class="icon-wrap linkedin">
            <i class="fa-brands fa-linkedin-in"></i>
          </div>
          <div class="card-body">
            <span class="card-label">LinkedIn</span>
            <span class="card-value">AeroInsight</span>
          </div>
          <div class="card-arrow">
            <i class="fa-solid fa-arrow-up-right"></i>
          </div>
        </div>
        <div class="card-shine"></div>
      </a>
    </div>

    <!-- Footer -->
    <footer class="footer">
      <p>San Francisco, CA · Mon–Fri, 9AM–6PM PST</p>
    </footer>
  </main>
</div>

<style>

  /* ===== PAGE ===== */
  .page {
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    overflow: hidden;
    padding: 40px 24px;
  }

  /* ===== BACKGROUND ===== */
  .bg-glow {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 800px;
    height: 800px;
    background: radial-gradient(
      circle at center,
      rgba(56, 189, 248, 0.06) 0%,
      rgba(139, 92, 246, 0.04) 40%,
      transparent 70%
    );
    pointer-events: none;
  }

  .bg-grid {
    position: absolute;
    inset: 0;
    background-image:
      linear-gradient(rgba(255,255,255,0.015) 1px, transparent 1px),
      linear-gradient(90deg, rgba(255,255,255,0.015) 1px, transparent 1px);
    background-size: 60px 60px;
    mask-image: radial-gradient(ellipse at center, black 30%, transparent 70%);
    -webkit-mask-image: radial-gradient(ellipse at center, black 30%, transparent 70%);
    pointer-events: none;
  }

  /* ===== CONTENT ===== */
  .content {
    position: relative;
    z-index: 1;
    max-width: 520px;
    width: 100%;
    text-align: center;
  }

  /* ===== HEADER ===== */
  .header {
    margin-bottom: 48px;
    animation: fadeUp 0.8s ease forwards;
  }

  .overline {
    font-size: 11px;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.2em;
    color: #64748b;
    margin-bottom: 16px;
  }

  .title {
    font-size: clamp(2.5rem, 6vw, 3.5rem);
    font-weight: 700;
    letter-spacing: -0.03em;
    margin: 0 0 16px;
    line-height: 1.1;
  }

  .accent {
    background: linear-gradient(135deg, #38bdf8, #818cf8, #c084fc);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .subtitle {
    font-size: 1.0625rem;
    color: black;
    line-height: 1.6;
    margin: 0;
    max-width: 400px;
    margin-left: auto;
    margin-right: auto;
  }

  /* ===== CARDS ===== */
  .cards {
    display: flex;
    flex-direction: column;
    gap: 12px;
    margin-bottom: 48px;
  }

  .card {
    position: relative;
    display: block;
    text-decoration: none;
    color: inherit;
    background: rgba(255, 255, 255, 0.03);
    border: 1px solid rgba(255, 255, 255, 0.06);
    border-radius: 16px;
    padding: 1px;
    overflow: hidden;
    transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
    animation: fadeUp 0.8s ease forwards;
    opacity: 0;
  }

  .card:nth-child(1) { animation-delay: 0.15s; }
  .card:nth-child(2) { animation-delay: 0.25s; }
  .card:nth-child(3) { animation-delay: 0.35s; }

  .card:hover {
    background: rgba(255, 255, 255, 0.05);
    border-color: rgba(255, 255, 255, 0.1);
    transform: translateY(-2px);
    box-shadow:
      0 20px 40px rgba(0, 0, 0, 0.4),
      0 0 0 1px rgba(56, 189, 248, 0.1);
  }

  .card-inner {
    display: flex;
    align-items: center;
    gap: 20px;
    padding: 24px;
    position: relative;
    z-index: 1;
  }

  .icon-wrap {
    width: 52px;
    height: 52px;
    border-radius: 14px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 22px;
    flex-shrink: 0;
    transition: transform 0.4s ease;
  }

  .card:hover .icon-wrap {
    transform: scale(1.05);
  }

  .icon-wrap.email  {
    background: linear-gradient(135deg, rgba(8, 167, 235, 0.15), rgba(14, 165, 233, 0.1));
    color: black;
    box-shadow: 0 4px 20px rgba(56, 189, 248, 0.15);
  }

  .icon-wrap.phone {
    background: linear-gradient(135deg, rgba(34, 197, 94, 0.15), rgba(22, 163, 74, 0.1));
    color: #4ade80;
    box-shadow: 0 4px 20px rgba(34, 197, 94, 0.15);
  }

  .icon-wrap.linkedin {
    background: linear-gradient(135deg, rgba(59, 130, 246, 0.15), rgba(37, 99, 235, 0.1));
    color: #60a5fa;
    box-shadow: 0 4px 20px rgba(59, 130, 246, 0.15);
  }

  .card-body {
    flex: 1;
    text-align: left;
    display: flex;
    flex-direction: column;
    gap: 4px;
  }

  .card-label {
    font-size: 12px;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    color: #6b7280;
  }

  .card-value {
    font-size: 1.0625rem;
    font-weight: 500;
    color: black;
    letter-spacing: -0.01em;
  }

  .card-arrow {
    width: 36px;
    height: 36px;
    border-radius: 10px;
    background: rgba(255, 255, 255, 0.05);
    display: flex;
    align-items: center;
    justify-content: center;
    color: #6b7280;
    font-size: 13px;
    transition: all 0.3s ease;
    flex-shrink: 0;
  }

  .card:hover .card-arrow {
    background: rgba(56, 189, 248, 0.1);
    color: #38bdf8;
    transform: translate(2px, -2px);
  }

  /* Card Shine Effect */
  .card-shine {
    position: absolute;
    top: 0;
    left: -100%;
    width: 50%;
    height: 100%;
    background: linear-gradient(
      90deg,
      transparent,
      rgba(255, 255, 255, 0.03),
      transparent
    );
    transition: left 0.6s ease;
    pointer-events: none;
  }

  .card:hover .card-shine {
    left: 150%;
  }

  /* ===== FOOTER ===== */
  .footer {
    animation: fadeUp 0.8s ease 0.5s forwards;
    opacity: 0;
  }

  .footer p {
    font-size: 13px;
    color: #4b5563;
    letter-spacing: 0.02em;
  }

  /* ===== ANIMATIONS ===== */
  @keyframes fadeUp {
    from {
      opacity: 0;
      transform: translateY(20px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  /* ===== RESPONSIVE ===== */
  @media (max-width: 480px) {
    .page {
      padding: 32px 20px;
    }

    .card-inner {
      padding: 20px;
      gap: 16px;
    }

    .icon-wrap {
      width: 44px;
      height: 44px;
      font-size: 18px;
    }

    .card-value {
      font-size: 0.9375rem;
    }
  }
</style>




