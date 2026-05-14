# Module 5 Assignment: Will the Customer Accept the Coupon?

This is the project assignment for Module 5 of the **Post Graduate Program in AI and Machine Learning** from UC Berkeley. It uses the UCI ML coupon dataset to explore what factors influence whether a driver accepts a coupon delivered to their phone while driving.

## Data Cleaning

Missing values were identified using `df.isna().sum()`. The `car` column had the overwhelming majority of its values missing and was dropped entirely (only 12576 out of 12682 rows did not have value). 

For the remaining columns with few gaps (`Bar`, `CoffeeHouse`, `CarryAway`, `RestaurantLessThan20`, `Restaurant20To50`), missing values were filled with each column's mode — a safe choice given the categorical nature of the data.

## Key Findings

- **~57% of all coupons** were accepted overall.
- **Bar coupons (~41% acceptance):** Drivers who visit bars more than once a month, are over 25, travel without kids, and work outside farming/fishing/forestry accept bar coupons at significantly higher rates than others — suggesting that social lifestyle and context are strong predictors.
- **Coffee House coupons:** Drivers who already visit coffee houses regularly (>1/month) accept coffee house coupons at a notably higher rate than infrequent visitors, confirming that existing habits are important for acceptance. Also, from histogram plot it is evident that chances of Coffee House coupons being accepted are higher than any other category
