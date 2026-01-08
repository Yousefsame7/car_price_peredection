# car_price_peredection
A model to predict the price of a used car 
Here are the **tools & libraries used in your code**, simply listed 👇

### 📦 Python Libraries

1. **pandas**

   * Data loading, cleaning, preprocessing

   ```python
   import pandas as pd
   ```

2. **numpy**

   * Numerical operations, arrays

   ```python
   import numpy as np
   ```

3. **matplotlib**

   * Data visualization (plots, charts)

   ```python
   import matplotlib.pyplot as plt
   ```

4. **seaborn**

   * Advanced statistical visualizations (heatmaps, distributions)

   ```python
   import seaborn as sns
   ```

5. **scikit-learn (sklearn)**

   * Machine Learning models & evaluation

   ```python
   from sklearn.ensemble import RandomForestRegressor, ExtraTreesRegressor
   from sklearn.model_selection import train_test_split, RandomizedSearchCV
   from sklearn.metrics import (
       mean_squared_error,
       mean_absolute_error,
       r2_score,
       confusion_matrix,
       classification_report,
       accuracy_score
   )
   ```

6. **pickle**

   * Save/load trained ML model

   ```python
   import pickle
   ```

7. **warnings**

   * Suppress warning messages

   ```python
   import warnings
   ```

---

### 🛠 Tools / Environment

* **Jupyter Notebook** (because of `%matplotlib inline`)
* **Python 3**
* **CSV dataset** (`car data.csv`)

---

### 📥 Install all required libraries (one command)

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

If you want, I can also:

* Explain **what each library does in 1 line**
* Give a **requirements.txt**
* Or **simplify the whole pipeline** 👍

The **model** used in your code is:

### ✅ **Random Forest Regressor**

Specifically from **scikit-learn**:

```python
from sklearn.ensemble import RandomForestRegressor
```

🔹 You also used **ExtraTreesRegressor** earlier, but **the final trained and saved model** is:

➡️ **RandomForestRegressor with RandomizedSearchCV** (hyperparameter tuning)

### Final Model (simple explanation)

* **Type:** Supervised Machine Learning
* **Task:** Regression (predicting car **Selling_Price**)
* **Algorithm:** Ensemble of decision trees
* **Final object saved:**

```python
pickle.dump(rf_random, file)
```

So the **actual model** is:

> **Tuned Random Forest Regression model**

If you want it **even simpler**:

> 🌳🌳🌳 Many decision trees voting together to predict car price.

Let me know if you want:

* Difference between **Random Forest vs Extra Trees**
* Model explanation for **presentation**
* Or **how to load & use the saved model**
### Simple explanation of the project 👇

**Project idea:**
Predict the **selling price of a used car** using machine learning.

---

### What the project does

* Takes car details مثل:

  * car age
  * current price
  * kilometers driven
  * fuel type
  * transmission type
* Uses these details to **predict the car’s selling price**.

---

### How it works (very simple)

1. **Load data** from a CSV file (car data).
2. **Clean & prepare data**

   * Remove unused columns
   * Convert text (Petrol, Diesel, Manual…) into numbers
   * Create a new feature: **car age**
3. **Analyze data**

   * Check correlations
   * Draw graphs and heatmaps
4. **Train the model**

   * Use **Random Forest Regressor**
   * Learn patterns from old car prices
5. **Test the model**

   * Compare predicted price vs real price
6. **Save the model**

   * Store it using `pickle` to use later

---

### Model used

* **Random Forest Regressor**
* Predicts prices by combining results from many decision trees

---

### Result

* The model predicts car prices with **high accuracy (R² ≈ 0.92)**

---

### One-line summary (perfect for presentation)

> This project uses machine learning to predict used car prices based on car features like age, fuel type, and mileage.

If you want:

* **Short explanation for viva**
* **Slides explanation**
* **Arabic explanation**
