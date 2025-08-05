# 🧱 Concrete Compressive Strength Analysis

This project performs a comprehensive statistical analysis on a dataset of concrete compressive strength using Python and its data analysis libraries.

## 📌 Objective

To understand how different components in a concrete mix affect its compressive strength by:
- Calculating statistical measures like mean and variance
- Visualizing distributions
- Computing confidence and tolerance intervals
- Performing hypothesis testing

## 👩‍💻 Team Members

- **Syeda Khadija Hassan**  — Frequency distribution, report writing, visualizations
- **Rida Syed**  —  built-in statistics & visualizations
- **Maryam Khan**  — Confidence & tolerance interval code

## 📊 Dataset

- Source: [Kaggle - Concrete Compressive Strength Dataset](https://www.kaggle.com/datasets/uciml/concrete-compressive-strength)
- Features: Amounts of concrete components (cement, water, fly ash, etc.)
- Target: Concrete compressive strength (MPa)

## 🛠️ Tools & Libraries

- Python 3
- Pandas
- NumPy
- Matplotlib
- SciPy
- Statistics (Python standard library)

## 🔬 Methodology

### 1. **Data Preparation**
- Loaded dataset using `pandas.read_csv()`
- Dropped rows with missing values
- Isolated the target variable

### 2. **Descriptive Statistics**
- Calculated mean & variance using:
  - Built-in methods
  - Frequency distribution with 100 bins

### 3. **Visualizations**
- Histogram of compressive strength
- Pie charts showing distribution in bins
- Annotated histograms with mean ± standard deviation

### 4. **Statistical Inference**
- **Confidence Interval** (95%):  
  - Mean ∈ [35.36, 37.76]  
  - Variance ∈ [280.28, 340.06]
- **Tolerance Interval (95%)**:  
  - Range = [2.14, 70.98]  
  - 99.51% of validation data within range
- **Hypothesis Testing**:  
  - H₀: μ ≤ 35 MPa  
  - H₁: μ > 35 MPa  
  - t = 2.548, p = 0.011 → Reject H₀

## 📈 Results

| Method                 | Mean (MPa) | Variance (MPa²) |
|------------------------|------------|-----------------|
| Built-in               | 35.817     | 279.08          |
| Frequency Distribution | 35.832     | 278.96          |

### Sample Distribution

| Strength Range (MPa) | Percentage |
|----------------------|------------|
| 7.91 - 22.9          | 22.1%      |
| 22.9 - 37.9          | 36.3%      |
| 37.9 - 52.9          | 26.1%      |
| 52.9 - 67.9          | 12.0%      |
| 67.9 - 82.9          | 3.4%       |

## 📌 Key Insights

- The dataset mostly falls within the 22.9–37.9 MPa range.
- Built-in and frequency-based statistics yield consistent results.
- Hypothesis testing confirms that the average compressive strength is significantly greater than 35 MPa.
- Tolerance interval validation shows strong generalizability.

## 📂 Project Files

- `project_analysis.ipynb` — Full implementation in Python
- `concrete_data.csv` — Original dataset from Kaggle
- `report.pdf` — Full project documentation and visualizations

## 📚 References

1. [Concrete Compressive Strength Dataset - Kaggle](https://www.kaggle.com/datasets/uciml/concrete-compressive-strength)  
2. McKinney, Wes. *Data Structures for Statistical Computing in Python*  
3. Hunter, J. D. *Matplotlib: A 2D Graphics Environment*  
4. Virtanen et al. *SciPy 1.0: Fundamental Algorithms for Scientific Computing in Python*

---

