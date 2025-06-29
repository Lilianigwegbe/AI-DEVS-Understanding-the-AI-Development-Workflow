# 🧠 Part 3: Critical Thinking — Ethics & Trade-offs in AI for Healthcare

## ⚖️ Ethics & Bias

### How might biased training data affect patient outcomes in the case study?

Biased training data can lead to significant disparities in patient outcomes. If the dataset used to train the AI model overrepresents certain demographics (e.g., adults, males, or patients from urban regions) and underrepresents others (e.g., children, females, rural populations), the model might learn patterns that do not generalize well to underrepresented groups. This could result in:

- Misdiagnosis or delayed diagnosis for minority groups.
- Ineffective or inappropriate treatment recommendations.
- Reinforcement of existing healthcare disparities.

**Example:**  
If a diagnostic AI tool is trained mostly on data from patients with lighter skin tones, it may perform poorly in detecting skin conditions in patients with darker skin tones.

### ✅ Strategy to Mitigate Bias

Use **stratified sampling and data augmentation** to ensure diverse and representative training data. Additionally, conduct **fairness audits** to test the model's performance across different subgroups (e.g., age, gender, ethnicity) and apply **re-weighting or re-sampling** techniques during model training to reduce bias.

---

## 🔁 Trade-offs

### What is the trade-off between model interpretability and accuracy in healthcare?

In healthcare, **model interpretability** is crucial because clinicians need to understand and trust the system’s recommendations to make informed decisions. However, **highly accurate models**, like deep neural networks, often act as black boxes and lack transparency.

- **Interpretable models** (e.g., decision trees, logistic regression):
  - ✅ Easier to understand and trust.
  - ❌ May sacrifice accuracy on complex tasks.
  
- **Highly accurate models** (e.g., deep learning, ensemble methods):
  - ✅ Better performance on complex predictions.
  - ❌ Harder to explain, making them less trusted by medical professionals.

A **balanced approach**—such as using explainable AI (XAI) techniques like **SHAP values** or **LIME**—can help make complex models more interpretable.

---

### How might limited computational resources impact model choice?

In a resource-constrained environment, hospitals may need to choose:

- **Lightweight models** (e.g., decision trees, logistic regression) that can run efficiently on standard CPUs or edge devices.
- Avoid complex, computationally expensive models (like deep learning networks) that require GPUs or high memory.

This means sacrificing some predictive power for **cost-effectiveness and speed**, especially in settings where real-time predictions or offline access are needed.

---
