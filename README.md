# Wine Quality Classification with Oversampling

This project performs wine quality prediction using Spark-based preprocessing and machine learning, with oversampling (e.g., SMOTE) applied to address class imbalance in red and white wine datasets.

## 1. Environment Setup

This project is designed to run in **Google Colab** and uses **PySpark** for distributed data processing.

### Steps:

1. Open Google Colab.
2. Upload the notebook file.
3. Ensure the required datasets (`winequality-red.csv`, `winequality-white.csv`) are available for upload during execution.

## 2. Dependencies

The following libraries are required and will be installed automatically in Colab:

```
pyspark
pandas
numpy
matplotlib
scikit-learn
imbalanced-learn
```

These may already be available depending on the Colab runtime.

## 3. Dataset

This project uses the **UCI Wine Quality Dataset**:

* `winequality-red.csv`
* `winequality-white.csv`

Both must be uploaded when prompted in the notebook.
Data is loaded manually using PySpark and labeled with a `wine_type` column.

## 4. Reproducing Results

1. Run all notebook cells in order.
2. When prompted, upload the two CSV files.
3. The notebook will clean, normalize, oversample, train models, and generate evaluation metrics.

## 5. Output Figures and Metrics

The notebook automatically outputs:

* Confusion matrices
* Classification reports
* Accuracy/F1 metrics
* Oversampling before/after class distributions
* Model comparison tables

## 6. Notes and Troubleshooting

* If PySpark fails to initialize, restart the Colab runtime.
* Ensure both CSV files are uploaded at the same prompt.
* Oversampling is applied separately for red and white wine datasets.
