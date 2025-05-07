# Assessing Future Overexploitation of Wild Life

DATA606 Capstone Proejct

### Goal

The goal of this project was to see what steps could be taken in the creation of predictive modeling to help with reducing overexploitation based on trading risk. This project focues on the top ten most traded species in the CITES dataset as well as a dataset from the World Bank Group detailing contries yearly GDP from the years 1975-2023.

### Research Questions

- Which species are most at risk of overexploitation based on trade behavior?
- How do economic factors like GDP correlate with trade risk?
- Can supervised learning models predict "at risk" species reliably?


### Datasets

I combined 2 different datasets for this predictive modeling. The first was the full CITES dataframe (https://trade.cites.org/) which includes over 26million rows and 21 different columns(too large to upload). The second dataset was from the World Bank Group, containing all available country GDPs' (https://data.worldbank.org/indicator/NY.GDP.MKTP.CD) from the years 1975-2023. These years were selected as they were the same years available in the CITES dataframe.

### Dataset issues
-The CITES dataset was very difficult to work with the 30,000+ taxon available on it, so for this project I limited the scope to just the top 10 traded taxon. This still left me with over 9million rows of trading data

-The Country GDP dataset required editing in order to successfully merge it with the CITES dataset, including adjusting the country codes and dropping the years where there was no GDP data available for the CITES dataset to track

-There was a large imbalance in the dataset, with the most "At risk" taxon only having 27% of their trading be "At Risk"

### Outcomes

I did not have much success with obtaining accurate models using logistic classification or random forest classifiers; however, the more advanced models such as Bagging Tree Classifier and MLP faired better in accurately identifying a species as "At Risk". 


### Requirements
- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib

### How to run
1. Clone repository
2. Download CITES dataset (877 MB available in attached google drive)
3. Open `DATA606Finalcopy.ipynb` in Jupyter Notebook
4. Run all cells
