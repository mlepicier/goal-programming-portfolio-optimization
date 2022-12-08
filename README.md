# Goal-Programming Portfolio Optimization

![readme-banner](https://user-images.githubusercontent.com/108199052/206316952-7d84c2d8-4ae6-4a72-b046-b722119d17de.jpg)

## Abstract:

<p align="justify">This project consists of using a goal-programming approach to a non-linear multi-objective optimization problem to create a financial stock portfolio maximizing valuation return while minimizing both volatility and unsystematic risks. This project was conducted from September 2022 to December 2022 as a student at <b>Ivey Business School</b>. Below are a few paragraphs to give you context about the project.</p> 

## Repository Assets:

- [Goal-Programming Portfolio Optimization Model](model/) - [Full Code](model/goal-programming-portfolio-optimization.ipynb)
- [Datasets](data/)

## Business Context:

<p align="justify"> <b>Quantitative Finance</b> overlaps heavily with <b>Operations Research</b>. Indeed, <b>Mathematical Optimization</b> serves investors well in improving their <b>Portfolio Management</b> practices. Since <i>Markowitz' 1952</i> paper, <b>Portfolio Optimization</b> falls under the <b>Multi-Objective</b> umbrella of operations research. In fact, regardless of the measures used, investors always deal with the well-known return-risk trade-off. Ultimately, this decision is up to the investor based on their preferences, often referred to as "risk profiles". We will address the need for minimization of the unsystematic risk in portfolio-building pointed out by the Covid-19-related financial crisis, while addressing the classic risk-return trade-off respictively assessed as volatility and capital valuation.</p>

## Problem Description:

<p align="justify"> <b>Goal Programming</b> is a commonly-used approach for multi-objective optimization. This approach consists of solving an <b>Linear Problem</b> for every single antithetical objective and storing the optimal solution as a benchmark of the best achievable result with regard to this respective objective. The next step involves minimizing the "deviations" of the final solution against every single benchmark. It is necessary to assess every objective in the same unit or same order of magnitude, weights attributed to these objectives can also be fine-tuned to reflect the decision maker preferences.  </p>

<p align="justify"> This study uses <i>Shannon's</i> Entropy as a measure of diversification to be maximized. Shannon's Entropy however, is not linear, which prevents us from feeding it into an LP as we did before, nonetheless, we know that this concave function finds its maximum value for a value of $x=ln(n)$. In this project, we will use the CPLEX Solver for the Linear-Programming and use a derivative of the <b>Stochastic Gradient Descent Algorithm</b> to optimize Non-Linear-Programming models proposed by SciPy as Sequential Least Square Programming. Finally we will proceed to Monte-Carlo Randomized-Moving-Block-Bootsrapping for the Cross-Validation stage.</p>

## Project Requirements
```
pip install pandas
pip install pandas-datareader
pip install plotly==5.3.1
pip install scipy
pip install docplex
pip install seaborn
pip install statsmodels
pip install numpy
pip install matplotlib
```

***

<i>Should you have any question, feel free to write me an [email](mailto:mlepicier.msc2022@ivey.ca), I am always happy to help.</i>