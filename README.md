Martin James — ML Engineer · MLOps · Telecom Analytics
Nairobi, Kenya 🇰🇪 · LinkedIn · Email · @jeymartins2

Who I Am
I build end-to-end ML systems — from raw data to live production APIs with automated monitoring and retraining. My focus is telecom analytics, fraud detection, and MLOps pipelines built to survive in production.
Currently executing a 10-week self-directed MLOps project series covering churn prediction, real-time fraud detection, customer segmentation, revenue forecasting, propensity modelling, anomaly detection, customer lifetime value, pipeline automation, and cloud deployment — all built with industry-standard tools and pushed live to AWS.
🏆 Best Paper Award — Beijing Institute of Technology 2018 · 34 countries

"Data is like garbage. You'd better know what to do with it before it piles up."


Proven Results
AchievementDetail🎯99.72% fraud detection accuracy284,807 transactions · live API💰KES 29.6M revenue turnaroundData-driven business transformation📈95.25% accuracy — mobile price predictionProduction ML classification model📊87.55% R² — insurance premium predictionProduction regression model🚀20+ production ML projectsDeployed and documented

🟢 Live Now — Real-Time Fraud Detection API
XGBoost · scikit-learn · REST API · Render
Real-time transaction scoring — 99.72% accuracy on 284,807 transactions.
jsonPOST /predict
{ "transaction_amount": 450.0, "time": 3600 }

Response:
{ "fraud_probability": 0.923, "decision": "BLOCK" }
🌐 Live API Endpoint · 📁 View Repository

🔨 Week 2 upgrade in progress: Kafka streaming · Redis caching · Docker · PostgreSQL · Grafana monitoring


📅 10-Week MLOps Project Series
WeekProjectStackStatus01Churn Prediction PipelineXGBoost · Flask · Docker · PostgreSQL · Grafana🔨 In Progress02Real-Time Fraud Detection v2XGBoost · Kafka · Redis · Flask · Docker⏳ Week 203Customer SegmentationKMeans · PCA · PostgreSQL · Power BI⏳ Week 304Revenue and ARPU ForecastingProphet · ARIMA · PostgreSQL · Grafana⏳ Week 405Propensity ModellingXGBoost Multi-class · Flask · Docker⏳ Week 506Anomaly DetectionIsolation Forest · DBSCAN · Kafka⏳ Week 607Customer Lifetime ValueBG/NBD · RFM · Power BI⏳ Week 708MLOps Pipeline AutomationMLflow · Prefect · Evidently AI · GitHub Actions⏳ Week 809Cloud Deployment on AWSEC2 · RDS · ECR · Docker · HTTPS⏳ Week 910Portfolio CapstoneEverything · Unitel Telecom Use Case⏳ Week 10
Updated every Sunday. Each completed week: ✅ Complete · live link added.

🔨 Week 1 — Churn Prediction Pipeline
Goal: Predict which telecom customers will churn and rank them by revenue at risk so the retention team calls the right customers first.
Pipeline
StageDetail🏢 Business UnderstandingWho is churning? Cost of missing one churner? What action on a high score?🔍 EDA7,043 customers · 26% churn rate · class imbalance identified⚙️ Feature Engineeringtenure_group · charges_per_month · is_high_value🔧 PreprocessingLabelEncoder · SMOTE · train_test_split(stratify=y) 80/20🤖 Model TrainingLogistic Regression (baseline) → Random Forest (bagging) → XGBoost (winner)✅ Cross ValidationStratifiedKFold(5) · scoring=roc_auc · mean AUC + std📊 EvaluationAUC · Precision · Recall · F1 · Confusion Matrix · SHAP values🚀 DeploymentFlask API → Docker → PostgreSQL → Grafana monitoring💰 Business Outputpriority_score = churn_probability × ARPU
Feature Engineering
pythontenure_group      = pd.cut(tenure, bins=[0,12,24,72])   # new vs loyal customer
charges_per_month = TotalCharges / tenure                 # spending rate
is_high_value     = (MonthlyCharges > 80).astype(int)    # high revenue flag
priority_score    = churn_probability × ARPU              # who to call first

🔨 AUC, Precision and Recall scores will be updated on completion

📁 View Repository · 🌐 Live API · 📊 Grafana Dashboard

🛠️ Skills
💻 Programming and Data Science
<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="40" height="40" alt="Python"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/r/r-original.svg" width="40" height="40" alt="R"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" width="40" height="40" alt="SQL"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tensorflow/tensorflow-original.svg" width="40" height="40" alt="TensorFlow"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" width="40" height="40" alt="NumPy"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" width="40" height="40" alt="Pandas"/>
</p>
🚀 Deployment and Infrastructure
<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flask/flask-original.svg" width="40" height="40" alt="Flask"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/fastapi/fastapi-original.svg" width="40" height="40" alt="FastAPI"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" width="40" height="40" alt="Docker"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" width="40" height="40" alt="PostgreSQL"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redis/redis-original.svg" width="40" height="40" alt="Redis"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/apachekafka/apachekafka-original.svg" width="40" height="40" alt="Kafka"/>
</p>
☁️ Cloud and Automation
<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/amazonwebservices/amazonwebservices-original.svg" width="40" height="40" alt="AWS"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="40" height="40" alt="GitHub Actions"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/grafana/grafana-original.svg" width="40" height="40" alt="Grafana"/>
</p>
📊 Visualisation and BI
<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/matplotlib/matplotlib-original.svg" width="40" height="40" alt="Matplotlib"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original.svg" width="40" height="40" alt="Jupyter"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" width="40" height="40" alt="VSCode"/>
</p>

🎯 Core Competencies
AreaDetailMachine LearningFraud detection · churn prediction · ensemble methods · feature engineering · SHAPMLOpsEnd-to-end pipelines · Docker · Grafana monitoring · MLflow · auto-retrainingTelecom AnalyticsChurn · ARPU · CLV · propensity modelling · anomaly detection · segmentationData VisualisationExecutive dashboards · Power BI · Tableau · interactive analyticsStreamingReal-time scoring · Apache Kafka · Redis caching · sub-200ms latencyCloudAWS EC2 · RDS · ECR · HTTPS deployment · production-grade infrastructure

📊 GitHub Stats
Show Image
Show Image
Show Image

📁 Other Repositories
RepositoryDescriptionData-Science-PortfolioClassification · regression · fraud detection · churn · Python · scikit-learnml-learning-journeyStructured ML notebooks — EDA through model deploymentR-Studio-ProjectsStatistical analysis · ggplot2 · R Markdown

🎯 Goals
🎓 MSc Computer Science — Georgia Tech OMSCS — January 2027
Specialisation in Machine Learning · One of the world's top ranked online CS programmes
🌍 African Language NLP
Building Kiswahili AI models for low-resource African languages — one of my most important long-term projects · language preservation through AI · making technology accessible across Africa

🤝 Connect
Open to collaborating on African AI, telecom analytics, MLOps pipelines, and fraud detection systems.
📧 ngangam93@gmail.com · 🔗 LinkedIn · 🐦 @jeymartins2

Building in public · one complete project per week · no shortcuts
