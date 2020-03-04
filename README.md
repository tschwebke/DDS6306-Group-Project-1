# MSDS 6306: Doing Data Science - Case Study 01

## Group Members
- Thad Schwebke
- Rajesh Satluri
- Kris Ghimire

### Introduction

Using the Beer and Breweries data files provided by Budweiser, our group was able to uncover 
information that could be beneficial for Budweiser if they are considering entering the craft 
beer market in the United States. 

The information we focused on was breweries by State, beer styles, container sizes, Alcohol by 
Volume (ABV), and International Bitterness Units (IBU).

The data provided for this analysis consists of 2410 US craft beers from 558 US breweries. The 
data analysis that follows highlights the following in order to describe the current craft beer 
market:

The purpose this project is to provide descriptive information about the current craft beer market 
in the United States.


### The Data
Beers dataset contains a list of 2410 US craft beers and Breweries dataset contains 558 US
breweries. The datasets descriptions are as follows.
Beers.csv:
Name: Name of the beer.
Beer ID: Unique identifier of the beer.
ABV: Alcohol by volume of the beer.
IBU: International Bitterness Units of the beer.
Brewery ID: Brewery id associated with the beer.
Style: Style of the beer.
Ounces: Ounces of beer.

Breweries.csv:
Brew ID: Unique identifier of the brewery.
Name: Name of the brewery.
City: City where the brewery is located.
State: State where the brewery is located.

### Folder & File Information

- `analysis/` contains the reports generate when conducting the EDA.

  + `report.html` report generated by DataExplorer library. The report contains Basic Statistics, 
  Data Structure, Missing Data Profile, Univariate Distribution plots, Correlation Analysis, and 
  Principal Component Analysis.
  + `report_files` supporting files for the report.html report
- `data/` Containsthe data files used in this study.

  + `Beers.csv` list of 2,410 craft beers and their attributes.
  + `Breweries.csv` list of 558 breweries within the United States and their attributes.

- `docs/` contains all the background information important for understanding
the purpose of the study. This folder contains two files.

  + `CaseStudy01Sp2020_2.docs` the case study document that outlines the questions to be answered
  by this study.
  + `CaseStudy1 Rubric.docx` requirements document that contains the requirements the study must 
  contain upon submission.

- `final/` this folder contains the files required for the group project final submission.

  + `DS6306 Group Project 1.pptx` final presentation used to share the findings for this study.

- `Case Study 01.rmd` the Rmarkdown with code and analysis for this study
- `Case Study 01.docx` the Knit document version of the Case Study 01.rmd Rmarkdown file
- `Case Study 01.html` the Knit HTML version of the Case Study 01.rmd Rmarkdown file
- `DDS6306-Group-Project-1.Rproj` R project file for Case Study 01 project
- `README.md` the repo file and folder definition, and the answer to the analysis questions

# Analysis Questions TODO<insert code and answers to questions>

1.   How many breweries are present in each state?

2.   Merge beer data with the breweries data. Print the first 6 observations and the last six 
observations to check the merged file.

3.   Address the missing values in each column.

4.   Compute the median alcohol content and international bitterness unit for each state. Plot 
a bar chart to compare.

5.   Which state has the maximum alcoholic (ABV) beer? Which state has the most bitter (IBU) beer?

6.   Comment on the summary statistics and distribution of the ABV variable.

7.   Is there an apparent relationship between the bitterness of the beer and its alcoholic content? 
Draw a scatter plot.  Make your best judgment of a relationship and EXPLAIN your answer.

8.  Budweiser would also like to investigate the difference with respect to IBU and ABV between 
IPAs (India Pale Ales) and other types of Ale (any beer with “Ale” in its name other than IPA).  
KNN classification is used to investigate this relationship.  Provide statistical evidence 
one way or the other. Budweiser audience is comfortable with percentages … KNN is very easy to 
understand conceptually.

In addition, while you have decided to use KNN to investigate this relationship (KNN is required) 
you may also feel free to supplement your response to this question with any other methods or 
techniques used.  Creativity and alternative solutions are always encouraged.  

9. Knock their socks off!  Find one other useful inference from the data that you feel Budweiser 
may be able to find value in. You must convince them why it is important and back up your conviction 
with appropriate statistical evidence. 

## Conclusions TODO<write the final conclusion>

In summary, this primary objective of this work is to take two different data files which are beer and breweries data, read the data from the a csv file into a data frame, inspect and understand the structure of the data, merge the data frames, and perform some analysis on the final data set.

As Data Scientist, it is very rare to work only on a single perfect data and thus a large percentage of work will be accept different datasets, merge different available data sets before processing it as illustrated in this work. After preparing the data, statistical inference can then be made to the data. 

Based on the analysis, California and Colorado are top two which have most breweries. If order the all the data by Brewery and Beer IDs. The first six observations include beer names: Parapet ESB, Stronghold, Pumpion, Wall's End, Maggie's Leap and Get Together. The last 6 obervations include beer names: Pilsner Ukiah, Porkslap Pale Ale, Moo Thunder Stout, Snapperhead IPA, Heinnieweisse Weissebier and Urban Wilderness Pale Ale; Out of 2410 total rows of the data, there are two columns having NA's: ABV has 62 and IBU has 1005. 

After computing the median alcohol content and international bitterness unit for each state. DC has the highest median ABV, MS has the highest median IBV; UT has the lowest median ABV, SD has the lowest median IBV. But Co has the mximum alcoholic (ABV) beer and OR has the most bitter(IBU) beer. Afer running the summary statistics to ABV variable, the min ABV is 0.001 and the max ABV is 0.128. The Mean is 0.05977 and the median is 0.056. It has a littble bit skewness here. Based on the scatter plot, there is no linear relation between the bitterness of the beer and the alcoholic cotent.