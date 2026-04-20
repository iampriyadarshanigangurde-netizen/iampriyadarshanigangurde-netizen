<div align="right">
  <img src="https://github-readme-stats.vercel.app/api?username=iampriyadarshanigangurde&show_icons=true&hide_border=true&bg_color=0e0e10&title_color=6ee7b7&icon_color=a78bfa&text_color=888899"/>
</div>

# Priyadarshani Gangurde

Data scientist based in New Jersey. I've spent the last 6 years turning messy datasets into things that actually run in production — at Philips right now, previously Deloitte and Genpact.

Most of my work sits at the intersection of **healthcare analytics**, **ML engineering**, and increasingly, **LLM-powered tools**. I care a lot about model reliability, not just accuracy numbers.

Currently wrapping up a master's thesis at Fordham on detecting cyberattacks in medical IoT networks. It's been the most technically demanding thing I've done — and also the most interesting.

---

**reach me** &nbsp;·&nbsp; [iampriyadarshanigangurde@gmail.com](mailto:iampriyadarshanigangurde@gmail.com) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/darshani-pri-31b413403/)

---

## work I'm proud of

**IoMT intrusion detection** &nbsp;·&nbsp; *thesis, 2024–2025*
&nbsp;&nbsp;&nbsp;&nbsp;🏆 2nd prize, Fordham CIS Research Exhibition 2025

Built a protocol-aware classifier to catch network intrusions on medical IoT devices. The hard part wasn't accuracy — it was getting reliable recall on attack types that appear maybe 0.1% of the time. Balanced Random Forest ended up hitting 98% recall on rare MQTT and Spoofing attacks. Final model: 99.81% accuracy on 7.8M records across 48 features.

---

**customer segmentation + product recommendation** &nbsp;·&nbsp; *2025*

Worked through the whole stack on a 392K-transaction retail dataset: RFM scoring, K-Means clustering (landed on 4 segments, Silhouette 0.41), Market Basket Analysis via Apriori (filtered down from 1M+ rules), and a Neural Network recommender on top. Three separate recommendation engines, one per meaningful cluster.

---

**AI flashcard generator** &nbsp;·&nbsp; *2024 · published paper*

You paste a YouTube link, it gives you flashcards. The interesting engineering is in the middle: tiktoken chunking, LangChain orchestration, Gemini extraction, structured Q&A output via FastAPI. Built with a few teammates at Fordham — we wrote it up and got it through peer review.

---

**CO₂ emissions prediction** &nbsp;·&nbsp; *2023*

Compared Linear Regression (R² = 0.906) and Random Forest (R² = 0.973) on Canadian vehicle data. Less about the models, more about doing the full pipeline right — EDA, encoding transmission and fuel types, Z-score outlier removal, cross-validation, Plotly visuals for the stakeholder presentation.

---

## what I reach for

```
languages       Python, SQL, R

ml / dl         Scikit-learn, TensorFlow, PyTorch, XGBoost,
                LightGBM, Keras

mlops / cloud   AWS SageMaker, S3, Athena · Snowflake · Databricks
                MLflow · Docker · CI/CD

genai           LangChain · Vertex AI · Gemini API · FastAPI

viz             Tableau · Power BI · Plotly · Seaborn
```

---

## background

Currently at **Philips** (2024–present) — building predictive models on EHR data, NLP pipelines over clinical notes, and ML workflows on SageMaker.

Before that, **Deloitte** (2020–2023) — marketing analytics for large clients, churn prediction, lead scoring, BI dashboards in Tableau.

Before that, **Genpact** (2018–2020) — credit risk modeling, fraud detection, time-series forecasting in banking.

**Fordham University** — MS in Data Science, graduating May 2025.  
**Mumbai University** — BE in Computer Engineering, 2018.
