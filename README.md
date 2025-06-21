# Hypertensive Retinopathy Risk Calculator

This web-based calculator predicts the probability of hypertensive retinopathy (HR) using logistic regression based on clinical variables. The model is derived from the Korean National Health and Nutrition Examination Survey (KNHANES) dataset (2008-2011).

## Features
1. **Input Variables:**
    Age (years)
    Systolic Blood Pressure (HE_sbp, mmHg)
    HbA1c (HE_HbA1c, %)
    Total Cholesterol (HE_chol, mg/dL)
    Creatinine (HE_crea, mg/dL)
    Hemoglobin (HE_HB, g/dL)

2. **Risk Assessment:**
   - Calculates the probability of hypertensive retinopathy using the logistic regression equation.
   - Risk categories are based on calibrated thresholds:
    High Risk: Probability > 0.0648 (top 1%)
    Moderate Risk: 0.0229 < Probability ≤ 0.0648 (top 10%)
    Low Risk: Probability ≤ 0.0229
   - Risk levels are color-coded for clarity:
    🟥 Red: High risk
    🟨 Yellow: Moderate risk
    🟩 Green: Low risk

## Dataset
The model is based on the KNHANES 2008-2011 dataset, which is a nationwide, cross-sectional survey conducted by the Korea Disease Control and Prevention Agency (KDCA). This dataset includes comprehensive health information, such as:
   - Demographic details (age, sex, etc.)
   - Medical history
   - Laboratory test results
   - Ophthalmological examinations, including detailed retinal evaluations.

### Why KNHANES?
KNHANES is a high-quality, representative dataset of the Korean population. It provides extensive health data, ensuring accurate risk prediction for hypertensive retinopathy.

## How to Use the Calculator
1. Open the HTML file in any modern web browser.
2. Enter the required clinical values (e.g., systolic blood pressure, fasting glucose, etc.).
3. Click the **"Calculate Risk"** button.
4. View the predicted probability and the risk classification.

## Limitations
- This calculator is specifically developed for non-diabetic patients, as the dataset excludes diabetic participants to avoid confounding effects from diabetic retinopathy.
- The model is designed based on the Korean population and may need validation before application in other populations.

## Acknowledgments
This calculator is based on data and insights from the KNHANES (2008-2011) survey. We thank the KDCA and the Korean Ophthalmologic Society for their contributions to data quality and analysis.

## Contact
For questions or further information, please contact [eyetaekeunyoo at gmail.com].

