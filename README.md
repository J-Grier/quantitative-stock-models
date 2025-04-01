# Quantitative Stock Models: Beating the S&P 500

This project explores multiple quantitative modeling techniques to identify stock selections that outperform the S&P 500 benchmark. The analysis focuses on evaluating data from 2022 to predict performance in 2023 using a combination of regression, clustering, and Bayesian methods.

## Project Goal

To classify and select a portfolio of stocks that beats the S&P 500 index, achieving over 17% relative outperformance through rigorous quantitative analysis.

## Models Used

- **Linear Regression**
  - Used as a baseline predictive model for price movement.
  - Found limited predictive power due to noisy stock features.

- **K-Means Clustering**
  - Grouped stocks based on financial and technical characteristics.
  - Helped in segmenting investment-worthy clusters.

- **Bayesian Inference**
  - Incorporated uncertainty into predictions.
  - Demonstrated robust performance with probabilistic confidence intervals.

## Key Features and Insights

- Focused on stock data post-2018, filtering out sparse short-interest periods.
- Subset includes only the 2022 training period to predict 2023 outcomes.
- Evaluated model outcomes relative to S&P 500 benchmark performance.

## Project Structure

quantitative-stock-models/ ├── cleaned_QuantitativeModels.ipynb # Main notebook with all analysis ├── README.md # Project overview and instructions ├── requirements.txt # Environment dependencies ├── data/ # (Optional) Include small public data or add link └── images/ # Charts and visualizations

## Results

- The final model-based portfolio **outperformed the S&P 500 by over 17%** in backtesting.
- Bayesian methods offered the best balance of performance and explainability.

## Requirements

See `requirements.txt` for all package dependencies.

## Setup

```bash
# Clone repo
git clone https://github.com/J-Grier/quantitative-stock-models.git

# Create environment and install dependencies
pip install -r requirements.txt

## Author

**John Grier**  
MS Data Science Candidate, Illinois Tech  
[GitHub: J-Grier](https://github.com/J-Grier)
