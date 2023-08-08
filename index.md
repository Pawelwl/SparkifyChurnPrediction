<div style="text-align: justify"> Stack Overflow runs an Annual Developer Survey every year since 2011. In this article the results of the survey are examined for a subgroup of developers that describe themselves as being from Data Science field. More specifically, they define themselves as 'Data scientist or machine learning specialist'. Five years of data (2018-2022) is analysed. </div> 

The survey data and other related details can be found [here](https://insights.stackoverflow.com/survey) 

The data analysis of the survey results aims to answer the following questions:

1. How do Data Scientists work (hybrid / remote / in-person)?
2. What is the education level of Data Scientists and how it has changed over time?
3. How Data Scientists learn to code?
4. How much Data Scientists earn and how the salaries differ between countries?
5. What are the most popular technologies used?
6. Do mental health problems and accessibility issues affect Data Scientists?

![Image](/docs/assets/blog_photo_1.JPG)

<div style="text-align: justify"> Between around 5% to 7% of survey participants describe themselves as Data Scientists, which is just a fraction of all types of professions that use Stack Overflow. The whole analysis presented below relates only to the Data Science area of expertise. </div> 

![Image](/docs/assets/DS_proportions.png)

Below I attempt to answer all the six questions using data analysis and visualistion.

#### 1. How do Data Scientists work (hybrid / remote / in-person)?
<div style="text-align: justify"> Around a half of Data Scientists worked in a hybrid model in 2022. 36% worked fully remotely and only 13% fully in-person. This information seems to be particularly important for companies that are willing to hire Data Scientists. If we assume that those proportions represent the working style preferences of Data Science community, a company that will require a full in-person attendance can lose an interest of on average seven out of eight candidates!</div> 

![Image](/docs/assets/DS_RemoteWork.png)

#### 2. What is the education level of Data Scientists and how it has changed over time?
<div style="text-align: justify"> By analysing the 5 most common education types in years 2018-2022 we observe increase in the highest levels of formal education (Master's and doctoral degrees) and decrease for the rest. This trends might be a result of Data Science requiring higher qualifications to be able to keep up with the more advanced technology that appears every year. On one side the Data Scientists might upskill themselves to get more advanced degrees. On the other side people who join this field might have already an advanced degree. </div>

![Image](/docs/assets/DS_EdLevel.png)

#### 3. How Data Scientist learn to code?
#### 3.1. Learning to code resources
<div style="text-align: justify"> Based on the chart below we can see that 'School' and 'other online resources' are the most important components in learning to code. Their importance raised in 2022. Books and online courses are also very important - more than a half of Data Scientists in 2022 learned coding using it. On the other side, Coding Bootcamp is not a primary resource for learning to code. </div>

![Image](/docs/assets/DS_LearnCode.png)

#### 3.2. Online resources to learn to code
<div style="text-align: justify"> We already know that online resources are widely used. Technical documentation, stack overflow and blogs are the most popular learning online resources. More than 50% of Data Scientists use also written tutorials, how-to videos and online books. Certification videos, programming games and auditory materials (e.g. podcasts) are not very common. </div>

![Image](/docs/assets/DS_LearnCodeOnline.png)

#### 3.3. Online courses or certifications used to learn to code
<div style="text-align: justify"> By far the most common platforms in 2022 are Coursera and Udemy. edX, Codecademy and Udacity are next, while being used by more than 20% of respondents. If we assume that what is the most commonly used is the most useful, this is a valuable information for companies which want to upskill their employees and for Data Scienstists as well if they want to learn new skills. </div>

![Image](/docs/assets/LearnCodeCoursesCert.png)

#### 4. How much Data Scientists earn and how the salaries differ between countries?
<div style="text-align: justify"> To answer this question a median monthly salary before taxes is compared for 12 most common countries in the survey in year 2022.  
The salary in country's currency is converted to EUR based on average exchange rate in 2022, which makes the comparison easier. </div>

![Image](/docs/assets/DS_MedainSalaryEUR.png)

<div style="text-align: justify"> After converting the median monthly salary to one common currency (EUR) it is possible to compare it between countries. The range is very wide, from ca. 12k EUR per month in the USA to 1.6k EUR in Brazil. This information can be very useful for Data Scientists looking for a job abroad. Also if a company is planning to build an international Team the information about median salary per country can be a good indicator of the people costs. For example a company based in the USA can hire 3 Data Scientists in Poland or 5 in India for the cost of one Data Scientist in the USA. From the perspective of a Data Scientist looking for a job abroad, not only salary matters, but costs of living as well. The information about living costs is provided based on data from numbeo (see references). 'Cost of Living Plus Rent Index' is used, which is an estimation of consumer goods prices including rent comparing to New York City. The value of the index for New York City is 100. </div>

![Image](/docs/assets/DS_MedainSalaryEUR_pivot.PNG)

<div style="text-align: justify"> While comparing not only the salary, but also taking into account the costs of living the hierarchy of countries changes (Look at the Financial_wellbeing_index columns which is the Median_Salary_in_EUR/cost_index). Still USA is the top pick. However, Switzerland which was top 2 according to salary only is on the 8th place when the cost of living is taken into account. Relatively good salary compared to costs have Data Scientists in India, Canada and Poland. </div>

#### 5. What are the most popular technologies used?
#### 5.1. Most popular languages
Five languages that seem to be the most relevant for Data Scientists are analysed in time: Python, R, Julia, Scala and SQL.

![Image](/docs/assets/DS_LanguageHaveWorkedWith.png)

<div style="text-align: justify"> Python is the most common language for Data Scientists. SQL and R are on the second and third place respecitvely. A growing interest in Julia and decreasing interest in Scala is visible. It will be interesting to observe Julia development in the upcoming years to see if the language will be accepted by the mainstream Data Science. The above information can be an good indicator for people planning to switch to a Data Scientist role. Learning Python seems as an obvious first choice, followed by SQL on the second place. </div>

#### 5.2. Most popular technologies
The following relevant from the point of view of Data Scientists technologies are analysed in time: Keras, NumPy, Pandas, TensorFlow, Torch/PyTorch.

![Image](/docs/assets/DS_MiscTechHaveWorkedWith.png)

<div style="text-align: justify"> Numpy and Pandas are the two top technologies among Data Scientists. Essentially they are Python libraries for numerical computations and data analysis. The other three technologies refer to deep learning. Tensorflow is the most popular one. However, when looking at the trends it seems that interest in Tensorflow is stable / decreasing while interest in Torch/PyTorch is rising. </div>

#### 6. Do mental health problems and accessibility issues affect Data Scientists?
#### 6.1. Accessibility
<div style="text-align: justify"> The first column in the below table presents options to select in a survey question related to accessibility. It's a multiple choice question. </div>

![Image](/docs/assets/DS_Accessibility_pivot.PNG)

<div style="text-align: justify"> Based on the survey results we can say that accessibility issues affect around 7% of the population of Data Scientists. There are different issues raised like problems with typing, walking, seeing or hearing. Awareness of the fact that 7 out of 100 Data Scientists might have problems like that is critical, especially for companies employing Data Scientists. For example, company policies regarding assitance for people with disabilities should be in place. Also recognizing the value of diversity and inclusion plays a key role here. </div>

#### 6.2. Mental Health
<div style="text-align: justify"> The first column in the below table presents options to select in a survey question related to mental health. It's a multiple choice question. </div>

![Image](/docs/assets/DS_MentalHealth_pivot.PNG)

<div style="text-align: justify"> Based on the survey results around 30% of Data Scientists have various mental health problems. The most common are concentration and/or memory disorder, anxiety and mood or emotional disorder. Around 4% respondents have autism spectrum disorder. The results show that mental health problems occur really often. In an average Team of 10 Data Scientists, 3 have various kinds of mental health issues. It is good that this question was added to stack overflow survey in 2021. Awareness that such problem exists and that the scale is significant is very informative, especially for companies who would like to create a great place to work for their employees. If a company offers a support for people with mental health problems it could be a significant benefit not only for existing employees, but also for prospective ones. </div>

#### Summary

<div style="text-align: justify"> The analysis, which is based on the results from stack overflow surveys run in years 2018-2022, provided interesting observations related to the way Data Scientists work, their education level, ways to learn, salaries, most common technologies and touches important subjects like mental health and accessibility issues.
Depending on the reader, if that is a Data Scientist, aspiring Data Scientist or someone from a company managing and building Data Science Teams, everyone should find interesting insights in the results of the analysis. </div>

#### References
[Jupyter Notebook based on which this article was created](https://github.com/Pawelwl/Stack_Overflow_Survey_Analysis/blob/main/Stack%20Overflow%20Survey%20Analysis%20-%20a%20Data%20Scientist%20perspective.ipynb) <br>
[Source Stack Overflow Survey Data](https://insights.stackoverflow.com/survey) <br>
[numbeo website - Cost of Living plus Rent Index](https://www.numbeo.com/cost-of-living/rankings_by_country.jsp?title=2022&displayColumn=2)
