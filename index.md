---
layout: page
title: Home
# Live app links
house_live:    https://new-london-house-price-pred.onrender.com
loan_live:     https://loan-default-predictor-45986ae9d37b.herokuapp.com
infl_live:     https://personal-inflation-impact.onrender.com
grocery_live:  https://uk-grocery-app.onrender.com
# Repo links (fill when ready)
house_repo:  https://github.com/Nas365/New_London_House_Price_Pred
loan_repo:  https://github.com/Nas365/loan-default-predictor
infl_repo:  https://github.com/Nas365/personal-inflation-impact
grocery_repo:  https://github.com/Nas365/uk-grocery-app
---

<!-- page-local styles -->
<style>
/* hide Minima’s header nav row and footer */
.site-nav { display:none !important; }
.site-footer { display:none !important; }

/* page layout */
.hero { display:flex; gap:18px; align-items:flex-start; margin: 0 0 10px; }
.hero img { width:120px; height:120px; border-radius:50%; object-fit:cover; }
.badge { display:inline-block; padding:4px 10px; border-radius:999px; background:#eef2ff; border:1px solid #c7d2fe; font-size:12px; margin:6px 6px 0 0; }
.meta a { color:#334155; text-decoration:underline; }
.grid { display:grid; grid-template-columns: repeat(auto-fit, minmax(280px,1fr)); gap:18px; }
.card { display:flex; flex-direction:column; border:1px solid #e5e7eb; border-radius:12px; padding:14px; background:#fff; }
.card img { width:100%; height:180px; object-fit:cover; border-radius:10px; margin-bottom:10px; }
.card p { margin:0 0 10px; }
.card .cta { margin-top:auto; }
.small { font-size:13px; color:#475569; }
h2 { margin-top:26px; }
.btn { display:inline-block; padding:6px 10px; border:1px solid #334155; border-radius:8px; text-decoration:none; }
.btn + .btn { margin-left:8px; }
</style>

<!-- PROFILE -->
<div class="hero">
  <!-- NOTE: your file is profile.png (not .jpg) -->
  <img src="{{ '/assets/images/profile.png' | relative_url }}" alt="Nasir Abubakar">
  <div>
    <h1 style="margin:0 0 6px 0;">Nasir Abubakar</h1>
    <div class="small" style="margin:0 0 8px 0;">
      Economist & Data Scientist · Oxford, UK.
    </div>
    <div class="meta small" style="line-height:1.7;">
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
      <span class="badge">CI/CD (GitHub Actions)</span>
      <span class="badge">Render / AWS</span>
      <span class="badge">Git</span>
      <span class="badge">R</span>
      <span class="badge">Econometrics</span>
    </div>
  </div>
</div>

---

## Background snapshot

**About.** Data Scientist with an Economics background, focused on turning real-world problems into practical ML solutions that solve real-world problems.

## Education
• MSc, International Economics, Finance & Development (Merit) — *University  of Surrey* (2020–2021)  
• MBA, Foreign Trade Management (A Grade) — *NIBM Global* (2020–2021)  
• BSc, Economics (First Class) — *Bauchi State University* (2013–2017)

## Awards
• Undergraduate — *Student of the Year* (2017) 
• Government Award — *Merit-Based Scholarship for Masters Degree* (2020)

## Certifications  
• DataCamp — *Associate Data Scientist in Python* (2025)  
• DataCamp — *Associate Data Analyst in SQL* (2024)  
• DataCamp — *Data Analyst in Python* (2024)  
• IBM — *Data Analytics with Excel & R* (2024)  
• IBM — *Introduction to Data Analytics* (2024)

## Experience highlights.
• **Head of Business Intelligence (Placement)**, *Kaduna Capital Territory Authority (KCTA)* — Mar 2022–Jun 2022  
• Enforced environmental compliance and coordinated waste management to improve urban cleanliness.
• Helped divide the city into operational lots, streamlining waste collection and boosting efficiency. 
• Led business licence registrations, strengthening the state’s commercial database and supporting record IGR growth (₦62.48bn in 2023; ₦14.16bn in Jan–Feb 2025). 
• Contributed to the Kaduna City Resilience Project, enhancing the city’s environmental and economic resilience.  

• **Department of Finance (Placement), Kaduna State Government** — 2022  
• Assisted with data entry, policy research, and financial records reconciliation. 
• Supported the analysis of budget implementation reports and helped prepare documentation for internal audits. 
• Worked alongside senior officers to gain practical exposure to public financial management and government accounting systems.

• **Research Assistant (Youth Servive)**, *Centre for the Study of the Economies of Africa (CSEA)* — Aug 2017–Jul 2018  
• Performed crucial data-related tasks to support CSEA’s research programs. •Conducted literature reviews to support senior researchers in building contextual understanding of development topics. 
• Carried out administrative and operational tasks as needed to support the research team and Director

---

## Featured Projects

<div class="grid">

<div class="card">
  <img src="{{ '/assets/images/p1_house.jpg' | relative_url }}" alt="London House Price Prediction">
  <h3 style="margin:6px 0;">1) London House Price Prediction</h3>
  <p class="small">
    The story begins with shelter: My first end-to-end ML project that estimates fair market prices for London properties using over 200 k records (Kaggle). 
    <strong>ML:</strong> XGBoost Regressor (outperformed LightGBM & Random Forest). 
    <strong>Stack:</strong> Python, scikit-learn, pandas, Flask; deployed on Render.
  </p>
  <p class="cta">
    <a class="btn" href="{{ page.house_live }}" target="_blank">Live</a>
    {% if page.house_repo %}<a class="btn" href="{{ page.house_repo }}" target="_blank">Repo</a>{% else %}<span class="small">repo coming soon</span>{% endif %}
  </p>
</div>

<div class="card">
  <img src="{{ '/assets/images/p2_loan.jpg' | relative_url }}" alt="Loan Default Predictor">
  <h3 style="margin:6px 0;">2) Loan Default Predictor</h3>
  <p class="small">
    While the first app was a regression problem, this one is a classification problem. Imagine using my first app to estimate the price of a house, and then approaching the bank for a loan. The bank could now use this app to decide whether you are likely to default on that loan or not.
    
    The project uses the Kaggle “Give Me Some Credit” dataset, features XGBoost as the final model, and has been built with Streamlit, containerized with Docker, and deployed on Heroku using GitHub Actions for CI/CD. 

   <strong>ML:</strong> compared models; <em>XGBoost</em> selected.<strong>Stack:</strong> Streamlit; Docker; GitHub Actions; Heroku.
  </p>
  <p class="cta">
    <a class="btn" href="{{ page.loan_live }}" target="_blank">Live</a>
    {% if page.loan_repo %}<a class="btn" href="{{ page.loan_repo }}" target="_blank">Repo</a>{% else %}<span class="small">repo coming soon</span>{% endif %}
  </p>
</div>

<div class="card">
  <img src="{{ '/assets/images/p3_inflation.jpg' | relative_url }}" alt="Personal Inflation Impact (UK)">
  <h3 style="margin:6px 0;">3) Personal Inflation Impact (UK)</h3>
  <p class="small">
    While the first project focused on predicting property prices across London and the second explored the likelihood of loan default, this new work extends the economic journey to the next stage — managing the cost of living once financial commitments like a mortgage are in place.

    After the Office for National Statistics (ONS) published its CPIH data on 17 September 2025, I became curious about how inflation affects people differently. As an Economist and Data Scientist, I wanted to understand the gap between the national inflation rate and what households actually experience in daily life.

    Inflation is often presented as a single national figure, but each household faces a unique mix of rising costs — food, housing, transport, health, and more. This project bridges that gap by estimating a household’s personal inflation rate and comparing it with the national average, helping users see whether their living costs rise faster or slower than the economy overall.
    
    The app uses official ONS CPIH data, allowing users to adjust their spending mix through sliders to reflect their household budget. It predicts the 3-month forward personal inflation rate and flags whether inflation risk is high or low relative to the national CPIH.
    Technically, it was built in Python using pandas, scikit-learn, and 
    
    LightGBM, integrated into a unified FastAPI + NiceGUI interface. Deployment was automated via GitHub Actions and hosted on Render, following the same CI/CD principles used in earlier projects. The dataset comes directly from the Office for National Statistics CPIH Divisional Index, ensuring accuracy and credibility.
    
  
   <strong>Data:</strong> official <em>ONS CPIH</em>.  
   <strong>ML:</strong> time-aware regression with <em>LightGBM</em>; risk flag vs CPIH.  
   <strong>Stack:</strong> FastAPI + NiceGUI; Render; CI/CD.
  </p>
  <p class="cta">
    <a class="btn" href="{{ page.infl_live }}" target="_blank">Live</a>
    {% if page.infl_repo %}<a class="btn" href="{{ page.infl_repo }}" target="_blank">Repo</a>{% else %}<span class="small">repo coming soon</span>{% endif %}
  </p>
</div>

<div class="card">
  <img src="{{ '/assets/images/p4_grocery.jpg' | relative_url }}" alt="UK Grocery Price Recommender">
  <h3 style="margin:6px 0;">4) UK Grocery Price Recommender (Tesco vs Sainsbury’s)</h3>
  <p class="small">
    After using the previous Machine Learning App to assess how I am personally going to be affected by inflation, the next question is how do I spend smarter on food now? 
    
    To spend smartly, I scraped real product listings from Tesco & Sainsbury’s (captured Nov 2025) and built an app that finds cheaper, similar alternatives across both retailers. Choose a category (pasta, cereals, cooking oil, rice, tinned tomatoes), optionally pick a brand and size, and the app shows where it’s cheaper and the % saving.

    Under the hood (brief): TF-IDF on product names → KMeans clusters for comparable SKUs → cosine similarity for look-alikes → price normalisation (per kg/L), size filters, and “cheapest retailer” logic. Served via FastAPI with GitHub Actions CI/CD and deployed on Render.
    
   <strong>ML:</strong> TF-IDF + cosine similarity, KMeans clusters, price rules.  
   <strong>Stack:</strong> FastAPI + Jinja; Render; CI/CD.
  </p>
  <p class="cta">
    <a class="btn" href="{{ page.grocery_live }}" target="_blank">Live</a>
    {% if page.grocery_repo %}<a class="btn" href="{{ page.grocery_repo }}" target="_blank">Repo</a>{% else %}<span class="small">repo coming soon</span>{% endif %}
  </p>
</div>

</div>

---

<div class="small">
<strong>Notes & privacy.</strong> No personal data is stored in any app; requests are only used to serve results.<br>
<strong>Data sources.</strong> Grocery prices come from captured retailer pages on the stated dates and may be outdated—always verify on retailer sites. Personal-inflation benchmarks use official <em>ONS CPIH</em>.
</div>
