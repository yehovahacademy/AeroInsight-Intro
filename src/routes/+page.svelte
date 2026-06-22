<script>


</script>

<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css"
/>

<section class="hero">
  <div class="badge">
    <svg xmlns="http://www.w3.org/2000/svg" width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><path d="M4.5 12.5l8 -8a4.94 4.94 0 0 1 7 7l-8 8a4.94 4.94 0 0 1 -7 -7"/><path d="M8.5 8.5l7 7"/></svg>
    Real-time aviation intelligence
  </div>

  <h1>Where aviation meets <span class="accent">intelligence</span></h1>

  <p class="subtitle">
    AeroInsights gives you predictive flight analytics, live route data, and ML-powered delay forecasting — all in one dashboard.
  </p>


  <div class="stats">
    <div class="stat-card">
      <span class="stat-value">98.4%</span>
      <span class="stat-label">Prediction accuracy</span>
    </div>
    <div class="stat-card">
      <span class="stat-value">1,200+</span>
      <span class="stat-label">Routes tracked</span>
    </div>
    <div class="stat-card">
      <span class="stat-value">Live</span>
      <span class="stat-label">Data updates</span>
    </div>
  </div>
</section>


<div class= "Intro-paragraph">
<h1>Introduction to AeroInsight</h1>
<img src="logo.png" alt="logo-para"/>
<br><br>
  <p class="para-1">AeroInsight is an aviation analytics platform designed to transform complex flight and airport data into meaningful insights.</p>
   <p class="para-2">Through interactive dashboards, visualizations, and data-driven analysis, AeroInsight helps users explore airline performance, airport operations, flight trends, and key aviation metrics.</p> 
   <p class="para-3">Built with modern web technologies and analytics tools, it empowers smarter decision-making in the aviation industry.</p>
</div>
<br><br>

<div class="Why-us">
  <h1>Why Choose AeroInsight ?</h1>
  <div class="Why-Paragraph">
  <h1 class="vision-heading"><i class="fa-solid fa-eye"></i>
    Our Vision</h1>
    <p class="vision">
      Our vision is to make aviation data accessible, understandable, and impactful for everyone. AeroInsight aims to become a leading platform for aviation analytics by transforming complex datasets into meaningful insights that support innovation, efficiency, and growth within the aviation industry.
</p>
<br>
<h1 class="mission-heading"><i class="fa-solid fa-helmet-un"></i>
  Our Mission</h1>
<p class="mission">Our mission is to provide aviation professionals, researchers, and enthusiasts with a modern analytics platform that simplifies the exploration of flight operations, airport performance, airline trends, and passenger statistics through interactive visualizations and data-driven insights.
</p>
<br>
<h1 class="goal-heading"><i class="fa-solid fa-bullseye"></i>
  Our Goal</h1>
<p class="goal">Our goal is to empower users to make informed decisions using aviation data. By combining analytics, visualization, and emerging technologies, AeroInsight strives to help identify trends, improve operational understanding, and unlock new opportunities within the aviation ecosystem.
</p>
  </div>
</div>

<div class=""></div>



<style>
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700&family=Inter:wght@300;400;500;600;700&display=swap');

  .hero {
    padding: 5rem 2rem 4rem;
    text-align: center;
    border-bottom: 1px solid #e5e7eb;
    background-image:linear-gradient(
            rgba(0,0,0,0.6),
            rgba(0,0,0,0.6)
        ), url('/background.png');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    background-attachment: fixed;
    height: 50vh;
    border-radius: 12px;
  }

  .badge {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    background: #E6F1FB;
    color: #0C447C;
    font-size: 12px;
    font-weight: 500;
    padding: 5px 12px;
    border-radius: 999px;
    margin-bottom: 1.5rem;
  }

  h1 {
    font-size: 42px;
    font-weight: 500;
    color: whitesmoke;
    margin: 0 0 1rem;
    letter-spacing: -0.5px;
    line-height: 1.2;
    font-family: 'Orbitron',sans-serif;
  }

  .accent { color: whitesmoke; }

  .subtitle {
    font-size: 16px;
    color: whitesmoke;
    margin: 0 auto 2.5rem;
    max-width: 460px;
    line-height: 1.7;
  }

  .stats {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 12px;
    max-width: 520px;
    margin: 0 auto;
  }

  .stat-card {
    background: #f9fafb;
    border-radius: 8px;
    padding: 1rem;
    display: flex;
    flex-direction: column;
    gap: 4px;
  }

  .stat-value {
    font-size: 24px;
    font-weight: 500;
    color: #111827;
  }

  .stat-label {
    font-size: 12px;
    color: #6b7280;
  }

  @media (max-width: 480px) {
    h1 { font-size: 28px; }
    .stats { grid-template-columns: 1fr; max-width: 280px; }
  }


  .Intro-paragraph {
    padding: 4rem 2rem;
    max-width: 720px;
    margin: 0 auto;
    display: flex;
   flex-direction: column;
   align-items: center;
  }

  .Intro-paragraph img {
    width: 35%;
    height: 35%;
    border-radius: 50%;
  }

  .Intro-paragraph h1{
    text-align: center;
    color: black;
  }

  .para-1 {
    font-size: 22px;
    font-weight: 500;
    color: #111827;
    line-height: 1.8;
    margin: 0 0 1.5rem;
    justify-content: center;
    font-weight: 650;
  }

  .para-2 {
    font-size: 22px;
    color: #111827;
    line-height: 1.8;
    justify-content: center;
    font-weight: 650;
  }

  .para-3 {
    font-size: 22px;
    color: #111827;
    line-height: 1.8;
    margin: 0;
    font-weight: 650;
  }


  .Why-us {
    padding: 4rem 2rem;
    max-width: 860px;
    margin: 0 auto;

  }

  .Why-us > h1 {
    font-size: 45px;
    font-weight: 700;
    color: #111827;
    text-align: center;
    margin: 0 0 2.5rem;
  }

  .Why-Paragraph {
    display: inline_block;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.25rem;
  }


  .Why-Paragraph h1 {
    font-size: 25px;
    font-weight:800;
    color: #111827;
    gap: 8px;
    text-align: center;
    line-height: 1.4;
    justify-content: center;
    
  }

  .Why-Paragraph  h1 i {
    width: 40px;
    height: 40px;
    border-radius: 8px;
    align-items: center;
    justify-content: center;
    
  }

  .vision-heading i { background: #E6F1FB; color: #185FA5; }
  .mission-heading i { background: #E1F5EE; color: #0F6E56; }
  .goal-heading i { background: #EEEDFE; color: #534AB7; }

  .vision, .mission, .goal {
    font-size: 20px;
    color: black;
    line-height: 1.75;
    margin: 0;
  }

  @media (max-width: 640px) {
    .Why-Paragraph { grid-template-columns: 1fr; }
  }
</style>



