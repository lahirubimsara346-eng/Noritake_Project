# Warpage Reduction in Porcelain Production using Beta Regression

## Overview
This project focuses on analyzing and minimizing the warpage percentage of porcelain cups in an industrial manufacturing process. Since the response variable is a continuous proportion (bounded between 0 and 1), a **beta regression model** with a logit link function was used.

The study identifies key process variables affecting product quality and provides data-driven recommendations to reduce defects.

---

## Objectives
- Model the relationship between process variables and warpage percentage  
- Identify significant factors influencing warpage  
- Validate model assumptions using diagnostic techniques  
- Provide recommendations to optimize production conditions  

---

## Data Description
The dataset consists of production process variables collected from a porcelain manufacturing environment.

**Variables used:**
- Hardness  
- Clay moisture  
- Drying temperature 1  
- First unloading moisture  
- Drying temperature 2  
- Warpage percentage (response variable)  

---

## Methodology
- Selected **beta regression** due to the proportional nature of the response variable  
- Used **logit link function** to relate predictors to the mean response  
- Compared alternative models (Poisson, Negative Binomial, Linear, Logistic) before final selection  
- Model form:
  
  μᵢ = g⁻¹(Xᵢβ), where g(.) is the logit link function  

---

## Model Diagnostics
To ensure model validity, the following diagnostic checks were performed:
- Residuals vs fitted values  
- Residuals vs linear predictor  
- Cook’s distance (influence diagnostics)  
- Generalized leverage  
- Half-normal plot  

Results indicated:
- No significant patterns in residuals  
- Limited influential observations  
- Good overall model fit  

---

## Key Findings
- Clay hardness, moisture levels, and drying temperatures significantly influence warpage  
- The beta regression model provided accurate predictions with minimal bias  
- Process imbalance between moisture and temperature is a major contributor to defects  

---

## Recommendations
- Maintain clay hardness below 80  
- Keep first unloading moisture above 20%  
- Keep second unloading moisture above 10%  
- Optimize drying conditions (moisture 25–30%, temperature < 50°C)  

---

## Tools & Technologies
- R (Beta regression modeling)
- Statistical analysis and visualization  

---

## Repository Structure
