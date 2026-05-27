# Airline Operational Analytics: Statistical Modeling & Probability Distributions

An end-to-end mathematical data analysis project conducted in a local Python development environment to model airport operational metrics. By assessing baseline descriptive characteristics and fitting continuous theoretical curves (Normal Distribution), this project transforms empirical flight logs into active probability models to determine risk thresholds and structural flight profiles.

## 🚀 Repository Assets
* **Core Workspace:** `Statistics and Probability (1).ipynb`
* **Technical Framework:** Python 3, Pandas, NumPy, Matplotlib, SciPy (`scipy.stats`)
* **Mathematical Applications:** Continuous Probability Density Functions (PDF), Parameter Estimation, Z-Score Intercepts, Right-Skewness Analysis

---

## 📊 Business Framework & Objective
For logistical hubs and airline carriers, calculating the spatial behavior of flights is foundational to resource allocation, fuel planning, and fleet routing. 

This project explores an enterprise database consisting of **24 performance columns** (including traveler categories, seating layout satisfaction, and downstream delay minutes). The core focus lies in extracting **Flight Distance** metrics to develop a rigorous mathematical baseline that calculates standard operational probabilities.

---

## 🛠️ Workspace Pipeline & Math Implementation

### 1. Parametric Data Auditing
Using `pandas`, raw consumer profiles are imported programmatically and checked. Central locations and dispersion limits are calculated directly from the core vector array:
* **Mathematical Mean ($\mu$):** `1190.32` miles, pinpointing the global balancing point of flight records.
* **Statistical Median:** `844.0` miles, capturing the exact 50th percentile mark.
* **Sample Variance ($\sigma^2$):** `994,911.44` (indicating high dispersion across regional and long-haul vectors).
* **Standard Deviation ($\sigma$):** `997.45` miles, tracking the average deviation around our operating mean.
* **Standard Error (SEM):** `2.77`, proving high stability and low variance in our global population mean.

### 2. Theoretical Continuous Distribution Fitting
To determine if operations follow a standard bell shape, the system maps out an empirical frequency density histogram overlaid with a custom continuous **Normal Probability Density Function (PDF)** using `scipy.stats.norm.pdf()`:

$$\mu = 1190.32, \quad \sigma = 997.45$$

$$f(x) = \frac{1}{997.45\sqrt{2\pi}} e^{-\frac{1}{2}\left(\frac{x - 1190.32}{997.45}\right)^2}$$

### 3. Z-Score Framework
By creating smooth continuous lines over real-world operational distributions, the workspace establishes a platform for calculating left-tail, right-tail, and step-wise interval probabilities:
* **Z-Score Formula:** $Z = \frac{X - \mu}{\sigma}$
* **Probability Metrics:** Solves cumulative area spaces under the fitted curve using the theoretical parameters.

---

## 💡 Core Insights & Skewness Findings

* **The Right-Skewed Operational Profile:** The immense gap between the calculated Median (`844.0` miles) and Mean (`1190.32` miles) indicates a distinct right-skewed distribution. The carrier's daily flights are heavily packed with high-frequency, short-distance regional tracks, while an isolated tail of high-mileage intercontinental flights pulls the mathematical average higher.
* **Friction Overlays:** By mapping continuous variables against discrete consumer response metrics, the pipeline tracks how physical properties (like long-range distances and late terminal delays) drive down base sentiment.
