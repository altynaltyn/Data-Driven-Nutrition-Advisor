# Data-Driven Nutrition Advisor

### Turning Dietary Guidelines into Realistic Weekly Shopping Baskets

---

## Project Summary

This project converts the **Harvard Healthy Eating Plate** framework into **real, purchasable weekly grocery baskets** using actual retail prices from Almaty.

It bridges the gap between:

* Nutritional theory
* Budget constraints
* Real-world package sizes

The output is a fully transparent, rule-based system that generates **balanced, cost-estimated weekly shopping lists**.

---

## Business Problem

Healthy eating guidelines define proportions (50% vegetables, 25% protein, 25% grains) but ignore:

* Product prices
* Package sizes
* Budget feasibility
* Store-level availability

This project transforms abstract proportions into **economically feasible shopping decisions**.

---

## Method

**1️ Data Collection**
Manual product data from Arbuz.kz (price, weight, macronutrients).

**2️ Price Standardization**

```math
P_{100} = \frac{Price}{Weight} \times 100
```

**3️ Basket Strategies**

*  **Budget** – minimizes total cost
*  **Standard** – balances cost and diversity
*  **Premium (Value-Based)** – maximizes protein per price

```math
ValueScore = \frac{Protein_{100g}}{Price_{100g}}
```

**4️ Package-Level Realism**

```math
Packages = \left\lceil \frac{Required\_grams}{Package\_weight} \right\rceil
```

No fractional purchases — fully realistic baskets.

---

##  Key Insight

Redefining “Premium” from *most expensive products* to *highest nutritional value per price* reduced total basket cost from:

**~199,000 KZT → ~28,000 KZT**

The quantity did not change.
Only the optimization logic changed.

This highlights how metric definition directly impacts economic outcomes.

---

## Results

* Protein drives the majority of total cost
* Vegetables offer high volume at low price
* Value-based optimization dramatically improves affordability
* Cost increases monotonically with protein share

---

##  Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib

✔ Fully interpretable
✔ No black-box ML
✔ Reproducible pipeline

---

##  Why This Project Matters

This work demonstrates:

* Translating theory into measurable systems
* Economic modeling under constraints
* Data-driven decision support
* Interpretable optimization logic

It showcases strong fundamentals in **data analysis, modeling, and structured problem-solving**.


