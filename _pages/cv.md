---
layout: archive
#title: ""
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Education

<p align="justify">
<b>M.S. in Industrial Engineering with Advanced Analytics, 2024</b><br>
University of Illinois at Urbana-Champaign, IL, USA<br>
GPA: 3.80/4.00<br>
Coursework: Basics of Statistical Learning, Data Science Analytics using Probabilistic Graph Models, Analysis of Network Data, Applied Machine Learning, Supply Chain Analytics, Deep Learning with Mathematical Applications, Dynamic Programming and Reinforcement Learning, Statistics for Big Data and Clustering
</p>

<p align="justify">
<b>Bachelor of Engineering in Industrial Engineering and Management, 2021</b><br>
BMS College of Engineering, Bangalore, India<br>
GPA: 9.16/10.00<br>
Coursework: Advanced Operations Research, Artificial Intelligence and Expert Systems, Statistics, Supply Chain and Logistics Management, Simulation Modeling and Analysis, Lean Manufacturing, Quality Assurance and Reliability, Enterprise Resource Planning, Production Technology, Operations Management
</p>

## Skills

<p align="justify">
<ul>
  <li><b>Programming Languages:</b> Python, R, SQL, C++, MATLAB</li>
  <li><b>Python Libraries:</b> Pandas, NumPy, Scikit-Learn, Seaborn, TensorFlow, Keras, PyTorch, XG-Boost, Networkx, NLTK, spaCy, Huggingface-hub, Transformers</li>
  <li><b>ML & DL Techniques:</b> Regression, SVM, Clustering, Time-series Analysis, RL, CNN, RNN, GAN, NLP, DQN, GCN</li>
  <li><b>Data-Centric AI and Graph Learning:</b> Data Quality Improvement, Predictive Analytics with Graphs, Graph Databases (Neo4j, Amazon Neptune)</li>
  <li><b>Big Data Technologies:</b> Apache (Hadoop, Spark, Kafka), Distributed Computing Frameworks (MapReduce)</li>
  <li><b>Cloud Computing and MLOps:</b> AWS (S3, EMR, EC2, Redshift, SageMaker, Glue, Lambda, Bedrock), GCP (GKE, Vertex AI, BigQuery), MS Azure</li>
  <li><b>Observability & Eval:</b> Langfuse, Langtrace, LangSmith, Prometheus, Grafana, OpenTelemetry, MLflow, Arize, RAGAS, Guardrails AI</li>
  <li><b>APIs & UI:</b> FastAPI, gRPC, GraphQL, Chainlit, Streamlit</li>
</ul>
</p>

## Work Experience

<p align="justify">
<b>Data Scientist @ Wells Fargo</b> (May 2023 - Present)<br>
<ul>
  <li>Developed AI-powered NER pipeline using transformer models (BERT, Llama) and LLM APIs via LangChain, reducing manual labeling by 80% and improving F1 scores by 40% to accelerate dataset creation for complaint triage and risk operations.</li>
  <li>Fine-tuned Llama 2 & Phi-2 using PEFT for CFPB complaint classification and summarization, improving F1 by +15 points through golden-set validation. Deployed via scheduled Vertex AI batch jobs with BigQuery output.</li>
  <li>Co-developed and fine-tuned Llama-3 8B using LoRA + RLHF with proprietary domain data, achieving 88% faithfulness through ablation studies, deployed as low-latency endpoints using vLLM with Ray Serve on GKE.</li>
  <li>Led intern mentorship to generate 12k+ synthetic training examples using teacher LLM (OpenAI) with rejection sampling, improving rare-class recall by +10 points and reducing annotation effort by 30% with Langfuse tracked HITL loops.</li>
  <li>Engineered content quality pipeline with semantic embedding deduplication and LLM-powered simplification, reducing duplicates and document length by 30% with Pydantic schema checks and data versioning.</li>
  <li>Built hybrid RAG platform on GKE with intelligent query routing across Postgres+pgvector, Vertex AI Vector Search, and Neo4j GraphRAG. Achieved +20% retrieval accuracy and -40% manual review time for compliance Q&A and research.</li>
  <li>Performed retrieval R&D on chunking and hybrid BM25+dense with graph/vector routing, rerankers and multi-hop reasoning. Deployed a production evaluation stack with RAGAS metrics, Arize and MLflow tracing, and CI/CD regression gates.</li>
  <li>Prototyped a governed multi-agent analytics stack with Google A2A and MCP tools, routed NL to SQL, RAG, and analytics tasks with memory, human-in-the-loop validation, and observability, reducing time-to-insight by 40%.</li>
</ul>
</p>

