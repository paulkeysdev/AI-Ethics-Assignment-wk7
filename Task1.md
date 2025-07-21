## 🧠 Case 1: Biased Hiring Tool – Amazon

### 🔍 **Scenario Summary**

Amazon developed an AI recruiting tool to screen resumes. However, it was discovered that the system penalized female candidates. The model downgraded resumes containing words like "women's" (e.g., “women’s chess club captain”) and favored male-dominated terms due to patterns in historical hiring data.

---

### 📌 Task 1: Identify the Source of Bias

**Primary Source of Bias:**

* **Training Data Bias:** The model was trained on 10 years of Amazon's past hiring data, which reflected male-dominated hiring patterns—especially in technical roles.
* **Historical Discrimination Replication:** Because men were hired more frequently in the past, the AI learned to associate "maleness" with success.
* **Feature Representation Bias:** Gender-specific terms (e.g., "women’s", female college names) were treated as negative signals.

---

### 🛠 Task 2: Propose Three Fixes to Make the Tool Fairer

1. **Debias the Training Data:**

   * Remove or anonymize gendered indicators (e.g., names, gendered pronouns, associations like “women's club”) before training.
   * Rebalance the dataset to ensure diverse representation across gender and roles.

2. **Introduce Fairness Constraints During Model Training:**

   * Use fairness-aware algorithms that constrain discriminatory patterns (e.g., reject options that lead to disparate impact).

3. **Human-in-the-Loop Systems:**

   * Supplement AI decisions with diverse human reviewers, especially for edge cases or sensitive applications.
   * Provide explainability tools so HR teams understand why a candidate was rejected.

---

### 📏 Task 3: Suggest Fairness Metrics Post-Correction

To measure fairness after applying fixes:

1. **Disparate Impact Ratio (DIR):**

   * Measures if protected groups (e.g., women) are selected at a similar rate as the privileged group.
   * Ideally, DIR should be between 0.8 and 1.25 (the 80% rule).

2. **Equal Opportunity Difference:**

   * Compares true positive rates between groups to ensure qualified individuals are treated equally.

3. **False Negative Rate Parity:**

   * Checks if qualified candidates from different groups are equally likely to be incorrectly rejected.
   ![image alt](https://github.com/paulkeysdev/AI-Ethics-Assignment-wk7/blob/6e5a64cfde608747642e2dfb200eb5d0bc92ad56/IMGS/ChatGPT%20Image%20Jul%2021%2C%202025%2C%2004_29_52%20PM.png)

