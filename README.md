### A Particulate Problem: Predicting Mortality from Diseases Related to Air Pollution and Revealing Significance of Air Pollution

This project looks at predicting mortality rates for two specific diseases related to air pollution:

Chronic Obstructive Pulmonary Disease
Ischaemic Heart Disease

It also extracts the significace of air pollution alone as a contrbuting factor in disease rates. The following notebooks are instrumental in the analysis:

CDC_COPD.ipynb, CDC_HID.ipynb:
These notebooks predict the death counts for each disease using the Poisson GLM, linear regression and Random Forest regression. Features were engineered to provide an eight year average. While both the Poisson regression and the Random Forest model performed well, air pollution did not prove to be a significant factor in determining death counts.

CDC_COPD-Propensity.ipynb, CDC_IHD-Propensity.ipynb
Since the predictive tools could not isolate the effect of air pollution, we switch to a propensity matching technique in order to isolate the effect of air pollution. We split counties into 'high' pollution and 'low' pullution groups and compare mean difference in deaths between pairs from each group (one from each). Pairs were selected according to similarities in their propensity scores. Air pollution showed up as significant for COPD, but not for IHD.

Regular_Time_Series/CDC_COPD-Redone.ipynb,Regular_Time_Series/CDC_COPD-Redone.ipynb
We carry out predictive modeling using a regular time series as opposed to a moving eight year average.

![Follow my process here](https://github.com/jitsen-design/Air_Pollution_and_Disease/blob/master/A_Particulate_Problem_Jit_Seneviratne.pdf)





