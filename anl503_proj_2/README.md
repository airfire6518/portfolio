## Project 5: "Insights from Zoom Transcripts: Analyzing Student Engagement in the Digital Classroom"


### Introduction:

This project addressed the challenge of measuring and enhancing student engagement during remote learning sessions conducted via Zoom. Recognizing the potential of auto-generated transcripts as a rich source of data, my objective was to process and analyze these transcripts to understand patterns in student participation and inform strategies for promoting engagement.

### Data Processing and Database Integration:

**Transcript Parsing:**

Developed a Python program to parse the 'captured_dialogue.vtt' file, extracting structured data from the raw transcript text.
Employed regular expressions to accurately identify and separate different components of the transcript, such as serial numbers, timestamps, speaker names, and utterances.

**Database Table Creation:**

Using the extracted data, I created a MySQL table named ‘vtt’ with columns corresponding to the transcript's structure: SNo, TimeFrom, TimeTo, RegName, and Utterance.
The program ensured data integrity and correct formatting for direct database importation.

### Data Enhancement and Analysis:

**Time Duration Calculation:**

Executed SQL operations to construct a new table, ‘vttclean,’ which included all columns from ‘vtt’ plus a new column for ‘milliseconds.’
The new column represented the duration of each utterance, providing a quantitative basis for subsequent analysis.

**Visualization of Class Participation:**

Designed an R program to visualize the total airtime each student contributed during class, represented in milliseconds.
The bar chart created succinctly captured the level of participation, allowing for quick comparison and assessment of engagement.

<a href="https://airfire6518.github.io/portfolio/anl503_proj_2/img/vttclean.png">
    <img src="img/vttclean.png" alt="Example Image" width="300" height="200">
</a>
<p style="margin-top: 0;"><em>Total Airtime per Person</em></p>


### Skills and Tools Used:

- Demonstrated the ability to leverage Python for data parsing and preprocessing, utilizing libraries such as re, pandas, and pymysql.
- Showcased SQL proficiency in data manipulation and schema design, enabling the calculation of utterance durations.
- Applied R programming for the generation of a meaningful data visualization, using either base R graphics or ggplot2 to create a bar chart of student participation.


### Challenges Overcome:

Addressed the complexity of processing inconsistent and unstructured text data and converting it into a structured format suitable for database storage.
Problem-solved the precise calculation of conversation durations from timestamp data and the translation of this data into actionable insights.


### Conclusion:

The project exemplified the power of combining text processing, database management, and data visualization to derive practical insights from virtual classroom interactions. It underlined the importance of student participation as a metric for engagement and provided a data-driven approach to foster a more interactive learning environment.