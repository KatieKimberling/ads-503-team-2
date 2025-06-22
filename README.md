# **The Root of All Ills:**

# **Predicting Metabolic Syndrome with Machine Learning**

## A machine learning project for developing algorithms to (eventually) predict Metabolic Syndrome with noninvasive predictors.

## USD MADS 503: Applied Predictive Modeling

### Summer 2025, Professor Ebrahim Tarshizi

#### Authors:

-   [Paola Rodriguez](https://www.linkedin.com/in/paola-rodriguez920623/)
-   [Gabriel "Gabe" Duffy](https://www.linkedin.com/in/gabriel-duffy/)
-   [Katherine "Katie" Kimberling](https://www.linkedin.com/in/katie-kimberling-b6617173/)

### **Abstract**

Metabolic syndrome (MetS) is a complex constellation of health metrics that collectively negatively impact the health and well being of individuals, significantly increasing the risk of cardiovascular disease, stroke, and development of type 2 diabetes.
This set of negative health markers that acts as a precursor to at least four of the top ten causes of death in the United States.
MetS leads to premature death, decrease in quality of life, and exponentially growing costs from health care and loss of earning potential.
More than a third of US adults have MetS, and the numbers are rising.

MetS is also almost completely preventable.

### **Objective**

The goal of this research is first to use data from both bloodwork and non-invasive metrics to predict MetS.
Successful model development with available (blood draw) data will pave the way for prediction of MetS through the use of alternative predictors that do not require invasive testing.
The less invasive a diagnostic test the more likely patients are to participate, leading to earlier diagnosis and more opportunities for prevention and cure.

The hope is that such predictive modeling can be used in a noninvasive, clinical setting to diagnose MetS early, so that through education and lifestyle change this global epidemic can be stopped.

### Getting Started

To run this project please take the following steps:

1\.
Run the git init code chunk in your terminal

```         
git init
```

2.  Clone the project repo:

```         
git clone https://github.com/KatieKimberling/ads-503-team-2.git
```

3.  Navigate to the Project Deliverables folder, then
   
4.  Run the project notebook:

```         
Metabolic Syndrome Final Project.ipynb
```

### Are YOU At Risk?

To determine your personal risk of metabolic syndrome, click the link below and enter your health metrics.
Your body mass index (BMI) is calculated as your weight (in kg) divided by your height (in meters) squared.
If you do not know your BMI, you can calculate it here: [BMI Calculator](https://www.nhlbi.nih.gov/calculate-your-bmi)

[Predict your risk of Metabolic Syndrome](https://paolarodriguez.shinyapps.io/metabolic-syndrome-predictor-v2/)

### **Modeling**

Five machine learning models were constructed, trained, and evaluated on an 80/20 split of data from [Kaggle](https://www.kaggle.com/datasets/antimoni/metabolic-syndrome?resource=download) (Antony, 2023).
Out of fourteen original predictor values, six were retained for modeling:

-   Triglycerides (log transformed)
-   Blood glucose (log transformed)
-   HDL (high density lipoprotein, or "good" cholesterol)
-   BMI
-   Waist circumference (cm)
-   Age (years)

The response variable was a binary classification indicating presence or absence of metabolic syndrome.

Models trained and tested were Logistic Regression (LR), Random Forest (RF), Support Vector Machine (SVM), k-Nearest Neighbors (k-NN), and Gradient Boosting (GBM).

Of the five models, GBM performed the best across the board in terms of accuracy, area under the receiver operating curve, and accurately detecting true positive and avoiding false negatives.

*Summary of performance metrics across all models*

|  |  |  |  |  |  |
|------------|------------|------------|------------|------------|------------|
| **Model** | **Accuracy** | **AUROC** | **Sensitivity** | **Specificity** | **Kappa** |
| Logistic Regression | 0.831 | 0.9056 | 0.76 | 0.87 | 0.63 |
| Random Forest | 0.857 | 0.9428 | 0.82 | 0.87 | 0.69 |
| SVM (RBF Kernel) | 0.854 | 0.9191 | 0.8 | 0.88 | 0.68 |
| k-NN (k = 15) | 0.829 | 0.9029 | 0.74 | 0.88 | 0.62 |
| GBM | **0.877** | **0.95** | **0.84** | **0.90** | **0.72** |

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

-   Professors Ebrahim Tarshizi, An Tran and Isabella Oakes of the University of San Diego – instrumental in helping us understand machine learning principles and urging us to excellence.
-   Team 2 for their commitment to communication, teamwork, and excellent work.

### References

-   Antony, A.
    (2023).
    Metabolic Syndrome: A Comprehensive Dataset on Risk Factors and Health Indicators.
    [Dataset].
    Retrieved from <https://www.kaggle.com/datasets/antimoni/metabolic-syndrome?resource=download>.

-   Center for Disease Control/National Center for Health Statistics.
    (2025).
    Deaths and mortality.
    <https://www.cdc.gov/nchs/fastats/deaths.htm>

-   Kuhn, M.
    & Johnson, K.
    (2013).
    Applied predictive modeling.
    New York: Springer.

-   Li, W., Qiu, X., Ma, H., & Geng, Q.
    (2023).
    Incidence and long-term specific mortality trends of metabolic syndrome in the United States.
    Frontiers in Endocrinology (13).
    <https://doi.org/10.3389/fendo.2022.1029736>

-   Neeland, I.J., Lim, S., Tchernof, A., Gastaldelli, A., Rangaswami, J., Ndumele, C.E., Powell-Wiley, T.M., & Despres, J-P.
    (2024).
    Metabolic syndrome.
    Nature Reviews Disease Primers 10(77).
    <https://doi-org.sandiego.idm.oclc.org/10.1038/s41572-024-00563-5>

-   OpenAI.
    (2025).
    ChatGPT (June 18 version).
    [LLM].[https://chatgpt.com](https://chatgpt.com/)

-   OpenAI.
    (2025).
    ChatGPT (June 21 version).
    [LLM].[https://chatgpt.com](https://chatgpt.com/)

-   Saklayen, M.G.
    (2018).
    The global epidemic of the metabolic syndrome.
    Current Hypertension Reports (20)12, 1-8. 
    <https://doi.org/10.1007/s11906-018-0812-z>

-   Shin, H., Shim, S., & Oh, S.
    (2023).
    Machine learning-based predictive model for prevention of metabolic syndrome.
    Public Library of Science ONE (18)6.
    <https://doi.org/10.1371/journal.pone.0286635>

-   [Xu, W](https://www.dovepress.com/author_profile.php?id=1751875)., [Zhang, Z](https://www.dovepress.com/author_profile.php?id=1689111)., [Hu, K](https://www.dovepress.com/author_profile.php?id=1884150)., [Fang, P](https://www.dovepress.com/author_profile.php?id=1634270)., [Li, R](https://www.dovepress.com/author_profile.php?id=1571149)., [Kong, D](https://www.dovepress.com/author_profile.php?id=1751874)., [Xuan, M](https://www.dovepress.com/author_profile.php?id=1173176)., [Yue, Y](https://www.dovepress.com/author_profile.php?id=1884151)., [She, D](https://www.dovepress.com/author_profile.php?id=1634275)., & [Xue, Y](https://www.dovepress.com/author_profile.php?id=1634276). 
    (2023. Identifying metabolic syndrome easily and cost effectively using non-invasive methods with machine learning models. Diabetes, Metabolic Syndrome and Obesity (2023)16, 2141–2151.
    <https://doi.org/10.2147/DMSO.S413829>
