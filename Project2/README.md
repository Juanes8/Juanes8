# Creating a Multidimensional Financial Index using PCA

This project was devolped for my *Optimization* course, and I worked alongside my fellows and friends [Carlos López](https://github.com/kennyldc) and [Fernando Miñaur](https://github.com/Fminaurol). 

## Description

The global financial market represents one of the pillars in the world economy and its success or failure determines the course of entire countries. Quite simply, colossal crises such as the one caused between 2007 and 2008 began with the collapse of these sectors, dragging with them millions of citizens who directly participate in transactions or indirectly see their condition affected by the entire imbalances that it causes for the government and thousands of more companies.

Stock market indicators are used by investors, financial organizations, and analysts to monitor market trends. They can anticipate possible falls in the value of their shares or take advantage of a period of growth.

Given the importance of the stock indexes, for our project, we decided to use those of greater relevance in the most important financial market in the world, the US stock market. In particular, historical data for the last four years (from November 29, 2017, to November 29, 2021) was obtained from the following: 1) Dow Jones (DJ) Utility; 2) DJ Composite; 3) CBOE Volatility; 4) DJ Industrial Average; 5) NASDAQ 100; 6) NAQC; 7) NYSE Composite; 8) NYSE Market Composite; 9) Russell 200; 10) S&P 100; 11) S&P 500.

Each index reflects different information, is constructed a particular way, and is on a different scale. The problem seems to be linked to a dimensionality reduction method that manages to capture the existing trends in all the data sources. Following [Rassiga (2017)](https://repositorio.udesa.edu.ar/jspui/bitstream/10908/15785/1/%5BP%5D%5BW%5D%20T.%20L.%20Eco.%20Rassiga%2C%20Paula.pdf), the use of the Principal Component Analysis (PCA) method is a useful alternative for this type of stock information since it is timely adjusted to the creation of a multidimensional financial index that transforms a series of possibly correlated variables.

The methods used for the analysis were the power method and the deflation method. The power method is used to calculate the eigenvalue with maximum modulus with its respective eigenvector; by performing this method it is possible to obtain the first component. However, when performing a PCA analysis we require to obtain the rest of components. The power method with deflation is supported to obtain the rest of the components and determine which of them is capable of capturing the original variation of the data, thus reducing the dimensionality of our problem.

This project was developed in AWS using a Docker container, the configuration used can be found in the [AWS:Docker](https://github.com/Juanes8/Juanes8/tree/main/Project2/AWS:Docker) folder. The folder [Implementación](https://github.com/Juanes8/Juanes8/tree/main/Project2/Implementaci%C3%B3n) has the Python fuctiond that were used, you can find more details about this project in this [repository](https://github.com/Juanes8/proyecto_final_opt21_eq8).

## Libraries
- Numpy
- Matplotlib
- Pandas
- Math

