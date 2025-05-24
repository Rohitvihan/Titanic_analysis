# 🚢 Titanic Data Analysis with Seaborn & Pandas 🐍

This project explores the famous Titanic dataset using **Pandas**, **Seaborn**, and **NumPy**. We clean, transform, and visualize the data to better understand passenger survival patterns and demographics. 📊

---

## 📁 Project Structure

* **📄 Jupyter Notebook**: Contains all preprocessing and visualization steps.
* **📈 Visualizations**: Insights on age distribution, passenger class, gender, and survival rates.

---

## 🔧 Steps Performed

### 1. 🧹 Data Cleaning

* Dropped irrelevant columns: `who`, `deck`, `embark_town`, `adult_male`, `fare`, `parch`, `alone`
* Mapped categorical values to numeric:

  * `sex`: male → 1, female → 0
  * `alive`: yes → 1, no → 0
  * `embarked`: C → 0, Q → 1, S → 2
  * `class`: First → 1, Second → 2, Third → 3
* Filled missing values:

  * `age`: with median
  * `embarked`: with mode

> ⚠️ Note: Warnings were raised due to chained assignment. Future versions of Pandas may require a different approach (e.g., `df.loc[:, 'col'] = df['col'].fillna(...)`).

---

### 2. 📊 Visualizations

* 🔥 **Heatmap**: General data overview
* 📦 **Boxplot**: Age distribution by sex
* 📉 **Histogram**: Distribution of age (with KDE)
* 📊 **Countplot**: Passenger count per class

---

## 📦 Requirements

Install the following Python packages to run the project:

```bash
pip install pandas numpy seaborn matplotlib
```

---

## 🚀 Run it Yourself

1. Clone the repository
2. Open the `.ipynb` file in Jupyter Notebook or JupyterLab
3. Run all cells to see the transformations and visualizations

---




