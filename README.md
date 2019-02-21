
# Project 1: SAT & ACT Analysis


#### by Jane Liang  on  Nov. 11 2018 

## Problem Statement

Nearly every four-year college and university require high school students to take the **SAT** or **ACT** as part of the college admissions process for testing students' knowledge and aptitude on an equal playing field. The **SAT** and **ACT** are quite similar in many ways (intensive reading, cover algebra I&II, geometry, trigonometry, and an optional writing section) and have been about equally popular for several years. However, the SAT, once the nation’s dominant college admission exam, fell behind the ACT in recent years after its rival locked up testing contracts with more than a dozen states, including many in the Southern and Central regions of the country.The ACT had been the overall leader since 2012. 

In this EDA (Exploration Data Analysis), I will be analyzing **SAT** and **ACT** scores by state, as well as participation rates in the year of 2017 and 2018 for answering following specific questions:

-  What is the more commonly taken test in each state?
-  Which state has the highest or lowest rate of participation on SAT and ACT tests? Possible reasons? 
-  Which state has the highest or lowest SAT/ACT scores? Possible reasons?
-  Is there any patterns in the data? Any possible relations between subsets of the data? (i.e., scores vs participation rate)
-  What are the major differences between 2017 and 2018?  
-  What are some other interesting facts in the data?

According to the exploration of the data, we can make recommendation to College Board, which owns SAT in order to increase SAT participation.

## Data Description

Data source: <br>
[sat_2017](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/) |
[act_2017](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows) |
[sat_2018](https://reports.collegeboard.org/sat-suite-program-results/state-results) |
[act_2018](http://www.act.org/content/dam/act/unsecured/documents/cccr2018/Average-Scores-by-State.pdf) |


Below is a data dictionary which provides a quick overview of features/variables/columns for 2017 SAT & ACT and 2018 SAT & ACT.<br>

Data files:
[combined_2017.csv](./data/combined_2017.csv)
[combined_2018.csv](./data/combined_2018.csv)
### <center>The data dictionary of sat_2017 and act_2017<center>
|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|*object*|sat_2017|The state of the country|
|sat_2017_par|*float*|sat_2017|The participation rate of SAT test for the class of 2017(%)|
|sat_2017_ebrw|*integer*|sat_2017|The average scores of the SAT Evidence-Based Reading and Writing test in each state for the class of 2017|
|sat_2017_math|*integer*|sat_2017|The average scores of the SAT Math test in each state for the class of 2017|
|sat_2017_total|*integer*|sat_2017|The total average scores of the SAT test in each state for the class of 2017|
|state|*object*|act_2017|The state of the country|
|act_2017_par|*float*|act_2017|The participation rate of ACT test for the class of 2017(%)|
|act_2017_eng|*float*|act_2017|The average scores of the ACT English test in each state for the class of 2017|
|act_2017_math|*float*|act_2017|The average scores of the ACT Math test in each state for the class of 2017|
|act_2017_reading|*float*|act_2017|The average scores of the ACT reading test in each state for the class of 2017|
|act_2017_science|*float*|act_2017|The average scores of the ACT science test in each state for the class of 2017|
|act_2017_composite|*float*|act_2017|The average of four ACT test scores in each state for the class of 2017|

<br>
<br>
<br>


### <center>The data dictionary of sat_2018 and act_2018<center>
|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|*object*|sat_2018|The state of the country|
|sat_2018_par|*float*|sat_2018|The participation rate of SAT test for the class of 2018(%)|
|sat_2018_ebrw|*integer*|sat_2018|The average scores of the SAT Evidence-Based Reading and Writing test in each state for the class of 2018|
|sat_2018_math|*integer*|sat_2018|The average scores of the SAT Math test in each state for the class of 2018|
|sat_2018_total|*integer*|sat_2018|The total average scores of the SAT test in each state for the class of 2018|
|state|*object*|act_2018|The state of the country|
|act_2018_par|*float*|act_2018|The participation rate of ACT test for the class of 2018(%)|
|act_2018_composite|*float*|act_2018|The average of four ACT test scores in each state for the class of 2018|




## Executive Summary

### Contents:
- [2017 Data Import & Cleaning]
- [2018 Data Import and Cleaning]
- [Exploratory Data Analysis]
- [Data Visualization]
- [Descriptive and Inferential Statistics]
- [Outside Research]
- [Conclusions and Recommendations]
    
## Figures and Findings 
   
  [Presentation Link](./data/Jane.pdf)

    
    
## Conclusions and Recommendations   

From the data, it's reasonable to conclude that statewide testing causes lower scores because it includes all seniors and not just those planning to apply to college. 

Though the SAT remains popularity on the East and West coasts, the ACT is the more popular test in the Midwest in 2017. But this year, 2 million U.S. students from the class of 2018 took the SAT, compared with 1.9 million who took the ACT. About 1.7 million students took the SAT last year.The SAT is gaining momentum in recent years [Source: Politico.com](https://www.politico.com/newsletters/morning-education/2018/10/25/sat-scores-rise-as-do-the-numbers-of-test-takers-388387). The College Board has won key battles in the statewide-contract war. New contracts with Colorado and Illinois, College Board data show, were instrumental in the SAT’s growth. Some states require all juniors to take the SAT(Connecticut, Delaware, Maine, Michigan, and New Hampshire), while others, such as Idaho, Michigan, Illinois, Colorado, and New Hampshire have statewide contracts that cover the cost for students, and give students the option of taking either the SAT or ACT. Because the test wasn't mandatory for all students in these states for the entire school year, participation rates here are below 100%.

College Board pushed to expand its market share in recent years by revising the test(released in 2016, making it far more appealing as an assessment test than the older version of the test) and entering into deals with numerous states and school systems to give students the exam. In 2010, the College Board introduced a SAT School Day that offering free SAT exam during a regular school day with the cost covered by their schools, not their parents. In addition, students who choose to participate in SAT will be connected to resources and activities designed (e.g., Khan Academy) to help identify next steps for extra support or possible acceleration.

**Recommendations:** 

There are a number of other states where some schools or districts can administer the SAT to their students (either as an option or a requirement). These states are mainly located in Midwest and South where the ACT is dominated.
Direct method: Collaborate with state departments of education and local education agencies set up a statewide testing requirements, full or partial funding or free test preparation programs. 
Indirect method: Covering all or part of exam fees, Offer more SAT school Days, collect more data from school district to help find more suitable target. 


