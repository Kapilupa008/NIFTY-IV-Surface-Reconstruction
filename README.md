# NIFTY Options IV Surface Reconstruction

## Author

Kapil Upadhyay (23112048)

## Project Overview

This project focuses on reconstructing missing implied volatility (IV) values in a partially observed NIFTY options volatility surface.

The objective is to estimate missing IV values while preserving:

- Surface smoothness
- Volatility skew
- Smile structure
- Local strike correlation
- Temporal consistency

The final predictions are evaluated using Mean Squared Error (MSE).

---

## Methodology

The proposed approach reconstructs the IV surface separately for Put (PE) and Call (CE) option families.

Key components:

1. Local strike-based interpolation
2. Adaptive convexity correction
3. Conditional temporal smoothing
4. Robust edge extrapolation
5. Separate PE and CE surface reconstruction

---

## Files

### code.ipynb

Main reconstruction notebook.

### dataset.csv

Original dataset containing missing IV values.

### filled_dataset.csv

Fully reconstructed IV surface.

### submission.csv

Final competition submission file.

### submission-converter.ipynb

Notebook used to generate the Kaggle submission format.

---

## Evaluation Metric

Mean Squared Error (MSE)

$$
MSE =
\frac{1}{N}
\sum_{i=1}^{N}
(\hat y_i-y_i)^2
$$

---

## Reproducibility

Run:

1. code2.ipynb
2. Generate filled_dataset.csv
3. Run submission converter
4. Generate submission.csv

The resulting submission.csv can be uploaded directly to Kaggle.