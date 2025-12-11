#  Data 5100 Kelp



>  This notebook explores whether there is a relationship between kelp expression in the Puget Sound and water temperature from previous years. 



---



## Project Overview





**Objective:** There are many variables that can impact the growth and health of kelp. We are analyzing the impact of temperature and salinity on kelp growth.

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

\- Dryad Data - Mascarenas, Dakota; Leeson, Aurora; Horner-Devine, Alexander; MacCready, Parker (2025). Data from: Century-scale changes in temperature, salinity, and dissolved oxygen in Puget Sound \[Dataset]. Dryad. https://doi.org/10.5061/dryad.612jm64g7





 **Description:**

---

The question our team would like to answer is how do environmental parameters affect the area of N. luetkeana expression on the sea surface in the Salish Sea? Is there variation in their effects as a function of time? The North West Straights Commission collects data about kelp expression via volunteer kayak surveys throughout the summer as part of a program to monitor the health of the Salish Sea. The literature and general consensus in the field, is that water temperatures from previous years impact current kelp expression. We want to test what year lag is the most correlated to the expression of kelp in the current year. 



## Analysis



There is only one notebook titled " " in the code folder. Each cell should be run in the order presented. After data cleaning steps the notebook will output a cleaned csv to the data folder which can be used separately for other analysis. However, all of our analysis is in this notebook and continues directly after the data cleaning steps.



Once data is cleaned then we used a group correlation matrix and linear regression tests to determine which year lag best predicts bed area expression.





An overview of the analysis performed:

\- Data was cleaned following best practices. Missing data was imputed by substituting with the mean from previous years for the bed.

\- Cleaned datasets for every bed is output into individual csvs in \data\cleaned_data. There is also a csv titled "AllBeds_Clean", which is a combination of all the of the beds. ex: Ebey Landing, Polnell Point, North Beach etc each have their own csv with data from all years, which can be found in the data folder.

\- Initial exploration was conducted with a correlation matrix which reveals some relationships between the data.

\- Proceed with linear regression analysis on Acres. We chose to start multilinear regression and end with single input linear regression.



---



## Results



None at this time



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

