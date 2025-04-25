# Quantitative Stock Models: Beating the S&P 500

## 📖 Quick Links
- [Overview](#overview)
- [Objectives](#objectives)
- [Modeling Approaches](#modeling-approaches)
- [Results Summary](#results-summary)
- [Supplemental Analysis: Macroeconomic Scenario-Based Portfolio Allocation (Newly Added!)](#supplemental-analysis-macroeconomic-scenario-based-portfolio-allocation-newly-added)
- [Key Takeaways](#key-takeaways)
- [Key Insights from Scenario Analysis](#key-insights-from-scenario-analysis)
- [Strategic Implications](#strategic-implications)
- [Limitations and Future Directions](#limitations-and-future-directions)
- [Conclusion](#conclusion)
- [Bayesian Inference Primer](#bayesian-inference-primer)
- [Macro Economic Scenario Allocations](#macro-economic-scenario-allocations)
- [🚀 Recent Updates & Enhancements](#-recent-updates--enhancements)
- [Author](#author)
- [References](#references)
- [Project Structure](#project-structure)
- [Requirements](#requirements)

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

## Supplemental Analysis: Macroeconomic Scenario-Based Portfolio Allocation (Newly Added!)

In addition to our original quantitative models, we conducted an explicit scenario-based portfolio analysis to assess investment performance under different macroeconomic conditions (Base Case, Recession, Expansion). This supplemental analysis demonstrates how strategically adjusting allocations based on economic indicators can enhance returns and improve portfolio resilience.

### Supplemental Results (Macroeconomic Scenario Analysis - 2023)

| Economic Scenario | Portfolio Return | Final Portfolio Value (from $10M) | Outperformed S&P 500 (26.71%)? |
|-------------------|------------------|-----------------------------------|--------------------------------|
| **Recession**     | 28.33% 📈        | $12,832,768.71                    | ✅ Yes                         |
| **Base Case**     | 44.43% 🚀        | $14,443,489.52                    | ✅ Yes                         |
| **Expansion**     | 52.03% 🚀        | $15,203,148.33                    | ✅ Yes                         |

### Benchmark Performance (S&P 500 - SPY)

| Benchmark | Return | Final Value (from $10M) |
|-----------|--------|--------------------------|
| **SPY**   | 26.71% | $12,670,922.43           |

### Key Takeaways:
- Linear Regression clearly outperformed, delivering highest returns with good predictive accuracy.
- K-Means offered solid but comparatively lower performance.
- Bayesian Inference needs computational refinement but remains promising for risk-aware strategies.

### Key Insights from Scenario Analysis:
- **Base Case** allocations closely align with original Linear Regression results (44.43% returns), confirming strategic consistency.
- **Expansion scenario** achieved notably higher returns (52.03%), clearly emphasizing the effectiveness of aggressive allocations in strong economic conditions.
- **Recession scenario** performed well (28.33%), explicitly demonstrating strong defensive capabilities and resilience during economic downturns.

### Strategic Implications:
- **Dynamic Scenario Toggles**: Explicitly adjust classifications and allocations based on economic assumptions (**interest rates**, **volatility**).
- **Strategic Reallocation**: Clearly highlights explicit shifts between **growth-oriented**, **value-oriented**, and **income-oriented** strategies depending on scenario.
- **Enhanced Model Flexibility**: Demonstrates realistic, adaptive stock selection explicitly, enhancing portfolio resilience across market cycles.

## Limitations and Future Directions
- **Computational Efficiency**: Bayesian approach requires optimization for real-time use.
- **Feature Selection**: Expanding and refining financial data features could further enhance model accuracy.
- **Hybrid Models**: Exploring combinations of these models may yield superior investment strategies.

### Future Scenario Modeling Enhancements:
- Integration of advanced Bayesian macroeconomic forecasts to explicitly optimize allocations.
- Real-time adaptive portfolio strategies based on explicit economic indicator forecasting.

## Conclusion
This project demonstrates the significant potential of quantitative strategies to consistently outperform traditional passive benchmarks such as the S&P 500. Initially, Linear Regression emerged as the strongest performer, providing immediate, high-accuracy returns, while Bayesian methods showed promise for future refinement through their adaptability and explicit handling of uncertainty.

The supplemental macroeconomic scenario analysis further enhances these quantitative insights, explicitly demonstrating how portfolio allocations can be dynamically and strategically adjusted to economic conditions. This scenario-based approach not only validates the robustness of the original models but clearly highlights their flexibility and practicality in real-world investing, offering resilience in downturns (Recession scenario) and substantial growth potential in favorable conditions (Expansion scenario).

Overall, this structured, comparative approach provides investors with actionable, robust strategies and highlights the importance of adaptive, economically informed quantitative modeling for maximizing returns and managing risk across diverse market environments.

## Bayesian Inference Primer
Bayesian inference models uncertainty explicitly through probability distributions:

p(w \mid D) \propto p(D \mid w) \cdot p(w)

- **p(w)**: Prior distribution based on Linear Regression insights.
- **p(D | w)**: Likelihood based on observed financial data.
- **p(w | D)**: Posterior distribution offering dynamic stock selection and risk-aware decision-making.

The model optimizes an **Evidence Lower Bound (ELBO)** using variational inference to approximate complex posterior distributions.

## Macro Economic Scenario Allocations

![Portfolio Allocations by Scenario](scenario_allocations.png)

This visualization clearly demonstrates how portfolio allocations shift dynamically under different macroeconomic scenarios (Base Case, Recession, Expansion).

-**Dynamic Scenario Toggles**: Adjust classifications and allocations based on economic assumptions (interest rates, volatility).

-**Strategic Reallocation**: Highlights explicit changes in growth-oriented, value-oriented, and income-oriented strategies depending on scenario.

-**Enhanced Model Flexibility**: Shows how model-driven stock selection adapts realistically, improving portfolio robustness across market cycles.

## 🚀 Recent Updates & Enhancements:
- Implemented explicit scenario toggling to simulate varying market conditions.

- Dynamically adjusted stock-classification thresholds and allocations.

- Integrated clear visualizations to enhance interpretability and demonstrate strategic flexibility.

## Author
**John Grier**  
MS Data Science Candidate, Illinois Tech  
[GitHub: J-Grier](https://github.com/J-Grier)

## References
- Yahoo Finance historical data
- Zhao Gao, \"The application of artificial intelligence in stock investment\" (2020)
- Wikipedia: [S&P 500 Tickers](https://en.wikipedia.org/wiki/List_of_S%26P_500_companies)


## Project Structure

quantitative-stock-models/ ├── cleaned_QuantitativeModels.ipynb # Core analysis: Linear, K-Means, Bayesian models (initial results) ├── dynamic_allocation.ipynb # Supplemental macroeconomic scenario-based portfolio allocation analysis ├── README.md # Project overview, instructions, and results summary ├── requirements.txt # Environment dependencies ├── data/ # Optional data storage or links to external data sources └── images/ # Charts and visualizations

## Requirements

See `requirements.txt` for all package dependencies.

## Setup

```bash
# Clone repo
git clone https://github.com/J-Grier/quantitative-stock-models.git

# Create environment and install dependencies
pip install -r requirements.txt
