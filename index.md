---
layout: page
title: Home
# Live app links
house_live:    https://new-london-house-price-pred.onrender.com
loan_live:     https://loan-default-predictor-45986ae9d37b.herokuapp.com
infl_live:     https://personal-inflation-impact.onrender.com
grocery_live:  https://uk-grocery-app.onrender.com
# Repo links (fill when ready)
house_repo:
loan_repo:
infl_repo:
grocery_repo:  https://github.com/Nas365/uk-grocery-app
---

<style>
.hero { display:flex; gap:18px; align-items:center; margin-bottom:10px; }
.hero img { width:120px; height:120px; border-radius:50%; object-fit:cover; }
.badge { display:inline-block; padding:4px 10px; border-radius:999px; background:#eef2ff; border:1px solid #c7d2fe; font-size:12px; margin-right:6px; }
.meta { color:#475569; margin:6px 0 14px; }
.grid { display:grid; grid-template-columns: repeat(auto-fit, minmax(260px,1fr)); gap:18px; }
.card { border:1px solid #e5e7eb; border-radius:12px; padding:14px; background:#fff; }
.card img { width:100%; border-radius:10px; margin-bottom:10px; }
.small { font-size:13px; color:#475569; }
h2 { margin-top:26px; }
.btn { display:inline-block; padding:6px 10px; border:1px solid #334155; border-radius:8px; text-decoration:none; }
.btn + .btn { margin-left:8px; }
</style>

<!-- PROFILE (keep images exactly under assets/images/ ) -->
<div class="hero">
  <img src="{{ '/assets/images/profile.jpg' | relative_url }}" alt="Nasir Abubakar">
  <div>
    <h1 style="margin:0;">Nasir Abubakar</h1>
    <div class="meta">
      Economist & Data Scientist · Abingdon-on-Thames, UK ·
      <a href="mailto:nasirdansabo10@gmail.com">nasirdansabo10@gmail.com</a> ·
      <a href="https://github.com/Nas365" target="_blank">github.com/Nas365</a> ·
      <a href="https://www.linkedin.com/in/nasabu" target="_blank">linkedin.com/in/nasabu</a>
    </div>
    <div>
      <span class="badge">Python</span>
      <span class="badge">SQL</span>
      <span class="badge">Machine Learning</span>
      <span class="badge">FastAPI / Streamlit</span>
      <span class="badge">Docker</span>
      <span class="badge">CI/CD (GitHub Actions)</span>
      <span class="badge">Render / AWS</span>
      <span class="badge">Econometrics</span>
    </div>
  </div>
</div>

**Everyday Economics — a practical ML series**

A four-app story mirroring real decisions:
1) **Find a fair price** (regression) →  
2) **Assess loan risk** (classification) →  
3) **Forecast personal inflation** (official ONS CPIH) →  
4) **Shop smarter** (real Tesco & Sainsbury’s product data).

---

## Background snapshot

**Education.** MSc, International Economics, Finance & Development (Merit) — University of Surrey ·  
MBA, Foreign Trade Management — NIBM Global (A Grade) ·  
BSc, Economics (First Class) — Bauchi State University.

**Certifications.** DataCamp — Associate Data Scientist in Python (2025) ·  
DataCamp — Associate Data Analyst in SQL (2024) ·  
IBM — Data Analytics with Excel & R (2024) ·  
IBM — Introduction to Data Analytics (2024).

**Experience highlights.** Head of Business Intelligence (Placement), KCTA — streamlined data-driven ops & licence registry improvements ·  
Department of Finance (Placement), Kaduna State Gov — budget analysis & internal audit support ·  
Research Assistant, CSEA — data & policy research analytics.

---

## Featured Projects

<div class="grid">

<div class="card">
  <img src="{{ '/assets/images/p1_house.jpg' | relative_url }}" alt="London House Price Prediction">
  <h3 style="margin:6px 0;">London House Price Prediction</h3>
  <p class="small">
  The journey starts with shelter: a regression app that estimates London property prices.<br>
  <strong>ML:</strong> baselines vs <em>Random Forest</em> (final).  
  <strong>Stack:</strong> Python, scikit-learn, pandas; Docker; AWS App Runner.
  </p>
  <p>
    <a class="btn" href="{{ page.house_live }}" target="_blank">Live</a>
    {% if page.house_repo %}<a class="btn" href="{{ page.house_repo }}" target="_blank">Code</a>{% else %}<span class="small">code coming soon</span>{% endif %}
  </p>
</div>

<div class="card">
  <img src="{{ '/assets/images/p2_loan.jpg' | relative_url }}" alt="Loan Default Predictor">
  <h3 style="margin:6px 0;">Loan Default Predictor</h3>
  <p class="small">
  After pricing a home, you seek financing: a classification app a lender could use to gauge risk.  
  <strong>ML:</strong> compared models; <em>XGBoost</em> selected.  
  <strong>Stack:</strong> Streamlit; Docker; GitHub Actions; Heroku.
  </p>
  <p>
    <a class="btn" href="{{ page.loan_live }}" target="_blank">Live</a>
    {% if page.loan_repo %}<a class="btn" href="{{ page.loan_repo }}" target="_blank">Code</a>{% else %}<span class="small">code coming soon</span>{% endif %}
  </p>
</div>

<div class="card">
  <img src="{{ '/assets/images/p3_inflation.jpg' | relative_url }}" alt="Personal Inflation Impact (UK)">
  <h3 style="margin:6px 0;">Personal Inflation Impact (UK)</h3>
  <p class="small">
  The day after the loan app, the ONS released CPIH data—so I built a tool to forecast a household’s personal inflation vs the national rate.  
  <strong>ML:</strong> time-aware regression with <em>LightGBM</em>; risk flag vs CPIH.  
  <strong>Data:</strong> <em>Official ONS CPIH</em>.  
  <strong>Stack:</strong> FastAPI + NiceGUI; Render; CI/CD.
  </p>
  <p>
    <a class="btn" href="{{ page.infl_live }}" target="_blank">Live</a>
    {% if page.infl_repo %}<a class="btn" href="{{ page.infl_repo }}" target="_blank">Code</a>{% else %}<span class="small">code coming soon</span>{% endif %}
  </p>
</div>

<div class="card">
  <img src="{{ '/assets/images/p4_grocery.jpg' | relative_url }}" alt="UK Grocery Price Recommender">
  <h3 style="margin:6px 0;">UK Grocery Price Recommender</h3>
  <p class="small">
  To spend smartly, I scraped real product listings from Tesco and Sainsbury’s and recommend like-for-like cheaper options.  
  <strong>ML:</strong> TF-IDF + cosine similarity; KMeans clusters; price rules.  
  <strong>Stack:</strong> FastAPI + Jinja; Render; CI/CD.
  </p>
  <p>
    <a class="btn" href="{{ page.grocery_live }}" target="_blank">Live</a>
    {% if page.grocery_repo %}<a class="btn" href="{{ page.grocery_repo }}" target="_blank">Code</a>{% else %}<span class="small">code coming soon</span>{% endif %}
  </p>
</div>

</div>

---

<div class="small">
<strong>Notes & privacy.</strong> No personal data is stored in any app; requests are used only to serve results.  
<strong>Data sources.</strong> Grocery prices come from captured retailer pages on the stated dates and may be outdated—always verify on retailer sites.  
Personal-inflation data and benchmarks use official <em>ONS CPIH</em> releases.
</div>
