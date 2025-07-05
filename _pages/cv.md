---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

You can also download my CV as a PDF file: [Download CV]({{ site.baseurl }}/files/YipuXu_CV.pdf)

## Education

**Master of Information Technology**  
*Monash University, Clayton, Australia* (Jul 2024 - Present)  
- GPA: 80/100 (WAM)
- **Main Courses**: Foundations of Data Science (92/100, HD), Cloud Computing and Security (90/100, HD), IT Research Methods (86/100, HD), Advanced Database Technology (80/100, HD)

**Bachelor of Information Management and Information Systems**  
*Wenzhou Medical University, Zhejiang, China* (Sep 2019 - Jun 2023)  
- Average Score: 78.95/100

## Research Interests

- Urban Computing & Public Health Intelligence
- Intelligent Decision Support Systems
- Clinical Natural Language Processing (NLP)
- Human-AI Collaboration
- Machine Learning & Data Science

## Project Experience

### Urban Computing: Accessibility and Efficiency Analysis of Melbourne's Public Transport
*Urban Computing Researcher, Monash University, Clayton* (Current)

**Core Research**: Systematically evaluated the public transport network in Melbourne's Box Hill area by integrating PTV's GTFS data with ABS geographical dataset. Leveraged SQL and QGIS for in-depth spatial-temporal analysis.

**Methods & Implementation**: Developed a comprehensive accessibility scoring model to quantify service levels, precisely identifying unserved residential mesh blocks (>300m walking distance). This model also facilitated an efficiency assessment based on peak-hour passenger flow, service duration, and average waiting times.

**Key Findings & Impact**: Revealed the network's structural weaknesses, such as heavy reliance on buses and insufficient rail coverage. Pinpointed critical low-accessibility hotspots and long-wait bottlenecks, culminating in a set of data-driven optimization recommendations delivered to PTV to enhance service planning and equity.

### Machine Learning: Predictive Analysis of Chatbot Dialogue Utility
*Machine Learning Researcher, supervised by Guanliang Chen at Monash University, Clayton* (Current)

**Core Research**: Predicted the utility scores of human-chatbot interactions using machine learning techniques and analyzed key factors influencing dialogue quality.

**Methods & Implementation**: Preprocessed data using rule-based filtering and normalization, then engineered structural and semantic features (TF-IDF, PCA, LDA, SVD). Selected XGBoost as the core model, achieving over a 20% improvement in key metrics (RMSE/MAE) compared to baselines after hyperparameter tuning.

**Outcome**: Utilized SHAP for model interpretability, identifying the key conversational features that drive utility and providing actionable insights for enhancing dialogue quality.

### Environmental Data Science: Correlating Bushfires, Land Cover, and Agricultural Impact
*Data Analytics Researcher, supervised by Guanliang Chen at Monash University, Clayton* (Current)

**Core Research**: Investigated the complex correlations between wildfires and agricultural ecosystems (especially wheat production) by integrating diverse datasets (forestry, agriculture, meteorology, insurance).

**Methods & Implementation**: Cleaned and integrated datasets using R; employed EDA to confirm a significant positive correlation between fire frequency and forest/grassland coverage and identified a lagged negative impact of severe fire seasons on the following year's wheat yield.

**Outcome**: Developed linear regression and PCA models to quantify key factors and utilized a time-series approach, accounting for the "Black Summer" anomaly, to forecast future fire and agricultural trends.

## Internship Experience

### Hangzhou First People's Hospital  
*Hardware Engineer & Database Administrator, Hangzhou, China* (Jul 2022 - Apr 2023)

- Managed software/hardware maintenance, deployment, and troubleshooting for over 500 terminal devices across 20+ clinical and administrative departments
- Independently diagnosed and resolved an average of 25+ technical support tickets weekly, maintaining an average fault recovery time of under 2 hours and ensuring the stability of the HIS
- Executed over 1,000 data addition and modification requests in the database with a zero-error rate

## Research Experience

### AI Othello Game: Design and Implementation using Evaluation Functions & Game Tree Search
*Undergraduate Thesis Researcher, supervised by Prof. Wei Xu at Wenzhou Medical University, Zhejiang* (2023)

**Core Research**: Investigated the AI decision-making process in human-computer games, focusing on game tree search, heuristic evaluation functions, and strategic choices.

**Methods & Implementation**: Based on the Minimax principle, designed and implemented a composite heuristic evaluation function combining positional, mobility, and greedy strategies to guide AI decisions. Developed the complete system in C#, including data persistence.

## Technical Skills

**Programming Languages**: Python (Proficient), R (Proficient), C#, Java, JavaScript/TypeScript

**Data Science & Machine Learning**:
- **Frameworks & Libraries**: Scikit-learn, XGBoost, PyTorch, TensorFlow, Caret, Tidyverse, ggplot2
- **Algorithms**: Linear Regression, Random Forest, XGBoost, KNN, CNN, PCA, LDA, Clustering, Sequential Pattern Mining
- **NLP**: TF-IDF, Word Embeddings, Topic Modeling, SHAP (Model Interpretability)
- **Computer Vision**: Medical Image Processing

**Database Technologies**: SQL (Proficient), SQL Server, PostgreSQL/PostGIS, Oracle

**Cloud & Development**: AWS (Lambda, S3), ASP.NET, Vue, Node.js, Mobile & Distributed Systems, RESTful API Design

**Visualization Tools**: QGIS, Echarts, MATLAB, AntV, Tableau

**Methodologies & Design**: IT Project Management, Software Engineering, System Analysis & Design, UI/UX Design

## Awards

- **Third-class Scholarship** (2020)

## Language Skills

- **IELTS**: Overall 6.5 (Writing 7.0)
- **Chinese**: Native
- **English**: Proficient

---

*Last updated: {{ site.time | date: "%B %Y" }}*
