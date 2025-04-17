# Quantitative Stock Models: Beating the S&P 500

## Overview
This project explores quantitative strategies—Linear Regression, K-Means Clustering, and Bayesian Inference—to select stocks and construct portfolios aimed at outperforming the S&P 500 index. Historical stock and financial data from 2022 was analyzed to predict and optimize investment outcomes for 2023, achieving significant market outperformance.

## Objectives
- **Primary Goal**: Develop quantitative investment strategies that reliably outperform the S&P 500 benchmark.
- **Model Comparison**: Evaluate Linear Regression, K-Means Clustering, and Bayesian methods based on predictive accuracy and portfolio returns.
- **Strategic Insight**: Provide actionable insights into stock categorization and strategic portfolio allocation.


## Modeling Approaches

### Linear Regression
- **Purpose**: Baseline predictive model identifying stock price drivers.
- **Features**: Financial ratios (EPS, revenue growth, ROE, dividend yield).
- **Portfolio Strategy**: Allocated 70% to Growth stocks, 20% Value stocks, 10% Income stocks.

### K-Means Clustering
- **Purpose**: Unsupervised approach identifying natural groupings of stocks based on financial indicators.
- **Metrics**: Silhouette Score used to ensure clustering quality.
- **Portfolio Strategy**: Same allocation strategy emphasizing Growth stocks.

### Bayesian Inference
- **Purpose**: Leveraged probabilistic modeling to integrate prior knowledge and handle uncertainty dynamically.
- **Methodology**: Bayesian regression using priors informed by Linear Regression results.
- **Challenges**: High computational demands and lower practical returns, highlighting need for optimization.


## Results Summary

| Model                | Annual Return (2023) | Outperformed S&P 500 (26.71%)? | Key Observations                 |
|----------------------|----------------------|--------------------------------|----------------------------------|
| **Linear Regression**| **44.43%** 🚀        | ✅ Yes                         | Highest predictive accuracy      |
| **K-Means Clustering**| 31.49% 📈           | ✅ Yes                         | Effective clustering; strong but lower returns |
| **Bayesian Inference**| 0.77% 📉            | ❌ No                          | Computationally demanding; underperformed |

### Key Takeaways:
- Linear Regression clearly outperformed, delivering highest returns with good predictive accuracy.
- K-Means offered solid but comparatively lower performance.
- Bayesian Inference needs computational refinement but remains promising for risk-aware strategies.

## Limitations and Future Directions
- **Computational Efficiency**: Bayesian approach requires optimization for real-time use.
- **Feature Selection**: Expanding and refining financial data features could further enhance model accuracy.
- **Hybrid Models**: Exploring combinations of these models may yield superior investment strategies.

## Conclusion
This project demonstrates the significant potential of quantitative strategies for outperforming traditional passive investment benchmarks like the S&P 500. Among the tested models, Linear Regression offered the strongest immediate returns, while Bayesian methods offer promising avenues for future enhancement with their inherent adaptability and uncertainty quantification.

This structured, comparative approach provides clear actionable insights for investors, emphasizing how systematic modeling can significantly enhance portfolio performance.

## Bayesian Inference Primer
Bayesian inference models uncertainty explicitly through probability distributions:

p(w \mid D) \propto p(D \mid w) \cdot p(w)

- **p(w)**: Prior distribution based on Linear Regression insights.
- **p(D | w)**: Likelihood based on observed financial data.
- **p(w | D)**: Posterior distribution offering dynamic stock selection and risk-aware decision-making.

The model optimizes an **Evidence Lower Bound (ELBO)** using variational inference to approximate complex posterior distributions.

## Author
**John Grier**  
MS Data Science Candidate, Illinois Tech  
[GitHub: J-Grier](https://github.com/J-Grier)

## References
- Yahoo Finance historical data
- Zhao Gao, \"The application of artificial intelligence in stock investment\" (2020)
- Wikipedia: [S&P 500 Tickers](https://en.wikipedia.org/wiki/List_of_S%26P_500_companies)


## Project Structure

quantitative-stock-models/ ├── cleaned_QuantitativeModels.ipynb # Main notebook with all analysis ├── README.md # Project overview and instructions ├── requirements.txt # Environment dependencies ├── data/ # (Optional) Include small public data or add link └── images/ # Charts and visualizations

## Requirements

See `requirements.txt` for all package dependencies.

## Setup

```bash
# Clone repo
git clone https://github.com/J-Grier/quantitative-stock-models.git

# Create environment and install dependencies
pip install -r requirements.txt
