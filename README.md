# -Forecasting-Stock-Market-Crashes# Forecasting Stock Market Crashes via Machine Learning

## Overview
This repository implements machine learning techniques to forecast stock market crashes, based on the research paper "Forecasting Stock Market Crashes via Machine Learning" by Hubert Dichtl et al. The model uses data from major Eurozone countries and employs Support Vector Machines (SVM) along with other ML techniques to predict market downturns.

## Features
- Comprehensive set of 28 market predictors including:
  - Price-based indicators
  - Fundamental metrics
  - Sentiment indicators
  - Macroeconomic variables
- Machine learning models:
  - Support Vector Machines (primary model)
  - Logistic Regression (baseline)
  - Random Forests (comparison)
  - Gradient Boosted Trees (comparison)
- Performance evaluation using both statistical and economic metrics

## Requirements
- Python 3.8+
- Required packages listed in `requirements.txt`

## Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/stock-market-crash-prediction.git
cd stock-market-crash-prediction

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## Project Structure
```
StockMarketCrashPrediction_ML/
│
├── README.md
├── LICENSE
├── .gitignore
├── data/
│   ├── raw/
│   ├── processed/
├── notebooks/
│   ├── 01_DataPreprocessing.ipynb
│   ├── 02_ExploratoryDataAnalysis.ipynb
│   ├── 03_FeatureEngineering.ipynb
│   ├── 04_ModelTraining.ipynb
│   ├── 05_EvaluationAndVisualization.ipynb
├── src/
│   ├── __init__.py
│   ├── data_preprocessing.py
│   ├── feature_engineering.py
│   ├── model_training.py
│   ├── evaluation.py
├── tests/
│   ├── test_data_preprocessing.py
│   ├── test_feature_engineering.py
│   ├── test_model_training.py
├── results/
│   ├── model_outputs/
│   ├── evaluation_metrics/
├── docs/
│   ├── requirements.md
│   ├── references.md
├── requirements.txt
├── environment.yml
└── scripts/
    ├── download_data.sh
    ├── run_pipeline.py

```

## Usage
1. Data Preparation:
```python
python src/data_preprocessing.py
```

2. Feature Engineering:
```python
python src/feature_engineering.py
```

3. Model Training:
```python
python src/model_training.py
```

4. Evaluation:
```python
python src/evaluation.py
```

## Model Performance
The SVM model demonstrates superior performance compared to baseline approaches:
- Higher prediction accuracy for crash events
- Better economic performance in portfolio simulation
- More robust across different market conditions

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Citation
If you use this code in your research, please cite:
```
@article{dichtl2022forecasting,
  title={Forecasting Stock Market Crashes via Machine Learning},
  author={Dichtl, Hubert and Drobetz, Wolfgang and Otto, Tizian},
  year={2022}
}
```

## Acknowledgments
- Based on research by Hubert Dichtl, Wolfgang Drobetz, and Tizian Otto
- Data providers: Refinitiv, ECB
