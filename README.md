# Alzheimer's Disease Analysis

## BIS 687 Group 4: Baijia Xu, Jinxuan Bian, Huangrui Chu


# Background

Alzheimer's Disease (AD) stands as a formidable challenge in the landscape of global health, affecting an estimated 50 million people worldwide. Characterized by progressive neurodegeneration leading to cognitive decline, AD is the most common cause of dementia among older adults, casting a shadow over the golden years of an increasing segment of the population. Despite significant research efforts, the pathophysiology of AD remains complex and multifactorial, involving genetic, molecular, and environmental components that interplay over time. The Alzheimer’s Disease Neuroimaging Initiative (ADNI) has been instrumental in elucidating this complexity, providing an extensive database of clinical, cognitive, and biomarker information. However, the trajectory of AD progression varies greatly among individuals, and current predictive models often fail to capture the nuances of this variability. The incorporation of time-varying factors into these models is a burgeoning field of inquiry that promises to refine predictive accuracy. This background underscores the urgent need for innovative research approaches that can leverage such dynamic data to enhance our understanding and prediction of AD progression, ultimately leading to improved patient outcomes and more effective allocation of healthcare resources.

# Research Plan
The research plan for evaluating and improving the predictive power of clinical and cognitive measures on the progression of Alzheimer's Disease (AD) by incorporating a time-varying factor includes several steps: 1) Data Collection 2) Identification of Time-Varying Factors 3) Development of Predictive Model 4) Model Validation and Benchmarking 5) Analysis and Interpretation 6) Continual Improvement and Future Research. Details of each step are included as below.

# Research Strategy
## Specific Aim
To Evaluate and Improve the Predictive Power of Alzheimer's Disease Progression by Introducing One or More Additional Time-Varying Factors at Multiple Time Points

## Hypothesis
We hypothesize that incorporating the time-varying factors (such as Mini Mental State Exam (MMSE), Brain Volume, Regional Thickness etc.) at multiple time points into predictive models with time-constant genetics measures and demographics information will significantly improve the predictions of Alzheimer’s Disease (AD) progression, providing a more comprehensive assessment.

# Experimental Approach
Data Collection and Preparation: 

Utilize data from the Alzheimer's Disease Neuroimaging Initiative (ADNI), focusing on patients with detailed records of clinical and cognitive assessments, alongside longitudinally collected factor data.

Selection of Features:

Time-Varying Factors —- Identify key factors that vary over time and are likely to influence AD progression and that have been recorded at multiple time points. Begin with a literature review and meta-analyses to figure out which cognitive scores, biomarkers, and clinical assessments have shown significant correlations with disease progression. 

Time-Independent Factors —- Conduct feature selection using marginal screening and  Principal component analysis (PCA), identifying the most predictive variables from clinical scores, cognitive test outcomes, and time-varying factors such as medication use, lifestyle alterations, or biomarker levels. 

Statistical Modeling and Analysis: 

Employ landmark analysis to periodically select cohorts of patients who have reached certain points in the disease progression. Then, for each “landmark” time, we build random survival forests to predict survival probabilities based on the data, accounting for time-dependent nature of survival data and potentially more dynamic and accurate predictions over time.

Competing method: 

Cox proportional hazard models that treat time-varying covariates as time-constant variables would serve as a competing benchmark.

Model Validation: 

Use cross-validation techniques to assess the predictive performance of the model. Performance metrics, such as the concordance index (C-index) would be used to evaluate the model’s predictive capabilities. Sensitivity analyses would also be conducted to further explore the robustness of the model, helping to understand how changes in time-varying factors or assumptions about the disease progression impact the predictions and providing a deeper insight into the dynamics of AD progression and enhancing the model's applicability in clinical settings.
