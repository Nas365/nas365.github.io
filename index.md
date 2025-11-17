---
layout: page
title: " "   # empty on purpose – removes any automatic "Home" heading
# Live apps
house_live: https://new-london-house-price-pred.onrender.com
loan_live: https://loan-default-predictor-45986ae9d37b.herokuapp.com
infl_live: https://personal-inflation-impact.onrender.com
grocery_live: https://uk-grocery-app.onrender.com
# Repos (all public now → always show)
house_repo: https://github.com/Nas365/New_London_House_Price_Pred
loan_repo: https://github.com/Nas365/loan-default-predictor
infl_repo: https://github.com/Nas365/personal-inflation-impact
grocery_repo: https://github.com/Nas365/uk-grocery-app
---

<style>
  /* === HIDE EVERYTHING WE DON'T WANT === */
  .site-header, .site-nav, .site-footer, .page-heading { display:none !important; }

  /* === GENERAL PAGE STYLE === */
  body {
    margin: 50px auto;
    max-width: 860px;
    padding: 0 20px;
    line-height: 1.7;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
    color: #1f2937;
  }
  h1, h2, h3 { color: #111827; }

  /* === HERO SECTION (profile) === */
  .hero {
    display: flex;
    gap: 28px;
    align-items: flex-start;
    margin-bottom: 40px;
  }

  /* BIGGER PROFILE PHOTO – forced with !important */
  .hero img {
    width: 220px !important;
    height: 220px !important;
    border-radius: 50%;
    object-fit: cover;
    border: 4px solid #e5e7eb;
  }

  .badge {
    display: inline-block;
    padding: 5px 11px;
    border-radius: 999px;
    background: #eef2ff;
    border: 1px solid #c7d2fe;
    font-size: 13px;
    margin: 4px 6px 4px 0;
  }

  /* === PROJECTS – VERTICAL STACK === */
  .project-card {
    border: 1px solid #e5e7eb;
    border-radius: 14px;
    padding: 22px;
    margin-bottom: 32px;
    background: #fff;
  }

  /* BIGGER PROJECT IMAGES – taller + forced with !important */
  .project-card img {
    width: 100% !important;
    height: 340px !important;    /* increase this if you want even taller */
    object-fit: cover;
    border-radius: 10px;
    margin-bottom: 16px;
  }

  .project-card h3 {
    margin: 0 0 12px;
    font-size: 1.35rem;
  }
  .project-card p {
    margin: 0 0 16px;
    font-size: 15px;
    line-height: 1.65;
    white-space: pre-line;   /* respects your line breaks */
  }
  .btn {
    display: inline-block;
    padding: 9px 16px;
    border: 1.5px solid #334155;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 500;
    font-size: 14px;
  }
  .btn + .btn { margin-left: 12px; }
</style>

<!-- ==================== PROFILE ==================== -->
<div class="hero">
  <img src="/assets/images/profile.png" alt="Nasir Abubakar">
  <div>
    <h1>Nasir Abubakar</h1>
    <p style="margin:4px 0 12px; font-size:18px; color:#374151;">
      Economist & Data Scientist · Oxford, UK
    </p>
    <div style="line-height:1.8; margin-bottom:14px; font-size:15px;">
      <div><a href="mailto:nasirdansabo10@gmail.com">nasirdansabo10@gmail.com</a></div>
      <div><a href="https://github.com/Nas365" target="_blank">github.com/Nas365</a></div>
      <div><a href="https://www.linkedin.com/in/nasabu" target="_blank">linkedin.com/in/nasabu</a></div>
    </div>
    <div>
      <span class="badge">Python</span>
      <span class="badge">SQL</span>
      <span class="badge">Machine Learning</span>
      <span class="badge">FastAPI / Streamlit</span>
      <span class="badge">Docker</span>
      <span class="badge">CI/CD</span>
      <span class="badge">Render / AWS</span>
      <span class="badge">Git</span>
      <span class="badge">R</span>
      <span class="badge">Econometrics</span>
    </div>
  </div>
</div>

<h2>About</h2>
<p>Data Scientist with an Economics background, focused on turning real-world problems into practical ML solutions.</p>

<h2>Education</h2>
<ul>
  <li>MSc, International Economics, Finance & Development (Merit) — <em>University of Surrey</em> (2020–2021)</li>
  <li>MBA, Foreign Trade Management (A Grade) — <em>NIBM Global</em> (2020–2021)</li>
  <li>BSc, Economics (First Class) — <em>Bauchi State University</em> (2013–2017)</li>
</ul>

<h2>Awards</h2>
<ul>
  <li><strong>Undergraduate</strong> — Student of the Year (2017)</li>
  <li><strong>Government Award</strong> — Merit-Based Scholarship for Master’s Degree (2020)</li>
</ul>

<h2>Certifications</h2>
<ul>
  <li>DataCamp — Associate Data Scientist in Python (2025)</li>
  <li>DataCamp — Associate Data Analyst in SQL (2024)</li>
  <li>DataCamp — Data Analyst in Python (2024)</li>
  <li>IBM — Data Analytics with Excel & R (2024)</li>
  <li>IBM — Introduction to Data Analytics (2024)</li>
</ul>

<h2>Experience Highlights</h2>
<ul>
  <li><strong>Head of Business Intelligence (Placement)</strong>, Kaduna Capital Territory Authority (KCTA) — Mar–Jun 2022<br>
    • Enforced environmental compliance & waste management<br>
    • Divided city into operational lots → improved collection efficiency<br>
    • Led business licence registrations (supported record IGR growth)<br>
    • Contributed to Kaduna City Resilience Project</li>
  <li><strong>Department of Finance (Placement)</strong>, Kaduna State Government — 2022<br>
    • Data entry, policy research, financial records reconciliation<br>
    • Supported budget analysis and internal audit documentation</li>
  <li><strong>Research Assistant (NYSC)</strong>, Centre for the Study of the Economies of Africa (CSEA) — Aug 2017–Jul 2018<br>
    • Data collection, cleaning, literature reviews<br>
    • Supported senior researchers on development economics topics</li>
</ul>

<h2>Featured Projects</h2>

<div class="project-card">
  <img src="/assets/images/p1_house.jpg" alt="London House Price">
  <h3>1) London House Price Prediction</h3>
  <p>
