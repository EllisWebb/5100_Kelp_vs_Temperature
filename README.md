# Analyzing the Effects of Temperature on Kelp Health and Expression



>  This notebook explores whether there is a relationship between kelp expression in the Puget Sound and water temperature from previous years. 



---



## Project Overview





**Objective:** There are many variables that can impact the growth and health of kelp. We are analyzing the impact of temperature on kelp growth.

**Domain:**  Ecology

**Key Techniques:**   Correlation Matrix, Pairplots, Linear Regression



---



## Project Structure



```

├── data/                 # Raw and processed data
	├── cleaned\_data/  # Cleaned data for every bed and one "AllBeds" csv


├── code/                 # Jupyter notebooks and Python scripts


├── research/              # Generated reports and visualizations

├── requirements.txt      # Dependencies

└── README.md             # Project documentation

```



---



## Data



**Source:** 

\- NWS-MRC Data - Community Science Monitoring Efforts Performed by the Marine Resource Committees (MRCs) and Northwest Straits Commission (NWSC) 2016 - 2024


 **Description:**

---

Here we focus on the effect of environmental parameters on the area of N. luetkeana expression on the sea surface in the Salish Sea. Further asking, is there variation in their effects as a function of time? The North West Straights Commission collects data about kelp expression via volunteer kayak surveys throughout the summer as part of a program to monitor the health of the Salish Sea. The literature and general consensus in the field, is that water temperatures from previous years may impact current kelp expression. We want to test what year lag is the most correlated to the expression of kelp in the current year. 



## Analysis



There is only one notebook titled "Cleaning.ipynb" in the code folder. Each cell should be run in the order presented. After data cleaning steps the notebook will output a cleaned csv to the data folder which can be used separately for other analysis. However, all of our analysis is in this notebook and continues directly after the data cleaning steps.



Once data is cleaned then we used a group correlation matrix and linear regression tests to determine which year lag best predicts bed area expression.





An overview of the analysis performed:

\- Data was cleaned following best practices. Missing data was imputed by substituting with the mean from previous years for the bed.

\- Cleaned datasets for every bed is output into individual csvs in \data\cleaned_data. There is also a csv titled "AllBeds_Clean", which is a combination of all the of the beds. ex: Ebey Landing, Polnell Point, North Beach etc each have their own csv with data from all years, which can be found in the data folder.

\- Initial exploration was conducted with a correlation matrix which reveals some relationships between the data.

\- Proceed with linear regression analysis on Acres. We chose to start multilinear regression and end with single input linear regression.



---



## Results
This study analyzed nearly a decade (2015–2024) of bull kelp monitoring data across 17 sites in the Salish Sea to investigate the relationship between temperature and annual kelp bed area.

Across all sites, temperature alone was not a strong predictor of kelp bed area change. Correlation analysis showed weak overall relationships, with the strongest signal emerging from temperature conditions two years prior correlated with percent acre change of all beds. While this correlation was notoriously weak, it warranted further exploration of potential lagged environmental effects.

Multiple linear regression models for all sites identified particularly lagged temperature variables as nearly statistically significant in a few cases (p ≈ 0.044), but with low explanatory power (R² ≈ 0.064). This indicated that temperature explains only a small portion of variability in kelp dynamics, or that signals of temperature influence are lost at this scale of analysis.

In contrast to global granularity, we further explored site-level analyses, revealing stronger relationships. 

These included:
	•	Positive and negative relationships between lagged temperature and kelp area, with significance and lag varying by site.
	•	Differences between relationships at nearby sites, even within the same basin
	•	A boost in explanatory power in select cases under these hyper-localized models

These findings highlight that kelp response to temperature is highly spatially dependent, and that local environmental conditions and site-specific dynamics may outweigh larger, more abstract trends.

Overall, results suggest that while temperature plays a role in kelp dynamics, it may be interacting with additional environmental factors, for example nutrients, light, and salinity, to create site-specific trends, with further evidence for temperature’s influence through multi-year lag effects rather than immediate responses.



---



## Authors

\- Carter Ellis- \[@EllisWebb](github.com/EllisWebb)

\- Sydney Golden- \[@sgolden3](github.com/sgolden3)

\- Ahrial Young - \[@ayoung42](https://github.com/ayoung42)



---



## License



This project is licensed under the MIT License - see the \[LICENSE](LICENSE) file for details.





---



## Acknowledgements
Dr. Brian Fischer for his 5100 class in which he taught us many of these tools.



\-

