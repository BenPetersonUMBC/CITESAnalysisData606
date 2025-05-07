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


### Future Consideration

While I originally tried regression models through the informaton from these 2 datasets, it was unable to show much useful results, whether that be from not having enough correlation or user error in coding. Future considerations for this problem could be to bring in additional information that we know impact wildlife such as habitat destruction and pollution and see if bringing in more features from a variety of datasets can help to paint a more clear picture within regression modeling.