My first end-to-end ML project — estimates fair London property prices using >200k records (Kaggle).
<strong>ML:</strong> XGBoost Regressor (beat LightGBM & Random Forest)
<strong>Stack:</strong> Python, scikit-learn, Flask → Render
  </p>
  <div>
    <a class="btn" href="{{ page.house_live }}" target="_blank">Live App</a>
    <a class="btn" href="{{ page.house_repo }}" target="_blank">GitHub Repo</a>
  </div>
</div>

<div class="project-card">
  <img src="/assets/images/p2_loan.jpg" alt="Loan Default">
  <h3>2) Loan Default Predictor</h3>
  <p>
Classification app to assess 90-day default risk (Kaggle “Give Me Some Credit”).
<strong>ML:</strong> XGBoost selected after full model comparison
<strong>Stack:</strong> Streamlit + Docker + GitHub Actions → Heroku
  </p>
  <div>
    <a class="btn" href="{{ page.loan_live }}" target="_blank">Live App</a>
    <a class="btn" href="{{ page.loan_repo }}" target="_blank">GitHub Repo</a>
  </div>
</div>

<div class="project-card">
  <img src="/assets/images/p3_inflation.jpg" alt="Personal Inflation">
  <h3>3) Personal Inflation Impact (UK)</h3>
  <p>
Forecasts your household inflation vs official ONS CPIH using your spending mix.
<strong>Data:</strong> Official ONS CPIH divisional indices
<strong>ML:</strong> LightGBM regression + risk flag
<strong>Stack:</strong> FastAPI + NiceGUI → Render (CI/CD)
  </p>
  <div>
    <a class="btn" href="{{ page.infl_live }}" target="_blank">Live App</a>
    <a class="btn" href="{{ page.infl_repo }}" target="_blank">GitHub Repo</a>
  </div>
</div>

<div class="project-card">
  <img src="/assets/images/p4_grocery.jpg" alt="Grocery Recommender">
  <h3>4) UK Grocery Price Recommender (Tesco vs Sainsbury’s)</h3>
  <p>
Scraped real listings (Nov 2025) → recommends cheaper like-for-like items.
<strong>ML:</strong> TF-IDF + cosine similarity, KMeans, price rules
<strong>Stack:</strong> FastAPI + Jinja → Render (CI/CD)
  </p>
  <div>
    <a class="btn" href="{{ page.grocery_live }}" target="_blank">Live App</a>
    <a class="btn" href="{{ page.grocery_repo }}" target="_blank">GitHub Repo</a>
  </div>
</div>

<p style="font-size:14px; color:#6b7280; margin-top:40px;">
  <strong>Notes & privacy:</strong> No personal data stored. All requests used only to serve results.<br>
  <strong>Data sources:</strong> Clearly stated in each project (Kaggle, ONS, captured retailer pages Nov 2025).
</p>
