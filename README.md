# 🐟 Not So Fishy After All!
### Visualizing Healthiest Seafood Options for Endometriosis

**Author:** Gabrielle Despaigne  
**Course:** DSC 209R – Data Visualization  
**Date:** October 2025  

---

## 📖 Project Overview

This project explores the relationship between seafood choices and anti-inflammatory benefits for individuals with endometriosis. Endometriosis is a chronic inflammatory condition that affects 1 in 10 women of reproductive age worldwide. Since diet plays a major role in managing inflammation, this visualization highlights which types of fish are the most beneficial, or harmful, to an anti-inflammatory diet.

Using a cleaned and preprocessed nutrition dataset, this project introduces a custom **Anti-Inflammation Index (AII)** to quantify how inflammatory each food is. The visualization helps endometriosis patients, and anyone seeking anti-inflammatory diets, make better seafood purchasing decisions at grocery stores.

---

## 🎯 Objectives

- Identify and visualize which fish products align with an anti-inflammatory diet  
- Compare fish preparations, fresh versus tinned versus processed or frozen  
- Present an intuitive and scientifically grounded visualization that simplifies complex nutrition data  

---

## 🧮 Methodology

### 1) Data Exploration and Cleaning
- Removed null entries and duplicate rows  
- Standardized nutrition features to z-scores for comparability  

### 2) Feature Engineering
**Anti-Inflammation Index (AII)** constructed with weighted nutrients:
- Positive, anti-inflammatory: Fiber, Protein  
- Negative, pro-inflammatory: Carbohydrates, Sugar, Sodium, Food Processing Score (Fpro)  

Each product received an AII score and was categorized into health zones: beneficial, neutral, or harmful.

### 3) Seafood Categorization
- Filter to seafood categories only, including whole food seafood  
- Rename to `sf-pckged` for packaged or processed and `sf-fresh` for fresh whole food  
- Add preparation type: fresh, tinned, processed or frozen  

### 4) Aggregation and Visualization
- Aggregate by item label to compute mean **AII** and **Fpro**  
- Scatter plot with:
  - x axis: Food Processing Score (Fpro)  
  - y axis: Anti-Inflammation Index (AII)  
  - color: fish species  
  - background bands: health impact zones for quick read  

---

## 📊 Insights

- Fresh fish clusters in the beneficial zone, indicating stronger anti-inflammatory potential  
- Tinned fish generally falls in the neutral region  
- Processed or frozen fish tends to be more inflammatory, often linked to higher sodium and processing scores  

---

## 🔬 Future Work

- Validate AII with omega 3 fatty acids and key micronutrients  
- Extend the model to other food groups for a broader dietary tool  
- Add interactivity with Tableau or Plotly so users can filter by species and prep type  

---

## 📚 References

- World Health Organization, Endometriosis, 2023  
- The Endometriosis Foundation, Diet and Lifestyle  
- Cleveland Clinic, The Best and Worst Foods for an Anti-Inflammatory Endometriosis Diet  

---
