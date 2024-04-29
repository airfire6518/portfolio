
## Project 1: Economic Growth and Population Dynamics: A Visual Story of Southeast Asia


### Introduction:
This project entry encapsulates my analytical exploration into the economic and demographic evolution of Southeast Asian nations from 1960 to 2022. The focal point of this project was to analyze and visualize the comparative trajectory of Singapore's GDP per capita in relation to its regional counterparts and to examine gender demographic proportions at key historical junctures.


### Data Import and Wrangling:
Leveraging the readxl package, data was meticulously imported from the "Population and GDP" worksheet within the ANL501_TMA_JAN24.xlsx file. I applied data filtering techniques to refine the dataset, concentrating on nine specified ASEAN countries. This subset was vital for maintaining a clear focus on the region's economic and demographic patterns. The creation of the df.asean dataframe entailed a transformation into a longitudinal format, ensuring each variable was clearly delineated across countries and years for subsequent analyses.

<a href="https://airfire6518.github.io/portfolio/anl501_proj_1/img/Source.png">
    <img src="img/Source.png" alt="Example Image" width="300" height="200">
</a>
<p style="margin-top: 0;"><em>ANL501_TMA_JAN24.xlsx (Source Data)</em></p>


<a href="https://airfire6518.github.io/portfolio/anl501_proj_1/img/Df_asean.png">
    <img src="img/Df_asean.png" alt="Example Image" width="300" height="200">
</a>
<p style="margin-top: 0;"><em>Dataframe (df.asean) in R</em></p>


### Data Analysis and Visualization:
The core of the analysis was the longitudinal review, which was meticulously carried out to ascertain the economic progression of each country with an emphasis on Singapore. Through a series of visualizations, I crafted comparative plots that narrated the story of Singapore’s economic journey, juxtaposed against its neighbors. By zeroing in on pivotal decades such as 1960 to 1970, I was able to uncover and depict specific historical economic phases, laying the foundation for a richer, context-driven exploration of the region's growth.

<a href="https://airfire6518.github.io/portfolio/anl501_proj_1/img/Question_B1.png">
    <img src="img/Question_B1.png" alt="Example Image" width="300" height="200">
</a>
<p style="margin-top: 0;"><em>Singapore vs. the Other Asean Countries (1960 ~ 2020)</em></p>

<a href="https://airfire6518.github.io/portfolio/anl501_proj_1/img/Question_B2.png">
    <img src="img/Question_B2.png" alt="Example Image" width="300" height="200">
</a>
<p style="margin-top: 0;"><em>Singapore vs. the Other Asean Countries (1960 ~ 1970)</em></p>


### Gender Proportion Bar Chart:
A focused demographic analysis was performed to determine the gender proportions within Malaysia, the Philippines, and Singapore for the years 1960, 1980, 2000, and 2020. Utilizing geom_bar with the stat="identity" parameter, I constructed bar charts that visually encoded the male-to-female ratios, offering an immediate understanding of demographic shifts. The data required pre-processing to accurately reflect these proportions and facilitate a side-by-side stacked representation for each gender category, enhancing the comparative clarity of the visualizations.

<a href="https://airfire6518.github.io/portfolio/anl501_proj_1/img/Question_C_df.jpg">
    <img src="img/Question_C_df.jpg" alt="Example Image" width="300" height="200">
</a>
<p style="margin-top: 0;"><em>The Dataframe after Pre-processing</em></p>

<a href="https://airfire6518.github.io/portfolio/anl501_proj_1/img/Question_C.png">
    <img src="img/Question_C.png" alt="Example Image" width="300" height="200">
</a>
<p style="margin-top: 0;"><em>The Break Down of Country Gender Proportion by Year</em></p>


### Data Animation with gganimate:
The animation phase brought to life the static images through the use of the gganimate package. I selected a GDP per capita visualization for this purpose, aiming to dynamically showcase Singapore's growth against the backdrop of its ASEAN peers. The animated plot, rendered as a GIF file, was then smoothly integrated into the accompanying Word document. This visual narrative captured the temporal dimension of economic development, illustrating not only the endpoints but the entire journey.

<a href="https://airfire6518.github.io/portfolio/anl501_proj_1/img/Question_D.gif">
    <img src="img/Question_D.gif" alt="Example Image" width="300" height="200">
</a>
<p style="margin-top: 0;"><em>Singapore vs. the Other Asean Countries - Animation</em></p>


### Discussions and Observations:
My observations from the static visualizations revealed Singapore's remarkable economic ascent, particularly when contrasted with the varying paces of its neighbors. The gender demographic analysis illuminated nuanced population structures, reflecting broader social and economic trends. The animated visualization underscored the changing economic landscape of Southeast Asia, with Singapore's rise to affluence being a standout story that unfolded over the span of six decades.


### Skills and Tools:
Throughout this project, I honed my proficiency in R and fortified my expertise in data manipulation (using dplyr), data tidying (with tidyr), data visualization (through ggplot2), and animated storytelling (via gganimate). These tools were instrumental in translating raw numbers into compelling visual stories.


### Challenges and Resolutions:
One challenge I encountered was ensuring the animated visualization conveyed the temporal trends without overwhelming the viewer. By iteratively refining the animation speed and transition effects, I achieved a balance that was both informative and engaging.


### Conclusion:
In conclusion, this project not only enriched my understanding of the region's economic and demographic trends but also served as a testament to my analytical and visualization skills. The processes and outcomes chronicled here substantiate my capacity to synthesize complex data into accessible and enlightening visual narratives.
