# Linear Regression with Custom Training Loops in TensorFlow

This project demonstrates a **from-scratch implementation of Linear Regression** using TensorFlow's **low-level API** and **custom training loops** with `tf.GradientTape`. It focuses on understanding the step-by-step mechanics of model training without relying on high-level APIs like `model.fit()`.

---

## 1. Problem Statement and Goal of Project

The objective of this project is to gain **granular control** over the training process of a simple machine learning model. While high-level frameworks are efficient, understanding the low-level mechanics is crucial for:

* Implementing non-standard loss functions
* Debugging model behavior
* Extending to advanced models

The specific goal is to:

1. Implement **Linear Regression** from scratch using TensorFlow.
2. Train the model using a **custom gradient calculation and weight update loop**.
3. Compare predictions with actual values to validate correctness.

---

## 2. Solution Approach

The project follows a clear progression:

* **Data Preparation:**

  * Generates synthetic linear data with added noise for demonstration.
  * Normalizes inputs for stable gradient updates.
* **Model Definition:**

  * Defines trainable weights (`W`) and bias (`b`) as `tf.Variable`.
* **Loss Function:**

  * Uses **Mean Squared Error (MSE)** for regression performance measurement.
* **Training Loop (Custom):**

  * Implements `tf.GradientTape` to compute gradients manually.
  * Applies gradients with a TensorFlow optimizer (`SGD`).
  * Tracks loss evolution over epochs.
* **Evaluation:**

  * Visualizes predicted vs actual values.
  * Displays loss reduction over time.

---

## 3. Technologies & Libraries

* **Frameworks:** TensorFlow (Low-Level API)
* **Libraries:** NumPy, Matplotlib
* **Tools:** Jupyter Notebook

---

## 4. Description about Dataset

* **Type:** Synthetic dataset generated for linear regression.
* **Structure:** Single feature (`X`) and target (`y`) with linear relationship + noise.
* **Purpose:** Educational demonstration of regression training mechanics.

---

## 5. Installation & Execution Guide

```bash
# 1. Clone the repository
git clone https://github.com/imehranasgari/your-repo-name.git
cd your-repo-name

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter Notebook
jupyter notebook
```

Open and run the cells in `linear_regression_training_loops_me.ipynb`.

---

## 6. Key Results / Performance

* Successful implementation of a **custom training loop** without using `model.fit()`.
* Loss consistently decreases over training epochs, confirming correct gradient computation and parameter updates.
* Final model accurately fits the generated linear data.

---

## 7. Screenshots / Sample Output

*(Use your own saved plots from the notebook — suggested examples include:)*

* Plot of **loss vs epochs**
* Plot of **predicted line vs actual data points**

---

## 8. Additional Learnings / Reflections

* Reinforced understanding of `tf.GradientTape` and gradient flow.
* Gained insights into manual optimizer steps and their effect on convergence.
* This foundational workflow is directly extendable to complex deep learning models.

---

## 👤 Author

**Mehran Asgari**
**Email:** [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com)
**GitHub:** [https://github.com/imehranasgari](https://github.com/imehranasgari)

---

## 📄 License

This project is licensed under the MIT License – see the `LICENSE` file for details.

---

> 💡 *Some interactive outputs (e.g., plots, widgets) may not display correctly on GitHub. If so, please view this notebook via [nbviewer.org](https://nbviewer.org) for full rendering.*

---
