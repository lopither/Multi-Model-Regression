# 📘 Multi-Model-Regression
 
### Advanced Mathematical Modeling, Curve Fitting, and Analysis Tool  
**Powered by Wolfram Mathematica**

MathModelingSuite is a complete, professional-level mathematical analysis tool designed to help students, researchers, data scientists, and engineers visualize, model, and understand complex datasets using symbolic and numerical approaches.

It automatically detects the best polynomial model, compares multiple regression techniques, computes calculus properties, finds roots, performs symbolic regression, and exports full high-quality PDFs containing everything generated in the environment.

---

# 🚀 Features Overview

Multi-Model-Regression includes more than 25 advanced mathematical capabilities.

---

## 🔹 1. **Automatic Best Polynomial Fit**
- Tests all polynomial orders from 1 to \( n-1 \) automatically  
- Selects the degree with the **highest R² score**  
- Outputs:
  - Clean symbolic polynomial  
  - Coefficient list (highest → constant)  
  - Full, train, and test R²  
- Automatically builds:
  - Derivative  
  - Critical points  
  - Plot with maxima/minima annotated  

---

## 🔹 2. **Supported Regression Models**

Every model includes R²(all), R²(train), R²(test):

| Model | Description |
|-------|-------------|
| **Polynomial (Auto degree)** | Fits \( \sum_{k} a_k x^k \) |
| **Exponential** | Fits \( a e^{b x} \) |
| **Logarithmic** | Fits \( a \ln(x) + b \) |
| **Power** | Fits \( a x^b \) |
| **Rational** | Fits \( (ax^2+bx+c)/(dx+e) \) |
| **Logistic** | Fits \( L / (1 + e^{-k(x-x_0)}) \) |
| **Fourier (order 4)** | Fits sinusoidal + cosinusoidal components |
| **Symbolic Regression** | Uses `FindFormula` to discover closed-form equations |

Each model is computed using training/testing split (80/20).

---

## 🔹 3. **Symbolic Regression**
Using Mathematica’s AI-assisted symbolic reasoning:

```wl
FindFormula[Transpose[{xs, ys}], x]
