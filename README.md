# COVID_19_Illinois
An analysis of COVID-19 data from Illinois.

#Analysis of COVID-19 data in Illinois
  Objective of analysis: To figure out how to best allocate resources to help the population effectively in the next outbreak of a highly infective virus.
First, I downloaded the data from (I believe it was from https://covid.cdc.gov/covid-data-tracker, but I need to recheck that source) and I performed data exploration making sure the data was clean. I changed a few of the data types in the test columns from double to number when importing the data to Microsoft SQL Server Studio.
  To-do list for cleaning data:
1.	Look for null values. There are 15,236 null values in the zip code column. I checked to see how many zip codes there are in IL.
  a.	I’ve created two CTEs to try to compare the null and not null zip codes to see if there were any similarities in the data. Turns out there isn’t, but the population   for some of the populations are the same in the rows with zip codes and null zip codes.
2.	Make sure there’s no duplicates where there shouldn’t be. There are a few duplicates in the population column, but that’s probably to be expected when there’s no deaths.
3.	Make sure all the data types are correct. I need to change the ZIP_Code column to integer.

Analyzing the data:
1.	Figure out what the average infection rate per zip code is.
2.	Figure out which zip code had the highest and lowest infection rates.
3.	Label what each data type means
4.	After analyzing the data, see what policies each zip code had.
What I learned: 
1.	I learned how to conditionally format cells in Excel to display a certain color when there’s any text in it (using the =ISTEXT function), and I also learned how to search for cells in the worksheet that have a cell highlighted.
