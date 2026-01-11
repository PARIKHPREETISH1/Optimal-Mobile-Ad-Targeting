# Optimal Mobile Ad Targeting using Uplift Modeling

## Project Overview
This project focuses on identifying the most effective users to target with mobile advertisements using uplift modeling. Instead of predicting who is likely to convert, the analysis estimates the incremental impact of showing an ad versus not showing one. The goal is to optimize ad spend by targeting users whose behavior is positively influenced by marketing interventions.

The project is based on the TZ Gaming case and simulates a real world mobile marketing decision making scenario.

## Business Problem
Mobile advertising budgets are limited, and targeting all users can lead to wasted spend, user fatigue, or even negative impact. The key challenge is to identify:
• Users who convert only because they saw the ad  
• Users who would convert anyway without the ad  
• Users who are negatively affected by ads  

The business objective is to maximize incremental conversions while minimizing unnecessary ad exposure.

## Dataset
The dataset represents user level mobile gaming behavior and includes:
• Treatment indicator showing whether a user was exposed to an ad  
• Conversion outcome  
• User demographic and behavioral features  
• Large scale parquet based data for efficient processing  

Data Source: TZ Gaming Case Dataset  
Format: Parquet and exploratory notebook

## Methodology
The analysis follows a structured uplift modeling workflow:

1. Exploratory Data Analysis  
   Understanding treatment distribution, conversion rates, and feature behavior.

2. Baseline Modeling  
   Traditional classification models trained to predict conversion probability.

3. Uplift Modeling Approaches  
   • Two Model Approach  
   • Class Transformation Approach  
   • Comparison of uplift performance across segments  

4. Model Evaluation  
   • Uplift curves  
   • Qini coefficient  
   • Incremental lift analysis  

5. Targeting Strategy  
   Identifying persuadable users and excluding sure things and lost causes.

## Key Insights
• Targeting based on uplift significantly improves marketing efficiency compared to traditional conversion models  
• A large portion of users either convert regardless of ads or are negatively impacted  
• Selective targeting leads to higher incremental conversions with lower ad spend  

## Business Impact
• Improved return on ad spend by focusing on persuadable users  
• Reduced customer fatigue from unnecessary ads  
• Data driven targeting strategy aligned with causal impact rather than correlation  

## Tools and Technologies
• Python  
• Pandas and NumPy  
• Scikit learn  
• Uplift modeling techniques  
• Jupyter Notebook  

## Repository Structure
Optimal-Mobile-Ad-Targeting-main  
│  
├── data  
│   ├── tz_gaming.parquet  
│   └── tz-gaming.ipynb  
│  
├── tz-gaming.ipynb  
├── tz-gaming-case.pdf  
└── README.md  

## How to Run
1. Clone the repository  
2. Install required Python libraries  
3. Open tz-gaming.ipynb  
4. Run the notebook cells sequentially  

## Learning Outcomes
• Applied causal inference concepts to marketing analytics  
• Learned how uplift modeling differs from standard prediction models  
• Built targeting strategies based on incremental impact  
• Evaluated marketing effectiveness using uplift specific metrics  

## Author
Preetish Parikh  
Master’s in Business Analytics, UC San Diego  

## License
This project is for academic and educational purposes.
