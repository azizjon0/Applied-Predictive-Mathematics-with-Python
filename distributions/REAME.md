## 📊 Normal vs Abnormal Distributions — Core Concepts

### 🔹 What is a **Normal Distribution**?
A **bell-shaped** distribution where:

- Most values are **centered around the mean (μ)**.
- The farther from the mean, the **less frequent** the values.
- It's **symmetrical** and smooth.
- Fully defined by two parameters:
  - **μ (mean)** — the center.
  - **σ (standard deviation)** — the spread.

> ✅ Common in real life: human height, IQ scores, measurement errors.

---

### 🔹 What is an **Abnormal Distribution**?
Any distribution that **does not follow the bell curve**:

- 🔸 **Skewed** – asymmetric (long tail to the left or right).
- 🔸 **Multimodal** – multiple peaks.
- 🔸 **Heavy-tailed** – outliers occur more frequently.

> ⚠️ These distributions often violate assumptions of standard ML models.

---

### 🔹 When to Use Normal Distribution?

Use **normal distribution** when:

- ✅ Data is **naturally symmetric and unimodal**.
- ✅ You’re using models that assume normality:
  - Linear Regression
  - PCA
  - Gaussian Naive Bayes

Avoid using it when:

- ❌ Data is **skewed**, **multimodal**, or contains **outliers**.
- ➤ Instead, apply:
  - **Transformations** (e.g., log, Box-Cox),
  - **Robust models** (e.g., Random Forest, XGBoost).

---

### 🔹 Parameters Required to Build a Distribution

You only need two:

- `μ` — **Mean** (location of the peak),
- `σ` — **Standard deviation** (spread/width of the curve).

These two fully define the shape of a normal distribution.

---

### 🔹 Where is Normal Distribution Used in ML / AI?

| Use Case                          | How It's Used                                         |
|-----------------------------------|--------------------------------------------------------|
| **Gaussian Naive Bayes**          | Assumes normal distribution for continuous features    |
| **PCA (Principal Component Analysis)** | Assumes normality for optimal component separation  |
| **Linear Regression**             | Assumes residuals follow a normal distribution         |
| **VAE (Variational Autoencoder)** | Uses Gaussian latent space for sampling                |
| **Neural Net Initialization**     | Weights often initialized from normal distribution     |
| **Gaussian Mixture Models (GMM)** | Clusters modeled as multiple normal distributions      |

---
