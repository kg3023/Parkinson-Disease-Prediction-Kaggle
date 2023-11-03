# Parkinson-Disease-Prediction-Kaggle

Parkinson’s disease is a brain disorder that causes unintended or uncontrollable movements,
such as shaking, stiffness, and difficulty with balance and coordination. Unfortunately, there is
no current cure and the disease worsens over time. Currently, Parkinson’s disease affects 1-2%
of individuals over the age of 65 and its prevalence is increasing rapidly as the population ages.
Studies have shown protein or peptide abnormalities play an important role in the onset and
exacerbation of the disease, and the MDS-UPDRS (Movement Disorder Society-Sponsored
Revision of the Unified Parkinson's Disease Rating Scale) is a comprehensive assessment of
both motor and non-motor symptoms associated with Parkinson's disease. The goal of this
project is to predict MDS-UPDRS scores, which represents the progression of Parkinson’s
disease in patients. More specifically, the goal is to predict a patient’s MDR-UPDR score in the
current visit for each of the 4 classes of symptoms as defined by the MDS-UPDRS.
DATASET
For our dataset, we will be using the Kaggle dataset from the AMP Parkinson Disease
Progression Prediction competition. The total dataset contains data from samples gathered over
several years for several hundred patients. For each patient’s visit, the dataset includes:
- Protein abundance values from Mass spectrometry data
- Protein expression frequencies aggregated from the peptide level data
- Patient MDR-UPDR scores
- Clinical records without any associated CSF samples
https://www.kaggle.com/competitions/amp-parkinsons-disease-progression-prediction/data
ML TECHNIQUES TO BE USED
Given this problem requires us to predict multiple numerical scores, we will need to develop a
multi-output regression model. As a result, we will begin by investigating several traditional
regression models, such as: linear regression, Random Forest, LGB, and XGBoot. We will also
investigate the usage of time series models, such as ARMA and ARIMA. Eventually, we will
progress towards investigating deep learning models such as neural networks.
For the data analysis, we will need to investigate time-series feature analysis techniques, since
the patient scores are provided over a series of months. Additionally, given that there are often
multiple peptides per protein, we will need to analyze the best way to map these features
between these two datasets. For the final prediction, we will try to combine traditional regression
models, time series models, and deep learning models to determine the best overall estimator.
