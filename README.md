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
! [ Netflix Data Model ] (

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
  
