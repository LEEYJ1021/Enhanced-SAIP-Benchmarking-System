**An Interdisciplinary Framework for Evaluating On-Device AI Performance Using Information Systems Theory and Econometric Analysis**

---

## 🌟 Overview

This repository presents a comprehensive benchmarking framework that integrates **Information Systems Theory**, **Technology Acceptance Models (TAM)**, and **Econometric Analysis** to evaluate Small Large Language Models (sLLMs) on Neural Processing Units (NPUs). The framework extends traditional performance metrics with theoretical constructs from multiple disciplines.

**Key Features:**
- Multi-dimensional performance evaluation (technical, economic, behavioral)
- Integration of DeLone & McLean IS Success Model
- Technology Acceptance Model (TAM) operationalization
- Advanced econometric modeling (Production Functions, Technical Efficiency)
- Machine Learning-based adaptive optimization (SAIP policy)
- Comprehensive visualization and reporting

## 📋 Quick Start

### Installation

```bash
git clone [https://github.com/your-username/Enhanced-SAIP-Benchmarking.git](https://github.com/your-username/Enhanced-SAIP-Benchmarking.git)
cd Enhanced-SAIP-Benchmarking

pip install -r requirements.txt
````

### Basic Usage

```python
from src.enhanced_saip_analyzer import EnhancedSAIPAnalyzer

# Initialize analyzer
analyzer = EnhancedSAIPAnalyzer()

# Run comprehensive analysis
results = analyzer.run_complete_analysis(
    main_data_path="data/sample_data_main.csv",
    timeseries_data_path="data/sample_data_timeseries.csv"
)

# Generate publication-ready visualizations
analyzer.generate_publication_figures()
```

### Jupyter Notebook

For interactive analysis, use the provided Jupyter notebook:

```bash
jupyter notebook notebooks/SAIP_Benchmarking_Analysis.ipynb
```

## 🏗️ Theoretical Framework

### 1\. Information Systems Quality Model (DeLone & McLean)

  - **System Quality:** Performance, reliability, response time
  - **Information Quality:** Accuracy, completeness, consistency
  - **Service Quality:** Responsiveness, efficiency, user satisfaction

### 2\. Technology Acceptance Model (TAM)

  - **Perceived Usefulness (PU):** Performance and efficiency metrics
  - **Perceived Ease of Use (PEOU):** Resource efficiency and stability
  - **Behavioral Intention (BI):** Adoption likelihood prediction

### 3\. Econometric Analysis

  - **Production Functions:** Cobb-Douglas modeling of AI inference
  - **Technical Efficiency:** Data Envelopment Analysis (DEA)
  - **Cost Functions:** Economic relationship between inputs and outputs

## 📊 Key Results

### Hypothesis Testing Summary

| Hypothesis | Research Area | Key Finding | Status |
| :--- | :--- | :--- | :--- |
| H1 | IS Success Model | Technical performance → Higher IS Quality | ✅ Supported |
| H2 | TAM | Performance + Efficiency → Higher Adoption | ✅ Supported |
| H3 | Econometrics | Diminishing returns to scale confirmed | ✅ Supported |
| H4 | Adaptive Policy | SAIP reduces latency (30-45% gains) | ✅ Largely Supported |

### Model Performance Ranking

1.  **Qwen2.5-0.5B-Instruct:** Best overall performance and efficiency
2.  **EXAONE-3.5-2.4B-Instruct:** Strong balance of performance and features
3.  **Gemma-2B-IT:** Competitive mid-range performer

## 🎯 Research Questions Addressed

### RQ1: Technical → IS Quality Translation

Our framework successfully translates low-level technical metrics (latency, throughput) into holistic IS quality measures using the D\&M model.

### RQ2: Performance → User Adoption

TAM analysis reveals that both performance (PU) and efficiency (PEOU) are critical for adoption intention.

### RQ3: Economic Production Relationships

Econometric models confirm diminishing marginal returns to scale in sLLM inference.

### RQ4: Adaptive Policy Effectiveness

SAIP policy demonstrates significant latency reductions (30-45%) across most model configurations.

## 📁 Dataset Description

### Model Specifications

9 sLLMs ranging from 0.5B to 3.2B parameters, including:

  - DeepSeek, Llama, Gemma, OPT, Qwen2.5, EXAONE, Midm families

### Task Categories

  - **NLU:** Sentiment classification (SST-2)
  - **QA:** Extractive question answering (SQuAD v2)
  - **Summarization:** Abstractive summarization (CNN/DailyMail)

### Evaluation Protocol

  - 100 samples per task, 3 independent trials
  - Zero-shot prompting strategy
  - N=300 observations per model-task combination

## 🔧 Configuration

Modify `config/analysis_config.yaml` to customize:

```yaml
analysis:
  models: ["Qwen2.5-0.5B", "Llama-3.2-3B", "Gemma-2B"]
  tasks: ["NLU", "QA", "Summarization"]
  metrics: ["latency", "throughput", "energy", "accuracy"]
  
econometric:
  production_function: "cobb_douglas"
  efficiency_method: "dea"
  confidence_level: 0.95
```

## 📈 Outputs

The framework generates:

  - Comprehensive Results (Excel, CSV, JSON)
  - Publication-Ready Visualizations (PNG, PDF)
  - Econometric Model Summaries
  - Statistical Validation Reports
  - Interactive Dashboards


## 🤝 Contributing

We welcome contributions\! Please see our Contributing Guidelines and read our Code of Conduct.

## 📄 License

This project is licensed under the MIT License - see the `LICENSE` file for details.

## 🙏 Acknowledgments

  - Rebellions Inc. for NPU access and support
  - The open-source AI community for model architectures
  - Contributors and beta testers
