<script>

</script>

<svelte:head>
  <title>About Us</title>
</svelte:head>

<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css"
/>

<div class="about-us-intro">
  <h1>About<span>Us</span></h1>
  <p class="para">
    AeroInsight is a modern aviation analytics platform that transforms aviation data into meaningful insights. Through interactive dashboards, visualizations, and analytical tools, we help users explore flight operations, airport performance, airline trends, and passenger traffic. Our mission is to make aviation data accessible, understandable, and valuable for researchers, professionals, and aviation enthusiasts alike.
  </p>
</div>

<div class="Tech-stack">
  <h1><i class="fa-solid fa-laptop"></i>
    Built - with Technologies</h1>
  <p>The technologies powering AeroInsight</p>

   <div class="stack-grid">
    <div class="stack-card svelte">
    <div class="stack-img">
      <img src="/svelte.png" alt="svelte">
     </div> 
      <div class="stack-info">
        <span class="stack-name">SvelteKit</span>
        <span class="stack-role">Frontend Framework</span>
      </div>
    </div>

    <div class="stack-card fastapi">
     <div class="stack-img">
      <img src="/fastapi.png" alt="fastapi"/>
     </div> 
      <div class="stack-info">
        <span class="stack-name">FastAPI</span>
        <span class="stack-role">Backend & REST API</span>
      </div>
    </div>

    <div class="stack-card matplotlib">
    <div class="stack-img">
      <img src="/matplotlib.png" alt="matplotlib"/>
      </div>
      <div class="stack-info">
        <span class="stack-name">Matplotlib & Seaborn</span>
        <span class="stack-role">Data Visualization</span>
      </div>
    </div>

      <div class="stack-card postgres">
      <div class="stack-img">
      <img src="/postgres.png" alt="postgres"/>
      </div>
      <div class="stack-info">
        <span class="stack-name">PostgreSQL</span>
        <span class="stack-role">Database</span>
      </div>
    </div>

     <div class="stack-card chartjs">
     <div class="stack-img">
      <img src="/charts.png" alt="charts"/>
      </div>
      <div class="stack-info">
        <span class="stack-name">Chart.js</span>
        <span class="stack-role">Interactive Visualizations</span>
      </div>
    </div>

    <div class="stack-card pandas">
    <div class="stack-img">
      <img src="/pandas.png" alt="pandas"/>
      </div>
      <div class="stack-info">
        <span class="stack-name">Pandas</span>
        <span class="stack-role">Data Processing</span>
      </div>
    </div>


</div>
</div>




<style>
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700&family=Inter:wght@300;400;500;600;700&display=swap');

.about-us-intro {
    padding: 4rem 2rem;
    max-width: 700px;
    margin: 0 auto;
    text-align: center;
  }

  .about-us-intro h1 {
    font-size: 36px;
    font-weight: 500;
    color: #111827;
    margin: 0 0 1.25rem;
    letter-spacing: -0.5px;
  }

  .about-us-intro h1 span {
    color: #185FA5;
    margin-left: 8px;
  }

  .about-us-intro h1::after {
    content: '';
    display: block;
    width: 40px;
    height: 3px;
    background: #185FA5;
    border-radius: 999px;
    margin: 1rem auto 0;
  }

  .para {
    font-size: 18px;
    color: black;
    line-height: 1.8;
    margin: 1.5rem auto 0;
    max-width: 580px;
    font-weight: 650;
    font-style: 'Orbitron',sans-serif;
  }

   .Tech-stack {
    padding: 4rem 2rem;
    max-width: 960px;
    margin: 0 auto;
  }

  .Tech-stack  h1 {
    font-size: 35px;
    font-weight: 700;
    color: #111827;
    text-align: center;
    margin: 0 0 0.5rem;
    letter-spacing: -0.3px;
  }

  .Tech-stack  p {
    font-size: 18px;
    color: black;
    text-align: center;
    margin: 0 0 2.5rem;
  }

  /* Grid becomes one unified bordered block */
 :global(.stack-grid) {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1px;
  border: 1px solid #e5e7eb;
  border-radius: 14px;
  overflow: hidden;
  background: #e5e7eb;
}

:global(.stack-card) {
  padding: 1.5rem;
  background: #ffffff;
  display: flex;
  align-items: center;
  gap: 14px;
}
  .stack-card:hover { background: #f9fafb; }

  .stack-img {
    width: 100px;
    height: 100px;
    border-radius: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    padding: 8px;
    box-sizing: border-box;
  }

  .stack-img img {
    width: 100px;
    height: 100px;
    object-fit: contain;
    border-radius: 10px;
    display:inline-block;
    align-items: center;
  justify-content: center;
  padding: 8px;
  box-sizing: border-box;
  }

  .stack-info { display: flex; flex-direction: column; gap: 3px; }

  .stack-name { font-size: 18px; font-weight: 700; color: #111827; text-align:center; }

  .stack-role { font-size: 16px; color: #6b7280; }

  /* Icon tint per technology */
  .svelte .stack-img    { background: #FFF0EB; }
  .fastapi .stack-img   { background: #E6F8F4; }
  .postgres .stack-img  { background: #E8F0FE; }
  .chartjs .stack-img   { background: #FFF8E6; }
  .matplotlib .stack-img { background: #F0EFFF; }
  .pandas .stack-img    { background: #E6F1FB; }

  @media (max-width: 640px) {
    .stack-grid { grid-template-columns: 1fr 1fr; }
  }

</style>