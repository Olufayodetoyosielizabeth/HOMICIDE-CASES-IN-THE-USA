# Homicide-Cases-in-the-USA

## My first Data Analysis Project at [Edge Line Careers](https://www.linkedin.com/company/edgeline-careers/)

## INTRODUCTION
The dataset is for the analysis on the patterns and trends of homicide cases in the United States recorded from the year 2007 to 2017. Homicide is a tragic act of violence resulting in the loss of human life. The findings from this analysis hold great importance for law enforcement, policymakers and community advocates, as they contribute to the ongoing efforts to create safer communities and protect lives across the United States.

## ABOUT THE DATA/DATA COLLECTION
It is a structured data, and it is a secondary data collected. The data contains a table in xlsx file with 52180 rows and 15 columns. The data was gotten from Kaggle under the instruction of [Ganiyat Olajumoke Ajala](https://www.linkedin.com/in/ganiyat-olajumoke-abe/).

The analysis to be carried out is to answer the following questions:

1.	What are the top 10 states with the highest number of cases?
  
2.	What are the top 10 cities with the highest number of cases?
   
3.	What is the number of cases by gender?
   
4.	What is the number of cases by race?
   
5.	What is the number of cases by disposition?
    
6.	Provide a breakdown of the number of cases by age group.
    
7.	How has the number of cases over the years been?
    
8.	How does the distribution of cases vary by month?

## TOOLS
The tool used is Microsoft excel for data cleaning and analysis.

## DATA CLEANING AND TRANSFORMATION
The following are the different cleaning procedures:
•	Renamed:

	uid to ‘Unique Identifier’

	reported_date to ‘Reported Date’

	victim_first to ‘Victim First Name’

	victim_last to ‘Victim Last Name’

	victim_race to ‘Victim Race’

	victim_age to ‘Victim Age’

	victim_sex to ‘Victim Sex’

	city to ‘City’

	state to ‘State’

	lat to ‘Latitude’

	ion to ‘Longitude’

	disposition to ‘Disposition’

•	A date under the reported date, has an incorrect date format, ‘2015/05/105’ but was changed to ‘Not Specify’.

•	The Abbreviated Words Under State were changed to their full meaning using the find and replace tab for easy readability.

•	The blanks in Lat and Ion were changed to unknown using the find and replace tab.

•	The Reported Date was divided using text to column and the fixed width to split into three columns. Then used the CONCAT function to join the three columns together inserting / sign in between them to form a date format. Created two columns for year and month separately using the TEXT function and was named ‘Year’ and ‘Month’ respectively.

•	Age group column was created out of the Victim Age Column using the IF function.


## DESCRIPTIVE DATA ANALYSIS(DDA) AND DATA VISUALIZATION TECNIQUES
For the analysis to be understood and the questions to be answered, pivot tables and pivot charts were created to efficiently summarize and visualize the data. The following consist of questions, its analysis and insight for each:
 
1.	What are the top 10 states with the highest number of cases?

A pivot table was created having the fields ‘state’ and ‘unique identifier’. The function ‘count’ was used to get the total number of cases in the states and the top 10 states was selected using the ‘value filter’. The Pivot table showed Top 10 states with the highest number of cases, with California having the highest number of 6288 cases.

 ![image](https://github.com/Elizabhettie/Homicide-Cases-in-the-USA/assets/153202306/103abf8f-c1e2-4a2e-9d4d-fb9f1e836d75)

The image above is the clustered column chart created to show the top 10 states with the highest number of cases.

2.	What are the top 10 cities with the highest number of cases?

A pivot table was created having the fields ‘city’ and ‘unique identifier’. The function ‘count’ was used to get the total count of homicide cases in the cities and the top 10 cities was selected using the ‘value filter’. The Pivot table showed Top 10 cities with the highest number of cases, with Chicago having the highest number of 5535 homicide cases.

 ![image](https://github.com/Elizabhettie/Homicide-Cases-in-the-USA/assets/153202306/ae1bcdec-9f15-4a93-9e0c-b51ed82cd670)
 
A clustered column chart was created to show the top 10 cities with the highest number of cases.

3.	What is the number of cases by gender?

To analyse the number of cases by gender, a pivot table was created using the fields 'gender' and 'unique identifier'. The 'count' function was used to calculate the total number of cases by gender involved. The pivot table displayed the gender and their corresponding number of cases, with the male having the number of 40739 cases, the female with 7209 cases and the unknow with 4231cases. 

![image](https://github.com/Elizabhettie/Homicide-Cases-in-the-USA/assets/153202306/176a2e6d-f399-41bc-b352-4b5f3ca9f953)
 
 A clustered column chart was created to show the number of cases by gender.

4.	What is the number of cases by race?

To analyse the number of homicide cases by the race involved, a pivot table was created using the fields 'race' and 'unique identifier'. A function called 'count' was used to count the number of cases by the race involved. The pivot table showed the race involve with the number of cases. The race includes Black, Hispanic, White, Unknown and Other. The black race with 33361 number of cases is the race with the highest number of cases. 

![image](https://github.com/Elizabhettie/Homicide-Cases-in-the-USA/assets/153202306/4ea83ca8-be4f-4878-9319-034b9fce4c7b)

A clustered column chart was created to show the number of cases by race.

5.	What is the number of cases by disposition?

A pivot table was created using the fields 'disposition' and 'unique identifier'. A function called 'count' was used to count the number of cases by the race involved. The pivot table showed the race involve with their number of cases. The race includes Black, Hispanic, White, Unknown and Other. The black race with 33361 number of cases is the race with the highest number of case. 
 
![image](https://github.com/Elizabhettie/Homicide-Cases-in-the-USA/assets/153202306/272a55ff-c49c-4b7a-9b97-ed321b33b2d5)

A clustered column chart was created to show the number of cases by disposition.

6.	Provide a detailed breakdown of the number of cases by age group.

A pivot table was created using the fields 'age group' and 'unique identifier'. A function called 'count' was used to count the number of cases by the distribution of age group. The pivot table showed the age group 0-9, 10-19, 20-29, 30-39, 40-49, 50-59, 60-69, 70-79, 80-89 and 90+ and their number of cases. The 20-29 age group with 18561 number of cases has the highest number of cases.

![image](https://github.com/Elizabhettie/Homicide-Cases-in-the-USA/assets/153202306/629ee4d8-e01f-4c62-94aa-991bc39f277e)

A clustered column chart was created to show number of cases by distribution of age group.

7.	How has the cases over the years been?
   
A pivot table was created having the fields ‘year’ and ‘unique identifier’. The function ‘count’ was used to get the total count of the cases per year. The Pivot table showed that 2016 have the highest number of cases with 6290 number of cases. It showed that number of cases in 2009 decrease then increase in 2010 and as the year progressed there is increase in the number of cases.

 ![image](https://github.com/Elizabhettie/Homicide-Cases-in-the-USA/assets/153202306/8010f3ff-2d9c-47ff-b790-b0c5a66219e8)

The image above is the line chart created to show the trend of cases from the year 2007 to 2017.

8.	How does the distribution of cases vary by month?

A pivot table was created having the fields ‘month’ and ‘unique identifier’. The function ‘count’ was used to get the number of cases by the distribution of cases over the months. The Pivot table showed that July has the highest number of cases with 5034 number of cases. It showed that number of cases in the month of January and March were similar with 4037 number of cases in January and 4031 number of cases in March.

 ![image](https://github.com/Elizabhettie/Homicide-Cases-in-the-USA/assets/153202306/081ed8f9-027c-406c-9c66-b3563ee6bb84)

The image above is the clustered column chart created to show number of cases by distribution of cases over months.

## INSIGHTS AND RECOMMENDATIONS
