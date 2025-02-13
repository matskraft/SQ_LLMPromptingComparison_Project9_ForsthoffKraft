# LLM Comparison Pipeline

## Overview

This project provides a comprehensive pipeline for evaluating different Large Language Models (LLMs) on translation tasks. It includes prompt generation, model interaction, and evaluation using multiple metrics. The results are logged and analyzed with MLflow.

## Features

- **Model Evaluation:** Supports multiple LLMs for translation tasks.
- **Automated Pipeline:** Streamlined workflow from data import to evaluation.
- **Custom Metrics:** Implements BERT Score and an enhanced LLM-as-a-Judge (LLMaaJ) metric.
- **MLflow Integration:** Tracks experiments and visualizes results.
- **Caching:** Option to reuse previous translations for efficiency.
- **Visualization:** Box plots and other analytics for model comparison.

## Workflow

1. **Setup & Installation**
   - Installs necessary dependencies, including `llama-cpp-python`, `mlflow`, and `bert-score`.
2. **Data Import & Preparation**
   - Loads dataset containing translation inputs and expected outputs.
3. **Model Interaction**
   - Calls different LLMs to generate translations.
   - Stores responses for evaluation.
4. **Evaluation Metrics**
   - Calculates BLEU, ROUGE, BERT Score, and LLMaaJ similarity.
5. **MLflow Logging**
   - Saves metrics and experiment data for analysis.
6. **Visualization & Analysis**
   - Generates plots for metric comparison across models.

## Getting Started

1. Clone the repository:
   ```sh
   git clone <repo-url>
   cd <project-folder>
   ```
2. Run the pipeline notebook:
   ```sh
   jupyter notebook llm_comparison_full_pipeline.ipynb
   ```

## Dependencies

- Python 3.x
- pandas, seaborn, matplotlib
- mlflow
- llama-cpp-python
- bert-score

## Contributors

- Mats Kraft and Leander Forsthoff

## License

This project is licensed under [MIT License](LICENSE).
