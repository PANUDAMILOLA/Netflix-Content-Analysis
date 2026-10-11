# Netflix-Content-Analysis
An interactive Power BI project exploring Netflix content distribution , release-year trends, and genre representation.
## Project Background
  ### The growth of digital streaming platforms has expanded the availability of movies and television shows across different countries and regions. Understanding the composition and distribution of a streaming platform's content library can reveal patterns in content availability, geographical representation and release-year trends.
 ### This project explores a Netflix titles dataset using Power BI to examine the platform's content library, identify notable patterns, and present data-driven insights through interactive dashboards.
 ### The analysis focuses on understanding how titles are distributed geographically, how content releases vary across years, and how the collection is represented by different content categories.
 ## Insights and recommendations are provided on the following Key areas:
   -  Trend Analysis : Examining the distribution of titles across release-years to identify patterns, peak release periods, and year-over-year changes.
  -   Geographical Distribution: Analyzing the representation of titles across countries and regions to identify locations with the highest content representation.
  -  Content Collection Analysis: Exploring the composition of the content library, including the distribution of movies and TV shows and the representation of different genres.
  ## Data Structure and Initial Checks
  ### The project uses the Netflix titles dataset as its primary data source. During data preparation and modelling, additional tables were created to support genre analysis, geographical distribution, and measure, serve additional analytical and organizational purposes within the Power BI model.
  | Column | Description |
  |----|----|
  |Show ID | Unique identifier assigned to a content record.
  | Content Type | Indicates whether the content is a movie or TV Show.
  | Title | Name of the Movie or TV show.
  | Director |  Director associated with the content.
  | Country | Countries associated with the content.
  | Date Added | Date the content was added to Netflix.
  | Release-year | Year the content was originally released
  | Rating | Content rating classification
  | Duration | Runtime in minutes for movies or number of seasons for TV shows.
  | Genre | Category Associated with the content.

  | Column | Description |
  |----|---|
  | Show-id | identifier linking the content record to the corresponding title.
  |Content-type | indicates whether the content is a movie or TV show.
  |Genre | Category associated with the content.

  | Column | Description |
  |----|----|
  | Country | Country represented in the dataset
  | Region | Region assigned to the country for geographical analysis.
  ## Data Cleaning and Transformation
  Data cleaning and transformation were carried out in Power Query to prepare the Netflix Dataset for analysis in Power BI.
  The process focused on  improving data consistency, preparing fields for analysis, and structuring the data to support geographical and content-based insights.
  The Key Areas included:
  - Data Type Corrections: Reviewing column datatypes to ensure field were suitable for analysis.
  - Missing and Inconsistent Values: Examining missing values, data errors and placeholder entries that could affect the reliability of the analysis.
  - Genre Transformation: Preparing genre information to support analysis of different content categories represented in the dataset.
  - Country Transformation: Creating a country dimension and adding regional classifications to support geographical analysis.
## Data Modelling and Relationships
<img width="544" height="397" alt="image" src="https://github.com/user-attachments/assets/b29f3265-7402-4730-bd0d-7d80ae10570b" />


## Key Metrics
A set of DAX measures was developed to evaluate the composition of the Netflix content library, examine release_year trends, and support geographical analysis.

| Metric | Description | Analytical Purpose |
|-----|-----|------|
| Total Titles | Counts the titles represented in the dataset according to the measure's counting logic. | Evaluate Overall size of the content library. |
| Total Movies | Counts titles classified as movies. | Evaluates the movie component of the library. |
| Total TV shows | Counts titles classified as TV shows. | Evaluates the TV show component of the library. |
| Total Genre | Counts the distinct genres represented in the analysis. | Assesses the variety of content categories |
| Total Growth | Measures overall growth according to the DAX calculation. | It provides a high level view of growth. |
| Previous Year Releases | Returns the release count of the previous year where applicable. | Provides comparison point for year-over-year analysis. |
| YoY Change | Calculates the difference between the current year's and previous year's release counts. | Identifies increases or decreases in releases. |
| YoY Growth | Calculates the percentage change releases compare with the previous year. | Evaluates the rate of change in annual releases. |

## Executive Summary
This analysis provides an overview of content release patterns and geographical distribution, offering insights into the composition and evolution of Netflix's content library.


The findings revealed that 2018 was the peak release year, with 1,146 titles released. Overall catalogue growth reached 561, while the United States accounted for the largest share of the content collection, followed by India and the United Kingdom, highlighting the prominence of these counties in Netflix's content library.


<img width="884" height="547" alt="image" src="https://github.com/user-attachments/assets/0597eeb1-748e-4311-8afa-9d87fa6aaee0" />

## Trend Analysis
- Peak Release Year: 2018 recorded the highest number of titles, with 1,146 releases, representing year-over-year growth of 11%.
- Declining Trend: By 2021, the year-over-year change -346 titles, representing a 38% declined compared with the previous year.
- Year-Over-Year Fluctuations: The number of titles varied across release years, with periods of growth and decline rather than a consistent upward trend.
<img width="929" height="519" alt="image" src="https://github.com/user-attachments/assets/8e580d7e-253f-4f6f-920d-889a7eaa16bd" />

## Countries and Regional Distribution
- Regional Distribution: North America leads in title distribution, followed by Asia and Europe, highlighting the prominence of these regions in the Netflix dataset.
- United States Leads Country Distribution: The United States rank first with 3,239 titles across 68 genres. Its leading genres are Drama, Documentaries, and Comedies. With approximately three times as many titles as India.
- Differences in Country-Level Content Composition: India ranks second with 1,057 titles across 45 genres, with International Movies, Dramas, and Comedies leading its catalogue. The United Kingdom follows with 638 titles across 57 genres, led by British TV shows, International Movies, and International TV shows. These findings illustrate differences in both catalogue size and genre representation across the three leading countries.


