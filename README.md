# Data Scaling vs Accuracy

## Overview

This project explores a simple but widely accepted assumption in machine learning: **does adding more data always lead to meaningfully better models?**

Rather than treating scale as a default solution, this study examines how model performance actually changes as dataset size increases, and where diminishing returns begin to appear. The aim is to look at data quantity with the same critical eye we apply to algorithms and evaluation methods.

## Motivation

The current narrative in AI often suggests that progress depends on ever-larger datasets and infrastructure. This project asks a smaller, practical question:

> *At what point does “more data” stop being the most effective way to improve a model?*

Understanding this could help shift focus toward better methodology, evaluation, and efficiency instead of brute-force scaling.

## What This Project Does

* Trains multiple machine learning models on progressively larger subsets of data
* Generates learning curves to track performance vs dataset size
* Compares simple and complex models to see who benefits most from additional data
* Measures variance and stability, not just raw accuracy
* Looks for points where gains begin to plateau

## Approach

1. Select datasets suitable for controlled subsampling
2. Apply consistent preprocessing to avoid leakage
3. Train several model types across increasing data sizes
4. Evaluate using robust cross-validation
5. Analyse marginal improvements and computational cost

## Key Questions

* Do all models continue to improve with more data?
* How early do diminishing returns appear?
* Are some models more data-hungry than others?
* When might better evaluation matter more than more data?

## Structure

```
├── data/               # datasets or instructions to obtain them  
├── notebooks/          # experiments and learning curve analysis  
├── src/                # reusable code for training & evaluation  
├── results/            # figures and tables  
└── README.md
```

## Tools

* Python
* scikit-learn
* standard data science libraries

## Notes

This is an exploratory, methodology-focused project rather than an attempt to build the “best” model. The goal is to question assumptions about scale and understand what the data actually shows.

---

*Technology works best when we ask not just what is possible, but what is necessary.*
