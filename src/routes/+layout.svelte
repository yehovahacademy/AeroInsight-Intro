<script></script>

<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css"
/>

<nav class="navbar">
  <a href="/" class="brand">
    <div class="logo-box-1">
      <!-- swap with your actual <img src="logo.png"> if preferred -->
      <img src="logo.png" alt="" aria-hidden="true" />
    </div>
    <span class="brand-name">AeroInsights</span>
  </a>

  <div class="nav-links">
    <a href="/">Home</a>
    <a href="/aboutus">About us</a>
    <a href="/features">Features</a>
    <a href="/contact">Contact</a>
  </div>

  <div class="nav-right">
    <a href="/dashboard" class="cta-btn">
      Dashboard
    </a>
  </div>
</nav>

<br><br>

<slot />

<footer class="footer">
  <div class="footer-grid">

    <div class="footer-brand">
      <div class="footer-logo">
        <div class="logo-box">
          <img src="logo.png" alt="AeroInsights logo" />
        </div>
        <span class="brand-name">AeroInsights</span>
      </div>
      <p class="tagline">Aviation prediction and analytics platform. Smarter decisions, powered by data.</p>
    </div>

    <div class="footer-col">
      <h3>Quick links</h3>
      <a href="/">Home</a>
      <a href="/aboutus">About us</a>
      <a href="/features">Features</a>
      <a href="/contact">Contact</a>
    </div>

    <div class="footer-col">
      <h3>Resources</h3>
      <a href="/documents">Documentation</a>
      <a href="/reports">Reports</a>
      <a href="/analytics">Analytics</a>
    </div>

    <div class="footer-col">
      <h3>Connect</h3>
      <a href="/" class="social-link">
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0 0 24 12c0-6.63-5.37-12-12-12z"/></svg>
        GitHub
      </a>
      <a href="/" class="social-link">
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 0 1-2.063-2.065 2.064 2.064 0 1 1 2.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
        LinkedIn
      </a>
      <a href="/" class="social-link">
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><rect width="20" height="16" x="2" y="4" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/></svg>
        Email
      </a>
    </div>

  </div>

  <div class="footer-bottom">
    <p>© 2026 AeroInsights. All rights reserved.</p>
    <p>Built with ♥ for aviation intelligence</p>
  </div>
</footer>

<style>
.navbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 1.5rem;
    height: 60px;
    background: #ffffff;
    border-bottom: 1px solid #e5e7eb;
  }

  .brand {
    display: flex;
    align-items: center;
    gap: 10px;
    text-decoration: none;
  }

  .logo-box-1 {
    width: 40px;
    height: 40px;
    border-radius: 8px;
    overflow: hidden;
    background: #185FA5;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .logo-box-1 img {
    width: 100%;
    height: 100%;
    object-fit: contain;
  }

  .brand-name {
    font-size: 16px;
    font-weight: 500;
    color: #111827;
    letter-spacing: -0.2px;
  }

  .nav-links {
    display: flex;
    align-items: center;
    gap: 4px;
  }

  .nav-links a {
    font-size: 14px;
    color: #6b7280;
    text-decoration: none;
    padding: 6px 12px;
    border-radius: 8px;
    transition: background 0.15s, color 0.15s;
  }

  .cta-btn {
    font-size: 14px;
    font-weight: 500;
    color: #ffffff;
    background: #185FA5;
    padding: 7px 16px;
    border-radius: 8px;
    text-decoration: none;
    transition: background 0.15s;
  }

  .cta-btn:hover {
    background: #0C447C;
  }

	 .footer {
    background: #f9fafb;
    border-top: 1px solid #e5e7eb;
    padding: 2.5rem 1.5rem 1.5rem;
  }

  .footer-grid {
    display: grid;
    grid-template-columns: 2fr 1fr 1fr 1fr;
    gap: 2rem;
    margin-bottom: 2rem;
  }

  .footer-brand { display: flex; flex-direction: column; gap: 10px; }

  .footer-logo { display: flex; align-items: center; gap: 10px; }

  .logo-box {
    width: 85px;
    height: 85px;
    border-radius: 8px;
    overflow: hidden;
    background: #185FA5;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .logo-box img { width: 100%; height: 100%; object-fit: contain; }

  .brand-name { font-size: 16px; font-weight: 500; color: #111827; }

  .tagline { font-size: 13px; color: #6b7280; line-height: 1.6; max-width: 220px; margin: 0; }

  .footer-col h3 {
    font-size: 12px;
    font-weight: 500;
    color: #111827;
    text-transform: uppercase;
    letter-spacing: 0.06em;
    margin: 0 0 12px;
  }

  .footer-col a {
    display: block;
    font-size: 14px;
    color: #6b7280;
    text-decoration: none;
    margin-bottom: 8px;
    transition: color 0.15s;
  }

  .footer-col a:hover { color: #111827; }

  .social-link {
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .footer-bottom {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding-top: 1.5rem;
    border-top: 1px solid #e5e7eb;
  }

  .footer-bottom p { font-size: 12px; color: #9ca3af; margin: 0; }

  @media (max-width: 640px) {
    .footer-grid { grid-template-columns: 1fr 1fr; }
    .footer-brand { grid-column: 1 / -1; }
  }

</style>