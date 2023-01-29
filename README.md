## Table of contents
1. Data Science
    1. [Data Science Salaries project](#project1)
    2. [Text Data Mining](#project2)
2. Programming
    1. [Android App](#project3)

## Project 1: Multivariate Analysis of Data Science Salaries <a name="project1"></a>
This project was completed in R and the report was produced using R Markdown.

### Project overview
The data set contains several hundred Data Science-related job listings in the United States scraped from the website Glassdoor. The purpose of this research was to determine which of a particular subset of explanatory variables had an effect on the Lower, Upper, and Average salaries of the jobs.

### Objectives
My aim was to answer the questions: 
1. Does the Location, Size, Sector, Revenue or Age of the company predict the Lower, Upper and Average salary of the job being advertised? 
2. Which of those variables are the best predictors of salary?

### Exploratory Data Analysis
I first looked at the five-number summary of the Lower, Upper and Average salaries. I was interested in the relationship between Age and each salary level so I looked at the correlations and found they were all less than 0.035, indicating an insignificant relationship. I compared the density curves of the three salary levels and found the most variation in the Upper salary estimates. I noted that these curves did not seem to be normally distributed as there was right skewness in all three.

   ![](/images/density_curve.png)
    
Focusing on Average salaries, I looked at the salaries based on company size, sector, and location to find the relevant groups with the largest and highest average salaries, and widest interquartile ranges. Interestingly, companies with a size of 51-200 and 10,000+ had very similar interquartile ranges. For sectors, Telecommunications, Accounting & Legal and Media were the top three sectors with the highest Average salary. Telecommunications and Finance were the two sectors with the widest interquartile ranges.

   ![](/images/salary_by_sector.png)
   
I looked at the relationship between five of the sectors that had the most job postings (they accounted for 71% of the job postings), Age, and Average salary. The older companies tend to be in the sectors Biotech & Pharmaceuticals, Insurance and Finance, and the younger companies are in Business Services and Information Technology. This was not a surprise. The ellipses represent 95% confidence levels. Judging by the fact that the dots for the older companies are largely concentrated in the same salary range as the younger companies, it didn’t seem that I could conclude that Age and Sector together have an effect on Average Salary.

   ![](/images/salary_age_sector.png)

### Methods Used In Analysis
1-way and 2-way MANOVA, multivariate linear regression, and testing for nested models was used to identify the best explanatory variables for a model. After selecting a model, Cook’s distance and normality of residuals were tested to verify the appropriateness of the model.

### Conclusion
The results were that the Sector, Location and Size of the company advertising the jobs were the best predictors of Upper and Lower salaries. This information could be used by any person seeking a job in this field in the United States who wants to maximize their salary.

* The full project in PDF format can be found [here](https://drive.google.com/file/d/1MU2WsG_zJHyf-Zyx4M4JnaMYkhg1RaMV/view?usp=sharing)

## Project 2: An Analysis of TED Talks - A data mining group project <a name="project2"></a>
I completed my portion of this group project in R.
#### Project overview
"An Analysis of TED Talks" was a group project done for the course Introduction to Data Mining. My contribution to the project involved analyzing the tags on TED talks over 15 years to find the ones that occurred most frequently. After cleaning the data, I utilized a term frequency statistic to find the top 10% most frequently occurring tags per year. Then using the text mining Apriori Algorithm I found the individual tags, pairs of tags, and triplets of tags that occurred most frequently throughout all 15 years.

* The full project in PDF format can be found [here](https://drive.google.com/file/d/1vzVzmsnDbTi1Ui9a2HhYrW5t8w63TjhZ/view?usp=sharing)


## Project 3: My Fitness Friend (MFF) - A group project Android App development <a name="project3"></a>
This project was coded in Java, and the app was developed using Android Studio.
#### Project overview
The MFF app tracks calories consumed and calories burned each day and calculates how many more are required to hit user-defined goals. It also shows graphs of daily caloric and macronutrient summaries. By clicking on the Add Food button corresponding to a particular meal, a user is able to select foods and add them as a food eaten for breakfast, lunch, dinner or snack. They can also click Add Water to enter in how many cups of water they've drank. After adding a food, that food is visible under the corresponding meal and a sum of calories consumed in that meal is shown and updated as foods are added. A running tally can also be seen at the top of the screen where a calculation is done for the number of calories remaining to be consumed that day. When clicking on the View Daily Summary button, the grams of fat, carbs and protein consumed is shown for the current day. The proportion of calories consumed in fat, carbs and protein is also shown as a pie chart. Clicking on View Profile will allow the user to enter a goal for the daily maximum number of calories they want to consume, and a goal for daily water consumption in number of cups. The user can select exercises from a list and enter in the duration they performed the exercise for. The user can enter a reflection about their day.

Here are screen shots displaying the different functionalities of the app:

   ![](/images/mff_screen_1.png)
   
   ![](/images/mff_screen_2.png)

* Java code written by me is found [here](https://github.com/AMUnrau/my-fitness-friend/blob/main/ExerciseItemPageActivity.java) and [here](https://github.com/AMUnrau/my-fitness-friend/blob/main/SearchExerciseActivity.java)
