# GROWA - NASA-Space-Apps-Challenge-2025

Growa-gov: Data Pathways to Healthy Cities

Growa-gov is an advanced analytics platform developed for the 2025 NASA Space Apps Challenge: "Data Pathways to Healthy Cities and Human Settlements." Our mission is to empower the public sector with tools to transform complex geostatistical, economic, and climate data into proactive, evidence-based decisions.

https://growateam.com/

In an era where climate volatility, rapid urbanization, and economic uncertainty present unprecedented challenges to governments, relying on intuition alone is no longer sufficient. Our mission is to empower the public sector by transforming vast streams of complex geostatistical, economic, and climate data into a clear signal for action. We provide leaders with the tools needed to navigate modern complexities and make proactive, evidence-based decisions that foster resilient and prosperous communities.
Our solution moves beyond static reports to create a dynamic intelligence ecosystem focused on the three interconnected pillars of sustainable development: Food Security, Public Health, and Urban Development. By integrating and analyzing data across these domains, Growa-gov uncovers critical relationships between environmental stressors and societal well-being. Using a hybrid approach of machine learning and econometric models, our platform anticipates risks like supply chain disruptions and disease outbreaks, identifies opportunities for sustainable growth, and quantifies the potential impact of policy interventions. Ultimately, we equip decision-makers with the precise insights required to execute policies with confidence and build a secure future.

Repository Structure and Technical Workflow

This repository is architecturally designed as a collection of self-contained Jupyter Notebooks (.ipynb) and their corresponding static HTML outputs. Each notebook represents a complete and reproducible analysis pipeline for a specific predictive task, from data ingestion to model evaluation. The file-naming convention, such as Module 1 - ... or Module 2 - ..., thematically groups these pipelines according to core project goals (e.g., food security, public health, urban development). Accompanying the notebooks, the .html files serve as interactive visualizations of the final predictions, presenting the rules and insights derived from each model in a universally accessible format. This dual-output structure ensures that the research is both fully reproducible for technical audiences and easily interpretable for stakeholders.

The data workflow is intentionally decoupled from the codebase to maintain portability. The complete raw dataset, spanning from 2003 to 2024 for 140 municipalities, is hosted externally on a centralized Google Drive to ensure a single source of truth. This repository integrates three distinct, high-dimensional data domains. The first is agro-climatic data, which fuses agricultural statistics from government portals like SIAP (including metrics like Superficie Cosechada and Producción for 5 primary crops) with a comprehensive set of 38 climate variables from the NASA POWER Project, such as radiation (ALLSKY_SFC_SW_DWN) and temperature (T2M). The second domain consists of epidemiological and sociodemographic data, which combines public health records on dengue cases with demographic indicators to model disease risk. The third domain includes urban and environmental data, which leverages demographic information and indicators of urban infrastructure to assess the climate resilience and sustainability of human settlements.

The initial cells within each Jupyter Notebook execute a detailed and domain-specific ETL (Extract, Transform, Load) process. Raw .xlsx and .csv files for each domain are programmatically extracted from the Drive, merged into unified data structures, and subjected to a rigorous cleaning and feature engineering pipeline. This crucial step transforms the multi-source raw data into a model-ready format, primed for the exploratory data analysis (EDA) and the subsequent training of our predictive models, which are built using libraries like TensorFlow, Keras, and Scikit-learn. This robust workflow guarantees a clear and replicable path from raw, diverse data sources to actionable, integrated insights.

DRIVE/FILES; https://drive.google.com/drive/folders/1x9ZU8qjvCQ9H-DJgKGc33JKkLV4W1USY?usp=drive_link








