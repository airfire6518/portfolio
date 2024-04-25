## Project 2: Integrating Python with R for Data Scraping and Analysis: A Study on GDP and Innovation


### Introduction:
This project demonstrates the powerful synergy between R and Python, two of the most prominent programming languages in data science. By harnessing Python's data scraping capabilities within RStudio, I extracted and analyzed World Intellectual Property Indicators from [Wikipedia](https://en.wikipedia.org/wiki/World_Intellectual_Property_Indicators) to explore the relationship between a country's GDP per capita and its propensity for innovation as measured by patent filings.


### Methodology:

**Python Integration:**

To bridge R with Python, I utilized the reticulate package, which provides a comprehensive set of tools for this purpose.
After ensuring Python was correctly installed on my system, I activated the Python interface within RStudio using reticulate::repl_python().

**Data Scraping:**

Python’s pandas library's read_html() function was employed to scrape tabular data directly from the Wikipedia page.
I filtered the table with the heading “Patents, trademarks, and industrial design filing activity by country of origin” and saved the extracted data as df_patents.
The data was then exported to a CSV file, patents.csv, for further manipulation in R.
Data Import and Preparation in R:

<img src=img/Df_patents.jpg alt="Example Image" width="300" height="200">
<p><em>Data Set Extraction Using Python (df_patents)</em></p>

<img src=img/CSV_patents.jpg alt="Example Image" width="300" height="200">
<p><em>Data Set Export into CSV (patents.csv)</em></p>

I imported the scraped data into R using the read.csv() command, ensuring continuity in data handling within a single environment.
To prepare for analysis, I joined the patent data with GDP per capita and population data from the provided ANL501_TMA_JAN24.xlsx file.
I computed the total patents per 100 thousand population by summing the patents for the years 2021 and 2022 and adjusting for population size.

<img src=img/Question_E_Merged.jpg alt="Example Image" width="300" height="200">
<p><em>The Final Merged Dataframe for Plotting</em></p>


**Visualization and Analysis:**

Utilizing R's ggplot2 package, I created a visualization to investigate the association between GDP per capita and total patents per 100 thousand population.
The visualization was refined with careful adjustments to improve readability and aesthetic appeal, including scaling, theming, and labeling.
The analysis provided a compelling visual representation of the relationship between a country's wealth and its innovation output.

<img src=img/Question_E.png alt="Example Image" width="300" height="200">
<p><em>Relationship Between GDP per Capita and Patents per 100,000 Population</em></p>

**Results and Discussion:**

The finalized plot revealed a noticeable trend suggesting a positive correlation between GDP per capita and the number of patents filed per 100,000 people, signifying that higher income levels may indeed be associated with increased innovation. However, the plot also indicated some outliers and variations, which suggests that while there is a general trend, there are also country-specific factors at play.


### Technical Proficiencies Showcased:
Fluency in R for data analysis and visualization.
Competence in Python for web-based data extraction.
Ability to integrate Python into the R environment using reticulate.
Skilled use of ggplot2 for creating insightful and polished visualizations.


### Challenges Overcome:
The main challenge was ensuring seamless communication between R and Python, particularly in maintaining data integrity across the transfer. Through careful debugging and validation of the data at each step, I ensured that the final dataset was accurate and ready for analysis.


### Conclusion:
This project not only reaffirmed the value of cross-disciplinary competence in data science but also provided evidence of a positive relationship between a country's economic prosperity and its capacity for innovation. This analysis underscores the importance of economic development in fostering an environment conducive to generating intellectual property.