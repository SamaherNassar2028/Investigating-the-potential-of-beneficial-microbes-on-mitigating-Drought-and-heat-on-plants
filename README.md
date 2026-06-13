# Investigating-the-potential-of-beneficial-microbes-on-mitigating-Drought-and-heat-on-plants
Expnaded Title: Investigating the potential of beneficial microbes—Agrobacterium and Arbuscular Mycorrhiza—on mitigating the effects of Drought and high Temperatures, on Black Seed Plants

**Updated as of June, 12th, 2026.

Research Question 1: How do beneficial microbes affect the height and qualitative survival indicator of plants under climate stress?
Research Question 2: What is the impact of microbial inoculation on chloroplast levels and leaf counts in stressed plants?

Name of the Dataset: Nigella sativa Resilience towards environmental stressors while subjected to microbial Inoculation.

**Note: Due to high climate-induced mortality rates observed within the *Nigella sativa* plants, additional ones from *Brassica oleracea* were added to the experiment to aid in reasonable sample sizes and statistical significance.

Dataset Source: Original experimental data collected by Samaher Faisal Nassar at the Chicago Botanic Garden. The project was conducted under the mentorship of Dr. Alicia Foxx.

Spatial and Temporal Coverage: Growth chamber at CBG, where the plants underwent a 5 week growth period following a 2 week germination period.

Variables:
  * `species`: Factor tracking plant varieties (*N. sativa* and *B. oleracea*).
  * `treatment`: Factor tracking 12 distinct environmental/microbial stress cohorts.
  * `final_height`: Continuous quantitative shoot height (cm) measured on 08/29.
  * `final_status`: Categorical qualitative survival score (0=Dead,1=Necrosis/Wilting, 2=Thriving).
  * `chlorophyll_final`: Continuous quantitative photosynthetic measurement.
  * `leaf_count_final`: Discrete count of emerged true leaves.

File Format: CSV, and xlsx.

Repository Structure
01_Code                # Documented R scripts numbered by execution sequence
01_data_cleaning.R
	02_analyze_data.R
03_make_figures.R
02_RawData         # Original, untouched greenhouse CSV spreadsheet data
03_ProcessedData # Cleaned, analysis-ready data
04_Results           # Output text files of statistical test results (.txt)
05_Figures          # Generated high-resolution data plots and graphics (.png)
06_Tables           # Calculated confidence interval summary metrics (.csv)
07_Final_Report # Final written paper

Preliminary Method Plan: 
1. Data Cleaning & Preparation 
a. Ensure deceased plants are handled separately to avoid skewing the data. 
b. Ensure uniform labelling and formatting of all variables to avoid errors or mishandling of data.

2. Catagorizing Variables (Monitored weeks 3-7) 
a. Independent: Treatment group (combinations of heat and/or drought stress along with Agrobacteria and Mycorrhizal inoculants). 
b. Dependant: plant height (mm), survival score (0-2).

3. Data Visualizations
a. A longitudinal growth line graph to show relative growth rates of groups subjected to different treatments.
b. Box plots of the final survivlal scores of each treatment group to visually compare within group and between group variation. 
c. Scatter plot of plant height v.s final survival score to visualize correlation between the two. 
d. Maybe a Survival Checkpoint Bar Chart to look at weekly progression.

* Google AI was briefly used here to provide examples of suitable data vizualization methods based on the data types available. 

5. Statistical Methods
a. Build 95% Confidence Intervals for mean height.
b. Conduct a t-test to find the difference between mean height of stresssed and control plants. 

6. Expected Outcomes
By the end of the project, I expect my results to indicate that the control groups are healthier than their stressed counterparts, but for the results to not be sufficient to reject the null hypothesis since the number of individuals with consistent data in the sample from the populations is not very high.
