# Enhanced-SAIP-Benchmarking

**An Interdisciplinary Framework for Evaluating On-Device AI Performance Using Information Systems Theory and Econometric Analysis**

---

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Python Version](https://img.shields.io/badge/python-3.9%2B-green.svg)]()

## 🌟 Overview

This repository provides a comprehensive benchmarking framework that integrates **Information Systems Theory (DeLone & McLean)**, **Technology Acceptance Models (TAM)**, and **Econometric Analysis** to evaluate small Large Language Models (sLLMs) running on Neural Processing Units (NPUs).

It extends standard engineering benchmarks with behavioral and economic constructs to produce a multi-dimensional assessment of on-device AI performance.

### Key Capabilities

* Multi-dimensional performance evaluation (technical, economic, behavioral)
* Translation of low-level metrics (latency, throughput) to IS Quality measures
* Operationalized TAM (PU, PEOU, BI) for adoption modeling
* Advanced econometric modeling (Cobb–Douglas, DEA, panel models)
* SAIP adaptive policy for latency/efficiency optimization
* Publication-ready visualizations and reproducible analysis notebooks

---

## 📁 Repository Layout

```
Enhanced-SAIP-Benchmarking/
├── data/
│   ├── comprehensive_analysis.json
│   ├── comprehensive_results.xlsx
│   ├── kpi_summary.csv
│   └── raw_results.csv
│
├── models/
│   ├── cost_function_summary.txt
│   ├── panel_data_model_summary.txt
│   └── production_function_summary.txt
│
├── visualizations/
│   ├── is_quality_dashboard.png
│   ├── performance_heatmap.png
│   ├── policy_effectiveness.png
│   ├── tam_analysis.png
│   └── technical_efficiency.png
│
├── .gitignore
├── LICENSE
├── README.md
├── requirements.txt
└── sLLM_MIS_논문반영.ipynb
```

---

## 📋 Quick Start

### Clone & Install

```bash
git clone https://github.com/your-username/Enhanced-SAIP-Benchmarking.git
cd Enhanced-SAIP-Benchmarking
pip install -r requirements.txt
```

### Run the Main Analysis Notebook

All analyses, visualizations, and econometric modeling are orchestrated from the main Jupyter Notebook:

```bash
jupyter notebook sLLM_MIS_논문반영.ipynb
```

Run all cells sequentially to reproduce the entire pipeline. The notebook will automatically load the required datasets, run econometric and IS-theory-based analyses, and generate visualization outputs.

---

## 🔧 Configuration & Inputs

Configuration parameters (e.g., model selection, number of trials, policy settings) can be modified in the first section of the notebook.

### Default Configuration

* **Tasks:** NLU (SST-2), QA (SQuAD v2), Summarization (CNN/DailyMail)
* **Trials:** 3 independent runs per task-model pair
* **Models:** 9 sLLMs (DeepSeek, Llama, Gemma, OPT, Qwen2.5, EXAONE, Midm families)
* **Prompt Mode:** Zero-shot

---

## 🧠 Theoretical Framework

### 1. Information Systems Quality Model (DeLone & McLean)

* **System Quality:** Performance, reliability, response time
* **Information Quality:** Accuracy, completeness, consistency
* **Service Quality:** Responsiveness, efficiency, user satisfaction

### 2. Technology Acceptance Model (TAM)

* **Perceived Usefulness (PU):** Performance and efficiency metrics
* **Perceived Ease of Use (PEOU):** Resource efficiency and stability
* **Behavioral Intention (BI):** Adoption likelihood prediction

### 3. Econometric Analysis

* **Production Functions:** Cobb–Douglas modeling of AI inference
* **Technical Efficiency:** Data Envelopment Analysis (DEA)
* **Cost Functions:** Economic relationship between inputs and outputs

---

## 📊 Key Results

### Hypothesis Testing Summary

| Hypothesis | Research Area    | Key Finding                                | Status              |
| :--------- | :--------------- | :----------------------------------------- | :------------------ |
| H1         | IS Success Model | Technical performance → Higher IS Quality  | ✅ Supported         |
| H2         | TAM              | Performance + Efficiency → Higher Adoption | ✅ Supported         |
| H3         | Econometrics     | Diminishing returns to scale confirmed     | ✅ Supported         |
| H4         | Adaptive Policy  | SAIP reduces latency (30–45% gains)        | ✅ Largely Supported |

### Model Performance Ranking

1. **Qwen2.5-0.5B-Instruct:** Best overall performance and efficiency
2. **EXAONE-3.5-2.4B-Instruct:** Strong balance of performance and features
3. **Gemma-2B-IT:** Competitive mid-range performer

---

## 📈 Outputs

### Data Directory (`data/`)

* `raw_results.csv`: Raw benchmark data
* `kpi_summary.csv`: Aggregated KPIs
* `comprehensive_results.xlsx`: Processed econometric outputs
* `comprehensive_analysis.json`: Detailed JSON summary

### Models Directory (`models/`)

* `cost_function_summary.txt`: Cost function estimations
* `production_function_summary.txt`: Cobb–Douglas production results
* `panel_data_model_summary.txt`: Panel data regression outputs

### Visualizations Directory (`visualizations/`)

* `is_quality_dashboard.png`: DeLone & McLean IS success visualization
* `performance_heatmap.png`: Latency and throughput distribution
* `policy_effectiveness.png`: SAIP policy before/after effects
* `tam_analysis.png`: PU–PEOU–BI relationships
* `technical_efficiency.png`: DEA efficiency frontier

---

## ✅ Summary of Findings

* **Technical → IS Quality:** Higher stability and throughput lead to greater IS Quality scores.
* **Performance → Adoption (TAM):** PU and PEOU strongly predict adoption intent.
* **Econometrics:** Confirmed diminishing returns to scale for sLLM inference.
* **Adaptive Policy (SAIP):** Reduced latency by ~30–45% without accuracy loss.

---

## 📄 License

This project is licensed under the **MIT License** — see the `LICENSE` file for details.

---

## 🙏 Acknowledgments

* Rebellions Inc. for NPU access and infrastructure support
* Open-source AI community for model architectures
* Beta testers and contributors



<!-- EOF -->
