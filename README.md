# Project Portfolio

## Table of contents
1. Data Science
    1. [Multivariate Analysis](#project1)
    2. [Text Data Mining](#project2)
2. Programming

## Project 1: Multivariate Analysis of Data Science Job Salaries <a name="project1"></a>
This project was completed in R and the report was produced using R Markdown.
#### Project overview
* The data set contains several hundred Data Science-related job listings in the United
States scraped from the website Glassdoor. The purpose of this research was to determine
which of a particular subset of explanatory variables had an effect on the Lower,
Upper, and Average salaries of the jobs. 1-way and 2-way MANOVA, multivariate linear
regression, and testing for nested models was used to identify the best explanatory
variables for a model. After selecting a model, Cook’s distance and normality of residuals
were tested to verify the appropriateness of the model. The results were that the
Sector, Location and Size of the company advertising the jobs were good predictors of
Upper and Lower salaries. This information could be used by any person seeking a job
in this field in the United States who wants to maximize their salary.
#### Full report and sample of visuals
* The full project in PDF format can be found [here](https://drive.google.com/file/d/1MU2WsG_zJHyf-Zyx4M4JnaMYkhg1RaMV/view?usp=sharing)

* Sample of the exploratory data analysis visuals:

    ![](/images/avg_salary_by_sector.png)
    ![](/images/groups_avg_salary_top5sector.png)


## Project 2: An Analysis of TED Talks - A data mining group project <a name="project2"></a>
I completed my portion of this group project in R.
#### Project overview
"An Analysis of TED Talks" was a group project done for the course Introduction to Data Mining. My contribution to the project involved analyzing the tags on TED talks over 15 years to find the ones that occurred most frequently. After cleaning the data, I utilized a term frequency statistic to find the top 10% most frequently occurring tags per year. Then using the text mining Apriori Algorithm I found the individual tags, pairs of tags, and triplets of tags that occurred most frequently throughout all 15 years.

* The full project in PDF format can be found [here](https://drive.google.com/file/d/1vzVzmsnDbTi1Ui9a2HhYrW5t8w63TjhZ/view?usp=sharing)
