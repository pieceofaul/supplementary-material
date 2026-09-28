# Supplementary Material

**Comparative Analysis of Rule-Based and Machine Learning Approaches for Anthropometric Body
Shape Classification** — IEEE ITIS 2026, Paper #1571345367

This material is referenced in the camera-ready paper but omitted from the manuscript itself
due to the ITIS 2026 6-page maximum length.

## Contents
- `per_class_precision_recall_f1.csv` — complete per-class Precision, Recall, F1, and Support
  for all five classifiers (Random Forest, XGBoost, SVM, Logistic Regression, KNN) against the
  rule-derived labels on the held-out test set. The paper's Table V reports per-class F1 only;
  this file adds Precision, Recall, and per-class Support.
- `confusion_matrix_<Model>.csv` — the raw 7x7 confusion matrix (counts) for each classifier
  vs. rule-derived labels on the test set.
- `confusion_matrices_long.csv` — the same five confusion matrices in long format
  (Model, True, Predicted, Count), convenient for re-plotting.
- `confusion_matrices_all_models.png` — combined heatmap figure of all five confusion matrices.

## Note on ground truth
As explained in the paper (Section on label circularity), all reported metrics are **fidelity
to the rule-derived labels**, not classification correctness against an independent ground
truth. This applies to every file in this folder as well.
