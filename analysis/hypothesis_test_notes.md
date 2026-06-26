# Experiment Hypothesis Testing Notes


## 1. Hypothesis Formulation
We test the onboarding campaign's performance using the primary success metric: **Paid Conversion Rate (p)**.

* **Null Hypothesis (H_0):** p{{Treatment}} <= p{{Control}}

    *The new onboarding campaign has no positive effect on the paid conversion rate; the conversion rate of the Treatment group is less than or equal to the Control group.*
* **Alternative Hypothesis (H_1):** p{{Treatment}} > p{{Control}} 

    *The new onboarding campaign systematically improves the user conversion rate compared to the old onboarding layout.*


## 2. Test Configuration
* **Test Type:** One-Tailed Two-Sample Proportions t-Test Assuming Unequal Variances (Directional change tracking for conversion improvements).
* **Significance Level (alpha):** 0.05 (Standard 95% Confidence Threshold).
* **Primary Metric: Paid Conversion Rate:** This metrics check whether this new campaign has a positive impact on the Business and to drive early conversion and product value.


## 3. Statistical Calculations & Inputs
* **Control Sample Size (n_1):** 669
* **Control Conversions (x_1):** 20
* **Control Proportion mean(p_1):** 0.029895 (2.99%)
* **Treatment Sample Size (n_2):** 675
* **Treatment Conversions (x_2):** 48
* **Treatment Proportion mean(p_2):** 0.071111 (7.11%)
* **Pooled Standard Error (SE):** 0.055274
* **Calculated t-Statistic:** -3.4658


## 4. Test Output & Evidence
* **Calculated t-Score:** `-3.4658`
* **Critical t-Value (One-tailed, alpha = 0.05):** `1.6461`
* **P-Value:** `0.00027`


## 5. Decision Rule & Business Interpretation
* **Rule:** If p-value < 0.05, we reject the Null Hypothesis (H_0).
* **Outcome:** The p-value `0.00027` is far below our alpha threshold of `0.05`.
* **Business Verdict:** We officially **reject the Null Hypothesis**. The observed 137.9% relative increase in the paid conversion rate is due to the new onboarding experience and cannot be explained by random sampling noise. The onboarding campaign delivers authentic business value.