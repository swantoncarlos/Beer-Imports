# Beer-Imports
Python Project 


Customs declarations 2017-2022.

This is my first project in Python. I have downloaded the customs declarations for beers that entered Ecuador between January 2017 and August 2022.
I have used Pandas to clean the database and Matplotlib to do the visualizations.

In the first part of the project I have used a "for loop" to join the 6 databases corresponding to the previously indicated period. After appending the databases, I have cleaned up the merged database. Mainly I have changed the name of the columns, dropped the columns that are not necessary for the data analysis, analyzed the "missing values" and made sure that there is no "bad data".

The most complicated aspects in the process of cleaning the database was:

  1. There were 2 columns with the name of the beer brand. I have decided to go for the one with the least missing values (414) and fill the missing values with a fillna of the column that gives the commercial description of the beer. In many cases the description has the name of the brand.

  2. The second biggest challenge was grouping the brands. That is, that the beer brand column is grouped correctly. They had
  instances where the same brand appeared in different formats. Example: (Corona, CORONA, Corona Extra, Coronita). This is important for
  when you need to analyze the data of the most imported brand.
  
  3. Clean the country of origin column. The country of origin is the place where the beer is produced. For some reason, Ecuador appears as a place of
  origin in more than 300 occasions. This should not be the case because the database is for customs declarations (Imports). Given this, there is no
  reason for Ecuador to appear in the place of origin. I have replaced Ecuador with "others".
  
  Now that I have a smaller, cleaner and tidier database. I'm going to work with her to answer certain questions.
  
  - What has been the trend of beer imports in Ecuador since 2017?
  - Is more beer been imported troughout the years or is it getting more expensive to import beer to Ecuador?
  - Which is the leading company in beer importation? Which beer do they import the most?
  - Which import do Ecuadorians import the most (USD)?
  - Where do beers come from?
  - What has been happening with freight costs?
