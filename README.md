# Statistical Modeling & Probability Distribution Analysis

An exploratory and mathematical data analysis project conducted in a local Python environment to apply probability theory to real-world operational data. By evaluating central tendencies, computing sample variance properties, and fitting continuous probability distributions (Normal Distribution), this project demonstrates how to translate raw data distributions into predictive, statistical models.

## 🚀 Key Deliverables
* **Main Analysis Notebook:** `Statistics and Probability.ipynb`
* **Core Technical Stack:** Python 3, Pandas, NumPy, Matplotlib, SciPy (`scipy.stats`)
* **Core Concepts:** Descriptive Statistics, Normal Distribution Fitting, Z-Score Calculations, Probability Density Functions (PDF)

---

## 📊 Business & Analytical Context
Understanding the probability distribution of organizational metrics (such as flight distances, delivery times, or transaction values) allows businesses to project risks, estimate capacity requirements, and calculate exact operational probabilities. 

This project takes a continuous numerical feature (**Flight Distance**) and builds a statistical framework to analyze its spread, assess its behavior against a theoretical bell curve, and calculate precise interval probabilities.

---

## 🛠️ Technical Workflow & Implementation

### 1. Statistical Baseline & Parameter Estimation
Using `numpy` and `pandas`, the system extracts key parameters from the sample population to define our distribution:
* **Mean ($\mu$):** Calculated as **~1190.32 miles**, establishing the balance point of the dataset.
* **Standard Deviation ($\sigma$):** Calculated as **~997.45 miles**, showing a wide operational dispersion across short and long-haul categories.
* **Standard Error (SEM):** Evaluated at **2.77**, indicating exceptionally high sample mean stability.

### 2. Probability Density Function (PDF) Modeling
* Built a theoretical **Normal Distribution Curve** using `scipy.stats.norm.pdf()` based on the estimated sample mean ($\mu$) and standard deviation ($\sigma$).
* Overlaid the continuous probability curve onto an empirical frequency histogram using `matplotlib` to visually inspect skewness and deviation from standard normality.

### 3. Z-Score & Interval Probability Calculations
Using cumulative distribution functions (`scipy.stats.norm.cdf()`), the project calculates exact probabilities for operational thresholds:
* **Left-Tail Probabilities:** Calculating the statistical likelihood of an event falling below a specific target value ($P(X \le x)$).
* **Interval Probabilities:** Subtracting cumulative bounds to find the exact probability of an asset falling within a specific operational range ($P(x_1 \le X \le x_2)$).

---

## 💡 Key Analytical Insights

* **Distribution Shape and Skewness:** While the theoretical normal curve assumes perfect symmetry, comparing the empirical data histogram to the generated PDF reveals a classic right-skewed distribution. The standard median sits significantly lower than the statistical mean, indicating that regional, short-distance metrics dominate daily operations.
* **Predictive Value of CDF:** By mapping data to a continuous distribution model, the business can rapidly calculate baseline probabilities for any arbitrary metric without needing to manually resample the entire database.

---

## ⚙️ Local Environment Setup

This project runs entirely on a clean, local Python environment using standard terminal execution.

1. **Clone the Project Repository:**
   ```bash
   git clone [https://github.com/your-username/statistical-probability-modeling.git](https://github.com/your-username/statistical-probability-modeling.git)
   cd statistical-probability-modeling