<p align="justify">
<b>Data Scientist @ Genpact</b> (August 2022 - August 2023)<br>
Contact-Center NLU analytics pipeline for a Financial Services Client:
<ul>
  <li>Built turn-level intent and sentiment classifiers for diarized call transcripts using Python and spaCy. Fine-tuned and benchmarked multiple transformer models (BERT, RoBERTa, DistilBERT, GPT-3) optimizing for F1/latency trade-offs. Deployed Streamlit applications for training needs analysis and operations dashboards, improving CSAT by 40% in pilot regions.</li>
  <li>Implemented comprehensive privacy controls for call transcripts with PII redaction, encryption, and audit trails. Collaborated with PMs and SMEs to label 2,500+ utterances across 15+ call categories, creating a compliant, high-quality training dataset.</li>
  <li>Developed hierarchical call-level feature aggregation system generating KPIs for QA, coaching, and trend analysis. Delivered prescriptive analytics that guided chatbot training improvements, increased resolution rates, and informed customer retention strategies.</li>
  <li>Enhanced sentiment detection accuracy from 68% to 92% by replacing VADER/logistic regression with class-weighted, threshold calibrated BERT model featuring span aggregation.</li>
  <li> Identified anomalously long handle-time calls using Isolation Forest trained on call features and operational metadata. Flagged outliers enabled root-cause analysis and workflow optimization to reduce call duration.</li>
  <li>Engineered end-to-end MLOps pipeline on AWS including batch processing (S3, Step Functions), model training/registry (SageMaker), real-time inference endpoints, CI/CD automation, and monitoring.</li>
</ul>
Predictive Analytics for a Global Sports Apparel Retail Client:
<ul>
  <li>Optimized ad targeting strategy by developing predictive models (Logistic Regression, SVM, Random Forest) to forecast user click propensity and delivered a 12% CTR increase and improved ROAS across key customer segments during seasonal, quarterly campaigns.</li>
  <li>Collaborated with the marketing and UX teams to design and execute A/B tests using Google Optimize and Hotjar, optimizing ad placement and creative strategies that improved CTR by 15% MoM across campaigns reaching 3M ad impressions per month.</li>
  <li>Developed ARIMA and autoregressive models to forecast key ad performance metrics (clicks, RPC, CTR), enabling proactive budget allocation and improving campaign ROI forecast accuracy by 20%.</li>
  <li>Built ETL pipelines using Python, SQL, AWS Glue, and Redshift to integrate cross-platform ad, CRM, and web data sources, ensuring near real-time availability for campaign performance tracking.</li>
  <li>Designed and maintained automated Tableau dashboards to visualize the customer journey, engagement metrics, lead conversion, and ad revenue, improving decision making between the Marketing and Product teams.</li>

</ul>  
</p>

<p align="justify">
<b>Operations Manager & Data Scientist@ Amazon India</b> (June 2020 – July 2021)<br>
<ul>
  <li>Improved SKU level forecast accuracy by 15% MAPE using ARIMA, SARIMAX, ETS, Prophet, LSTM, and DeepAR models, reducing inventory cost by 10% while preserving fill rate across 13 FCs.</li>
 <li>Built reusable SKU-week feature store with key attributes (buffer, staleness, discount, segment) that powered forecasting models, pricing algorithms, and operational dashboards across multiple business functions.</li>
 <li>Automated Andes to S3 ETL with Redshift, Glue, Athena, and PySpark, eliminating manual refresh and enabling reliable updates.</li>
 <li>Designed SKU-Customer segmentation to optimize inventory routing between replenishment and clearance channels, increasing GMROI on markdown cohorts, and accelerating turnover of slow movers.</li>
 <li>Standardized KPIs and launched Inventory Health, in-stock, and compliance dashboards in Tableau, automating over 300 recurring reports and improving operational efficiency by 20%.</li>
  <li>Collaborated with ops, marketing, finance, and FC leaders on weekly reviews, applying causal inference and what-if analysis to identify forecast drivers and align supply chain strategies.</li>
</ul>
</p>

<p align="justify">
<b>Research Intern @ Hindustan Aeronautics Limited</b> (May 2018 - Jul 2018)<br>
<ul>
  <li>Conducted a comprehensive research internship in the Integrated Materials Management Department within the Engine Division.</li>
  <li>Led a pivotal project investigating the feasibility of integrating barcode technology for enhanced material traceability.</li>
</ul>
</p>


## Teaching

<p align="justify">
<b>Graduate Teaching Assistant @ University of Illinois Urbana-Champaign</b><br>
<ul>
  <li>Course: ECE 486 - Control Systems</li>
  <li>Supervised weekly control systems labs, guiding 30+ students through experiments, ensuring comprehension of key concepts, and assisting in the grading of lab assignments</li>
  <li>Mentored students in their final projects on the design and implementation of control systems, including evaluating and grading project work</li>
</ul>
</p>

## Certifications

<p align="justify">
<ul>
  <li><b>Tensorflow Developer Certificate</b></li>
  <li><b>AWS Certified Cloud Practitioner</b></li>
  <li><b>Natural Language Processing on Google Cloud</b></li>
  <li><b>Practical MLOps: AWS for Data Scientists & DevOps</b></li>
  <li><b>Six Sigma: DMAIC from Technical University of Munich</b></li>
  <li><b>Excel Skills for Business from Macquarie University</b></li>
</ul>
</p>

## Languages

<p align="justify">
<ul>
  <li><b>English</b></li>
  <li><b>German - A2 Level</b></li>
</ul>
</p>



  
