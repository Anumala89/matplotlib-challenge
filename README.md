# matplotlib-challenge
Compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens.


### Purpose

The focus of the assignment was to generate tables and figures showcasing the effects of Campomulin, a drug that gave promising results in comparision to other drug regimens, on tumor development in mice over the course of 45 days and also to provide a summary of the study results.


### Pre-Analaysis

Before beginning the anaylsis, the first step is to check the data for any duplicate values and to remove it. Here, Mouse ID g989 had double time points and so it was removed. Then a summary statistics consisting of the mean, median, variance, standard deviation, and SEM of tumor volume for each treatment regimen was generated to get an outline of their effects on the tumor. 


### Analysis

Bar plot and pie plot were created using both Pandas's `Dataframe.plot()` and Matplotlib's `pyplot` to showcase the number of total mice for each treatment regimens. A scatter plot of mouse weight versus average tumor volume for the Capomulin treatment was also generated along with calculation of the correlation coefficient and linear regression model. 


### Observations and Insights
The least favorable drug to lower the tumor volume seems to be Ketapril with average tumor volume higher than any other drug. Compared to Ramicane, the average tumor was high by almost 6% over the period of 45 days but remarkably close to average tumor volume of mice on Placebo. Looking at the bar graph, the number of mice on Capomulin and Ramicane were larger than any other drugs, making these drugs potential candidates to lower the growth of tumor and the survival of mice.

![bar graph](https://github.com/Anumala89/matplotlib-challenge/blob/master/graphs/mice_per_drug_barpylot.png)

The median tumor volume for mice on Infubinol is approx. 60 mm3 and the halves of the box indicate a normal distribution of data. This tells us that most of the mice on Infubinol have larger tumor volume compared to the ones on another drug regimen. Like Infubinol, the lack of skewness of the box of Ramicane indicates normal distribution but unlike Infubinol the tumor volumes are on smaller range and with a median of approx. 37 mm3. Thus, Ramicane looks like a promising drug to reduce tumor at the end of 45 days period.

![box plot](https://github.com/Anumala89/matplotlib-challenge/blob/master/graphs/tumor_vol_for_four_regimens.png)

There is a high correlation between the weight and average tumor volume of mice on Capomulin. Judging by the linear equation, as the number of weights increased so did the tumor volume. On average, the tumor of mice on Capomulin is less than the tumor of mice on any other drug regimen proving that there is a link between the body weight and the progression in tumor regardless of treatments

[linear regression](https://github.com/Anumala89/matplotlib-challenge/blob/master/graphs/liner_regression.png)
