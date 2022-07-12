# Credit-Risk-Assesment-Part-2
An updated version of the Credit Risk Assesment Project adding in two custom variables, [refined dashboard](https://public.tableau.com/app/profile/samantha.britschgi6603/viz/CreditRiskData-ClassificationDashboardStory/Story1?publish=yes), applying the model to null customer data, and more in depth insights.

# Credit-Risk-Assesment-Part-1
A one day project to classify credit risk and visualize findings in a single dashboard for "Decision Making with Business Intelligence and Analytics" as part of the MS Data Analytics program at Seattle Pacific University.  

### Background
[Data](https://github.com/Samantha-Britschgi/Credit-Risk-Assesment/blob/6277e8a533ec386605f2f522e111d75cca3db005/Credit%20Risk%20Data.xlsx) was provided in a single XLSX format, containing a total of 437 rows and 12 columns.
An additional ID column was added to the trraining data for ease of use in Rapid Miner.

* ***The goals:*** 
- There is a desire to classify if a borrower will be at high risk or low risk of repaying lenders money.
- Analyze whom is at higher or lower risk of repaying debt. 
- Determine where credit risk classification model can be improved.

### instructions

The Rapid Miner [process](https://github.com/Samantha-Britschgi/Credit-Risk-Assesment/blob/6277e8a533ec386605f2f522e111d75cca3db005/CreditRiskModel.rmp) can be imported into Rapid Miner for ease of use.
 
### Process

    1. Inputed XLSX data
    2. Set Role of Credit Risk as label
    3. Applied a weighted relative sample bootstraping with a ratio of 2.0
    4. Applied stratified sampling Cross Validation with 13 folds
    5. Random forest model was deployed with 500 trees, maximal depth of 10, and criterion set to gini_index
    6. Model was applied with split data 
    7. Determined classification performance 
    8. Additional sheet in data file with null credit risk had the model applied

### Overall Rapid Miner Process

<img src="https://github.com/Samantha-Britschgi/Credit-Risk-Assesment/blob/959dc899f219c86c08f52b99bf0a069afc6818e1/Credit-Risk-Assesment-RapidMiner-Images/Model%20Process.png" width="500" height="200" />

<img src="https://github.com/Samantha-Britschgi/Credit-Risk-Assesment/blob/959dc899f219c86c08f52b99bf0a069afc6818e1/Credit-Risk-Assesment-RapidMiner-Images/ModelApplication.png" width="1400" height="200" />

    
### Findings
The model performed with an accuracy of 93.76% with percision and recall between 93-94%.

<img src="https://github.com/Samantha-Britschgi/Credit-Risk-Assesment/blob/959dc899f219c86c08f52b99bf0a069afc6818e1/Credit-Risk-Assesment-RapidMiner-Images/Confuson%20Matrix.png" width="900" height="200" />
