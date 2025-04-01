# Synthetic Data Generation for Supervised Learner Comparison

## Project Overview  
This project involved generating synthetic datasets to evaluate the strengths and weaknesses of two supervised learning models: a **Linear Regression Learner** and a **Decision Tree Learner**. By controlling the data generation process, the project demonstrates how different learning algorithms are better suited to specific types of relationships between features and target variables. The work emphasizes the importance of data structure and function complexity when selecting machine learning models.

**Languages/Tools Used:** Python, NumPy  
**Key Concepts:** Supervised Learning, Synthetic Data Generation, Linear Regression, Decision Trees, Model Evaluation, Reproducibility

---

## Project Objectives
- Implement custom dataset generators to:
  - Favor **Linear Regression** over **Decision Trees**
  - Favor **Decision Trees** over **Linear Regression**
- Ensure deterministic output using random seeds for reproducibility
- Avoid trivial or hardcoded targets by generating meaningful, function-based Y values
- Demonstrate that no single learner universally outperforms others—model performance depends on the data

---

## Technical Highlights
- Developed two key functions:
  - `best_4_lin_reg(seed)` — generates data where a linear model significantly outperforms a decision tree
  - `best_4_dt(seed)` — generates data where a decision tree significantly outperforms a linear model
- Used mathematical functions (linear and nonlinear) to define relationships between input features and output targets
- Ensured Y is computed based on X (no hardcoded outputs)
- Generated data with 2–10 feature columns and 10–1000 examples per dataset
- Reproducibility guaranteed via seeding and pure NumPy-based generation
- No external file reading or learner importing allowed per constraints

---

## Value & Learning Outcomes
- Strengthened understanding of **bias-variance tradeoffs** and how learner assumptions affect performance  
- Gained practical experience in **constructing datasets** tailored to test model suitability  
- Reinforced concepts in **function approximation**, **non-linearity**, and **generalization**  
- Practiced clean, controlled experimentation without external dependencies

---

## Repository Access  
Due to academic policy, the full implementation—including code and generated dataset logic—is stored in a private GitHub repository. **Access available upon request.**
