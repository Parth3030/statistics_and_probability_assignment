# Airline Passenger Satisfaction - Descriptive Statistics & Distribution Analysis

An end-to-end descriptive analytics and statistical modeling project implemented inside a local Python development environment. This project focuses on auditing, parsing, and building a mathematical baseline for airline operational metrics by extracting core central tendencies, variation parameters, and structural distributions from real-world customer flight logs.

## 🚀 Key Project Assets
* **Core Workspace:** `Statistics and Probability.ipynb`
* **Technical Stack:** Python 3, Pandas, NumPy, Matplotlib
* **Core Column Analyzed:** `Flight Distance`

---

## 📊 Business Context & Analytics Objective
For airline operations, analyzing passenger flight behavior is critical to predicting cabin wear, service resource allocation, and frequent flyer profiling. 

This project processes an industry database across a numerical vector space (**Flight Distance**) to isolate exact statistical behaviors. By establishing clear mathematical parameters, the business can accurately assess structural shifts in travel lengths and understand the true shape of day-to-day flight operations.

---

## 🛠️ Implemented Technical & Statistical Workflows

The notebook systematically calculates and implements **7 distinct statistical properties** to define the dataset's baseline profile:

### I. Central Tendencies
* **1. Mean ($\mu$):** Evaluated at **1,190.32 miles**. This marks the mathematical balance point of all recorded passenger flight paths.
* **2. Median:** Evaluated at **844.0 miles**. This captures the absolute 50th percentile mark, splitting the dataset directly in half.
* **3. Mode:** Evaluated at **337 miles**. This identifies the single most frequently occurring flight distance within the carrier's logs.

### II. Dispersion & Variance Analytics
* **4. Variance ($\sigma^2$):** Calculated as **994,911.44**. This measures the absolute internal spread and squared deviations of individual flights away from our operational mean.
* **5. Standard Deviation ($\sigma$):** Calculated as **997.45 miles**. This benchmarks the standard volatility and dispersion, indicating how far typical flights stray from the center.
* **6. Standard Error of the Mean (SEM):** Evaluated at **2.77**. This quantifies sample mean precision, mathematically proving that our calculated sample average is exceptionally stable and true to the wider population.

### III. Continuous Curve Fitting
* **7. Normal Distribution Modeling:** Custom-built an empirical data frequency histogram and overlaid it with a calculated **Continuous Normal Distribution Curve** using `matplotlib`. This provides immediate visual proof of how closely real-world commercial logs align with a theoretical ideal bell curve.

---

## 💡 Key Analytical Insights & Skewness Findings

* **The Regional Flight Skew:** The significant margin separating the Mode (`337.0` miles), Median (`844.0` miles), and Mean (`1,190.32` miles) reveals a classic **Right-Skewed Distribution** ($Mode < Median < Mean$). 
* **Operational Implication:** The airline's daily schedule is heavily anchored by ultra-high-frequency, short-distance regional commutes (hence the low mode). However, a minor, spread-out cluster of long-haul transoceanic flights pulls the mathematical average significantly upward.
