# Awesome-Fraud-Analytics

# Top Fraud Analytics Platforms

A curated list of leading fraud analytics and detection platforms that combine machine learning, behavioral analytics, real-time scoring, case management, and network intelligence to identify and prevent financial crime, payment fraud, account takeover, and related risks.  
**Primary focus: open-source software.**

Commercial / hosted platforms are listed separately for completeness. Open-source alternatives and community tools are emphasized throughout.

---

## SaaS / Hosted Platforms

| Platform | Description | Key Focus |
|----------|-------------|-----------|
| **[Feedzai](https://feedzai.com/)** | End-to-end financial crime and fraud analytics platform with behavioral analytics, real-time detection, AML capabilities, and case management for banks, acquirers, and large institutions. | Banking-grade fraud + AML analytics |
| **[Sardine](https://www.sardine.ai/)** | Adaptive fraud detection platform with ML models trained on billions of signals, a rich feature store (12,000+ features), consortium intelligence, score transparency, and flexible model deployment. | Adaptive ML + feature-store fraud detection |
| **[Featurespace](https://www.featurespace.com/)** | Adaptive behavioral analytics platform specializing in real-time anomaly detection and fraud scoring, with strong performance on low-prevalence fraud patterns and proven uplift in detection rates. | Adaptive behavioral analytics |
| **[SEON](https://seon.io/)** | Real-time fraud prevention and analytics platform with extensive data enrichment, customizable scoring engine, digital footprint analysis, and hybrid rules + AI decisioning. | Data enrichment + flexible fraud scoring |
| **[Sift](https://sift.com/)** | Machine-learning fraud platform delivering real-time risk scores, global network intelligence, account defense, and workflow automation across payments, ATO, and content integrity. | Real-time risk scoring + global signals |
| **[Forter](https://www.forter.com/)** | Identity-centric fraud and abuse decisioning platform providing real-time approve/decline decisions, behavioral insights, and policy enforcement across the customer journey. | Identity & behavioral fraud decisioning |
| **[Riskified](https://www.riskified.com/)** | E-commerce fraud analytics and prevention with chargeback guarantees, adaptive checkout, merchant network intelligence, and decisioning optimized for approval rates. | E-commerce fraud analytics + guarantee |
| **[Kount](https://kount.com/)** (Equifax) | Fraud analytics platform combining device intelligence, customizable rules, omnichannel risk scoring, and robust reporting for e-commerce and digital businesses. | Device intelligence + rules-based analytics |
| **[FICO Falcon](https://www.fico.com/)** | Enterprise fraud management solution with consortium-trained AI/ML models, multi-channel detection, case management, and decades of analytic expertise used by thousands of financial institutions. | Enterprise / consortium fraud models |
| **[Fraud.net](https://www.fraud.net/)** | Enterprise fraud detection and analytics platform with AI/ML, behavioral analytics, orchestration, and case management focused on payments and financial crime. | Enterprise payment fraud analytics |

---

## Open-Source Softwares

Fully production-grade, consortium-powered open-source fraud analytics platforms are rare. Strong open-source building blocks exist for real-time transaction monitoring, adaptive ML, graph-based detection, case management, and end-to-end analytics pipelines.

### Core Frameworks & Fraud Analytics Platforms

| Project | Description | License | Notes |
|---------|-------------|---------|-------|
| **[Jube](https://github.com/jube-home/aml-fraud-transaction-monitoring)** | Open-source AML and fraud detection platform for real-time transaction monitoring, adaptive machine learning, rule-based detection, and workflow-driven case management. | AGPLv3 | One of the more complete open fraud/AML stacks |
| **[Rift](https://github.com/AngelP17/Rift)** | Graph-based intelligence system for entity resolution, anomaly detection, and investigative workflows. Combines GraphSAGE + XGBoost, audit trails, drift monitoring, and governance features. | Open source | Graph-native fraud intelligence |
| **AntiFraud (AI4Risk / finint)** | Research and implementation framework for financial fraud detection, including multiple published graph and attention-based models (MCNN, STAN, STAGN, GTAN, RGTAN, etc.). | GPL-3.0 | Advanced academic / graph fraud models |
| **Financial Fraud Analytics Platforms** | Community end-to-end projects offering risk scoring, batch & real-time detection, investigation tools, and Streamlit/FastAPI dashboards (often Isolation Forest, XGBoost, or similar). | Various (MIT/GPL) | Practical analytics + monitoring demos |
| **CreditGuard & similar MLOps fraud APIs** | Production-oriented fraud/credit risk scoring APIs built with FastAPI, XGBoost/LightGBM, MLflow, and monitoring stacks. | Open source | Deployable scoring services |
| **Graph & hybrid detection toolkits** | Projects implementing temporal graph networks, attention mechanisms, and hybrid supervised/unsupervised models for fraud. | Various | Research-to-production bridges |

### Specialized Libraries & Related Tools

| Project | Description | Focus Area |
|---------|-------------|---------|
| **Anomaly detection libraries** | PyOD, scikit-learn isolation forests, autoencoders, and streaming anomaly tools for unsupervised fraud signals. | Anomaly & outlier detection |
| **Graph ML frameworks** | PyTorch Geometric, DGL, NetworkX, and related libraries for building fraud-ring and entity-link models. | Graph-based fraud detection |
| **Explainability toolkits** | SHAP, LIME, and model-card tooling for transparent fraud scoring. | Model interpretability |
| **Feature stores & streaming** | Feast, Kafka, Flink, or simple feature pipelines for real-time risk features (velocity, device, behavioral). | Real-time feature engineering |
| **Rules engines** | Drools, Easy Rules, or custom Python/JS engines for policy and hybrid decisioning. | Rules + hybrid analytics |
| **Case management foundations** | Open workflow and ticket systems adaptable to fraud investigation queues. | Alert investigation |
| **Drift & monitoring** | Evidently, WhyLogs, or Prometheus/Grafana stacks for model and data drift in fraud systems. | Model operations |

### Additional Notable Open-Source Tools

- **End-to-end pipelines** — Kafka + model serving + feedback loops + continuous training patterns for production fraud analytics.
- **Entity resolution** — Open tools for linking accounts, devices, and identities that underpin network analytics.
- **Dashboarding** — Streamlit, Dash, Metabase, or Apache Superset for risk scorecards, alert queues, and investigation views.
- **Public datasets & benchmarks** — Credit-card fraud, synthetic transaction sets, and graph fraud datasets used to train and evaluate models.
- **Academic model zoos** — Repositories implementing published fraud detection architectures that can be adapted to internal data.
- **Integration layers** — Open API gateways and orchestration tools to connect scoring engines with payment, identity, and case systems.

**Note:** Commercial fraud analytics platforms derive major advantage from proprietary global consortia, massive labeled datasets, continuously updated threat intelligence, and battle-tested case management. Open-source solutions excel as self-hosted monitoring platforms (Jube), graph intelligence systems (Rift), research-grade models, and customizable MLOps scoring pipelines that organizations fully control. Production deployments often combine open analytics engines with commercial enrichment or decisioning services.

---

## Quick Start Recommendations

| Goal | Recommended Starting Point |
|------|---------------------------|
| Self-hosted real-time fraud + AML monitoring | **Jube** |
| Graph-based fraud intelligence & investigation | **Rift** |
| Advanced research / graph neural fraud models | **AntiFraud (AI4Risk)** framework |
| Deployable ML fraud scoring API | CreditGuard-style or FastAPI + XGBoost/LightGBM projects |
| Adaptive behavioral analytics at scale | **Featurespace** or **Sardine** |
| Banking / financial-crime grade analytics | **Feedzai** or **FICO Falcon** |
| Real-time risk scoring + global network | **Sift** |
| Data enrichment + flexible scoring | **SEON** |
| E-commerce fraud analytics + guarantee | **Riskified** or **Forter** |
| Device + rules-based analytics | **Kount** |
| Enterprise payment fraud analytics | **Fraud.net** |

---

## Contributing

Contributions, corrections, and new open-source projects are welcome.  
Please open an issue or pull request.

---

**Last updated:** August 2026  
Emphasizing open-source tools while documenting the major commercial platforms for context. Fully featured, consortium-powered open-source fraud analytics platforms remain limited; the strongest options are self-hosted monitoring systems (Jube), graph intelligence platforms (Rift), research model frameworks, and customizable MLOps scoring pipelines that organizations can extend and operate themselves.
