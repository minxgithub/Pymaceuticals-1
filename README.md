<img src="https://images.unsplash.com/photo-1542736667-069246bdbc6d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1351&q=80" height="80%" width="80%"> 

# Pymaceuticals
In cancer research, we are interested in looking at which drug treatments tested in mice are likely candidates to help fight against cancer spread and does not impact the survival rate of the mouse injected with the drug. 

For this case, we want to observe four potential candidates (Capomulin, Infubinol, Ketapril, and Placebo) to treat squamous cell carcinoma (SCC), a commonly occurring form of skin cancer. The purpose of this folder is to use matplotlib and pandas to help visualize our data so that we can make meaningful insights (Results Discussion below). 


## Prerequisites
- [Pandas](https://pandas.pydata.org/) (Python module)
- [Matplotlib](https://matplotlib.org/) (Python module) 
- [Jupyter Notebook](https://jupyter.org/) 

## Resources 
- Clincial and mouse data have been kindly provided by UC Berkeley's Data Analytics and Visualization 

## Demostration 
Load and open the Jupyter Notebook file in your computer.
```
git clone https://github.com/ying-li-python/Pymaceuticals.git
cd Pymaceuticals 
jupyter notebook 
```

## Results 
With the clincial and mouse data provided, we are interested in generating data to show: 
- how tumor volume changes over time for each treatment
- how the number of metastatic (cancer spreading) sites changes over 
time for each treatment
- number of mice still alive through the course of treatment (Survival Rate)
- the total % tumor volume change for each drug across the full 45 days

## Results Discussion 

#### Tumor volume and metastatic spread was significantly reduced when Capomulin was used to treat mouse with skin cancer 

##### Figure 1
<img src="https://raw.githubusercontent.com/ying-li-python/Pymaceuticals/master/Images/tumor_response.png">

Results from Figure 1 show that from 0-45 days of drug treatment, mice treated with Capomulin showed significant reduction in tumor volume as compared to that of mice treated with Infubinol, Ketapril, and Placebo. As expected, placebo-treated mice did not affect tumor growth. Mice treated with Infubinol and Ketapril displayed similar effects compared to that of the Placebo, suggesting that these drugs do not influence tumor volume. 

##### Figure 2 
<img src="https://raw.githubusercontent.com/ying-li-python/Pymaceuticals/master/Images/metastatic_spread.png"> 
Consistent from the results of Figure 1, mice treated with Capomulin for 45 days displayed a significant reduction in metastatic spread as compared to that of mice treated with Infubinol, Ketapril, and Placebo. As expected, placebo-treated mice did not influence metastatic spread; metastatic spread continued to grow steadily in placebo-treated mice. Similarily, Infubinol and Ketapril-treated mice displayed a similar pattern to that of Placebo, suggeting that these drugs are not as potent. 

Collectively, these data demonstrate that Capomulin is a strong candidate against the cancer growth and spread, whereas Infubinol and Ketapril have weak potency against cancer growth.

#### Mice treated with Capomulin have higher chances of survival 

##### Figure 3 
<img src="https://raw.githubusercontent.com/ying-li-python/Pymaceuticals/master/Images/survival_rates-1.png"> 

As shown in Figure 3, mice treated with Capomulin for 45 days have increased survival rates as compared to that of mice treated with Infubinol, Ketapril, and Placebo. As expected, placebo-treated mice showed a moderate decrease in survival across time; similarily, mice treated with Infubinol and Ketapril also had decreasing survival rates over time. 

From these data, it is likely that due to Capomulin treatment on reducing tumor growth, mice treated with Capomulin are living longer than their counterparts. As such, mice treated with Infubinol and Ketapril, which do not appear to influence tumor growth, do not improve survival. 

#### Mice treated with Capomulin display significant reduction in tumor volume for the entire treatment period 

##### Figure 4
<img src="https://github.com/ying-li-python/Pymaceuticals/blob/master/Images/tumor_volume.png"> 

According to the results from Figure 4, Capomulin-treated mice showed significant reduction in tumor growth between day 0 and 45, as compared to that of other drugs. As expected, Placebo-treated mice displayed increased tumor growth for the entire treatment period. Similarly, mice treated with Infubinol and Ketapril showed an overall increase in tumor growth for the 45 days of treatment. 

In summary, Capomulin is a promising drug candidate to help reduce tumor growth and metastatic spread, and as a result, improve survival rates for mice with SCC. 
