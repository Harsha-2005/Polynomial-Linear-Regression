# Polynomial-Linear-Regression
Polynomial regression is an extension of linear regression that models a non-linear relationship between an independent variable (x) and a dependent variable (y) by transforming the independent variable into a polynomial term (x^n)

# Polynomial Regression on the Auto MPG Dataset

## 📝 Overview

This project demonstrates the application of **Polynomial Regression** to model a non-linear relationship in a real-world dataset. We use the classic "Auto MPG" dataset to predict a car's fuel efficiency (Miles Per Gallon) based on its horsepower.

The notebook first fits a **Simple Linear Regression** model as a baseline to show its limitations with curved data. It then implements a **Polynomial Regression** model, which provides a significantly better fit, highlighting its strength in capturing non-linear trends.

---

## 📈 Final Result

The final output clearly shows the superior fit of the polynomial regression curve (green) compared to a standard linear model for this dataset.



---

## 💾 Dataset

* **Name**: Auto MPG
* **Source**: Loaded directly from the `seaborn` library.
* **Independent Variable (Feature)**: `horsepower`
* **Dependent Variable (Target)**: `mpg`

The dataset contains information about cars from the 1970s and 80s. The relationship between horsepower and MPG is inverse and non-linear—as horsepower increases, MPG decreases at a changing rate.

---

## 🛠️ Technologies & Libraries Used

This project is implemented in Python 3 and requires the following libraries:

* `pandas` for data manipulation.
* `numpy` for numerical operations.
* `matplotlib` and `seaborn` for data visualization.
* `scikit-learn` for building the regression models.

---

## 🚀 How to Run

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/](https://github.com/)<Harsha-2005>/<Polynomial-Linear-Regression>.git
    ```
2.  **Open the notebook:**
    The project is contained within a single Jupyter Notebook file (`.ipynb`). You can open and run it using:
    * Google Colab (recommended for ease of use)
    * Jupyter Notebook or JupyterLab
    * VS Code with the Python and Jupyter extensions.

3.  **Execute the cells:**
    Run the cells in the notebook sequentially from top to bottom.

---

## 📊 Model & Evaluation

Two models were built and compared:

1.  **Simple Linear Regression**:
    * This model attempts to fit a straight line to the data.
    * Result: It fails to capture the curve in the data, resulting in a low R-squared score and poor predictive performance.

2.  **Polynomial Regression (Degree 2)**:
    * This model transforms the `horsepower` feature into `horsepower` and `horsepower²`, allowing it to fit a parabolic curve.
    * Result: It provides a much better fit to the data, as evidenced by a significantly higher **R-squared ($R^2$) value**, and the visualization confirms its accuracy.
