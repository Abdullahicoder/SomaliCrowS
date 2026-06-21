# SomaliCrowS Analysis: Gender Bias Evaluation in Somali Language Models

## Overview

This repository contains the analysis pipeline, statistical summaries, and visualizations for **SomaliCrowS**, a benchmark designed to measure **gender bias in Somali language models**.

The project evaluates whether language models systematically assign higher probabilities to male-associated or female-associated sentence variants across multiple social domains, including:

- Occupation
- Leadership
- Business
- Education
- STEM
- Family
- Politics

The analysis quantifies bias using log-probability differences between matched male and female sentence pairs and generates publication-ready figures and statistical summaries.

---

## Motivation

While fairness benchmarks are widely available for high-resource languages such as English, Somali remains significantly underrepresented in NLP bias and fairness research.

SomaliCrowS aims to:

- Measure gender bias in Somali language models
- Identify domain-specific stereotypes
- Provide reproducible evaluation methods
- Support fairness research for low-resource languages
- Enable comparison across future Somali NLP systems

---

## Dataset Structure

| Column | Description |
|----------|------------|
| ID | Unique example identifier |
| Category | Original Somali category |
| Subcategory | Fine-grained stereotype category |
| Female Sentence | Female-targeted sentence |
| Male Sentence | Male-targeted sentence |
| Mask Template | Template used during evaluation |
| Target Concept | Occupation or concept being evaluated |
| Bias Type | Human-readable bias category |
| Female_Log_Prob | Log probability assigned to the female sentence |
| Male_Log_Prob | Log probability assigned to the male sentence |
| Delta_Bias | Female score minus male score |
| Direction | Model preference direction |

---

## Analysis Outputs

### Statistical Tables

- Bias statistics by category
- Mean bias scores
- Standard deviations
- Preference percentages
- Most stereotyped examples

### Visualizations

- Mean Bias by Bias Type
- Direction Counts by Bias Type
- Distribution of Delta Bias
- Overall Preference Breakdown

---

## Repository Structure

```text
SomaliCrows_Analysis/
│
├── somali_bias_analysis_results.csv
├── bias_type_summary.csv
│
├── figures/
│   ├── fig1_mean_bias_by_bias_type.png
│   ├── fig2_direction_counts_by_bias_type.png
│   ├── fig3_delta_bias_distribution.png
│   └── fig4_overall_direction_breakdown.png
│
└── New_SomaliCrowS_Analysis.ipynb
```

---

## Research Applications

- Fairness evaluation
- Bias auditing
- Somali NLP research
- Cross-lingual bias studies
- Responsible AI development
- Low-resource language benchmarking

## Citation

```bibtex
@dataset{somalicrows2026,
  title={SomaliCrowS: A Gender Bias Benchmark for Somali Language Models},
  author={Abdullahi Ahmed},
  year={2026}
}
```
