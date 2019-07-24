# happiness_project
Data Analysis and Visualization

Ryan Anthony Hess

Code Louisville Python/SQL Project for Summer 2019

World Happiness Analysis & Prediction

One of my goals for this project was to analyze happiness reports from 2015 to 2017 and, based on the changes in those sets of data, create visualizations to help me make general predictions for 2019.  I realize this is a difficult if not nearly impossible prediction to make given the limited data as well as its scope but I will try to make an educated guess based on my analysis. I’m curious to see the impact perceived freedoms have on the overall happiness score as well. I will be using a seaborn heatmap to determine the correlation and a seaborn point plot to attempt to visualize any trend in happiness.
As this class was my first introduction to Python, SQL, and data science in general, my main goal was to utilize what I’d learned in the treehouse videos and fulfill the project requirements.


Procedure:
1. Import all necessary packages
2. Create the database / database connections
3. Initial Analysis and Explanation of further exploration
4. Compare the top five countries and determine which were the happiest amongst the three years.
5. Determine the correlation between freedom and happiness
6. Using visualization techniques attempt to predict the top happiest countries in 2019
7. See if I am right


First Question:
According to the data, which five countries are the happiest in 2015, 2016. And 2017?

Second Question:
How freedom corelates to happiness in these three years?

Third Question:
Which countries are likely to be the happiest in 2019?


Reference : The data sets for this project are from Kaggle.com https://www.kaggle.com/unsdsn/world-happiness




Information from the Data Description on Kaggle.com:
Context
The World Happiness Report is a landmark survey of the state of global happiness. The first report was published in 2012, the second in 2013, the third in 2015, and the fourth in the 2016 Update. The World Happiness 2017, which ranks 155 countries by their happiness levels, was released at the United Nations at an event celebrating International Day of Happiness on March 20th. The report continues to gain global recognition as governments, organizations and civil society increasingly use happiness indicators to inform their policy-making decisions. Leading experts across fields – economics, psychology, survey analysis, national statistics, health, public policy and more – describe how measurements of well-being can be used effectively to assess the progress of nations. The reports review the state of happiness in the world today and show how the new science of happiness explains personal and national variations in happiness.
Content
The happiness scores and rankings use data from the Gallup World Poll. The scores are based on answers to the main life evaluation question asked in the poll. This question, known as the Cantril ladder, asks respondents to think of a ladder with the best possible life for them being a 10 and the worst possible life being a 0 and to rate their own current lives on that scale. The scores are from nationally representative samples for the years 2013-2016 and use the Gallup weights to make the estimates representative. The columns following the happiness score estimate the extent to which each of six factors – economic production, social support, life expectancy, freedom, absence of corruption, and generosity – contribute to making life evaluations higher in each country than they are in Dystopia, a hypothetical country that has values equal to the world’s lowest national averages for each of the six factors. They have no impact on the total score reported for each country, but they do explain why some countries rank higher than others.
Inspiration
What countries or regions rank the highest in overall happiness and each of the six factors contributing to happiness? How did country ranks or scores change between the 2015 and 2016 as well as the 2016 and 2017 reports? Did any country experience a significant increase or decrease in happiness?
What is Dystopia?
Dystopia is an imaginary country that has the world’s least-happy people. The purpose in establishing Dystopia is to have a benchmark against which all countries can be favorably compared (no country performs more poorly than Dystopia) in terms of each of the six key variables, thus allowing each sub-bar to be of positive width. The lowest scores observed for the six key variables, therefore, characterize Dystopia. Since life would be very unpleasant in a country with the world’s lowest incomes, lowest life expectancy, lowest generosity, most corruption, least freedom and least social support, it is referred to as “Dystopia,” in contrast to Utopia.
What are the residuals?
The residuals, or unexplained components, differ for each country, reflecting the extent to which the six variables either over- or under-explain average 2014-2016 life evaluations. These residuals have an average value of approximately zero over the whole set of countries. Figure 2.2 shows the average residual for each country when the equation in Table 2.1 is applied to average 2014- 2016 data for the six variables in that country. We combine these residuals with the estimate for life evaluations in Dystopia so that the combined bar will always have positive values. As can be seen in Figure 2.2, although some life evaluation residuals are quite large, occasionally exceeding one point on the scale from 0 to 10, they are always much smaller than the calculated value in Dystopia, where the average life is rated at 1.85 on the 0 to 10 scale.
What do the columns succeeding the Happiness Score(like Family, Generosity, etc.) describe?
The following columns: GDP per Capita, Family, Life Expectancy, Freedom, Generosity, Trust Government Corruption describe the extent to which these factors contribute in evaluating the happiness in each country. The Dystopia Residual metric actually is the Dystopia Happiness Score(1.85) + the Residual value or the unexplained value for each country as stated in the previous answer.
If you add all these factors up, you get the happiness score so it might be un-reliable to model them to predict Happiness Scores.
