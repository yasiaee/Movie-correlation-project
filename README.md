# Movie-correlation-project
This is the dataset from kaggle and available at this https://www.kaggle.com/datasets/danielgrijalvas/movies link.
The dataset shows 6820 movie revenue and other parameters like budget, company, etc.
In this project our aim is to find the features which have the most correlation with the gross income of the movie.
This project has three steps:
1. Data cleaning
2. Finding correlation
3. Analyzing results


1. Data cleaning:
Data cleaning is one of the most important parts of any dataset analysis. The null value is one of the most important factors which can affect our final result. using df[col].isnull() module to find the null value. There are multiple ways to tackle null values, however in this project I simply removed null values.  Then use df.dropna() to eliminate the null values. Also changing the types of data from float to int and also adding the released year to the new column and calling it yearcorrect are the other steps in this part.

2. Finding correlation:
There are three methods that can be used for finding data correlation in Python. pearson, kendall and spearman. The Pearson method is used in this project for finding the correlation. Also cat.codes is used to numerized the non numeric features like genre.

3. Analyzing results:
using corr_pairs.sort_values() to find the most correlated features to gross income which are budget and votes respectively. 
