# Netflix Content Analysis - Exploratory Data Analysis (EDA)

## Project Overview
This project focuses on an **Exploratory Data Analysis (EDA)** of Netflix's content library using a dataset from Flixable (as of 2019). The analysis uncovers trends in Netflix's content strategy, regional variability, and content characteristics, providing actionable insights for business strategy optimization. The dataset includes 7787 titles, covering movies and TV shows, with plans to enrich the data using external sources like IMDB ratings and Rotten Tomatoes in future iterations.

### Project Type
- **Type**: EDA
- **Contribution**: Individual

## Problem Statement
The dataset reveals a significant shift in Netflix's content strategy:
- TV shows have nearly tripled since 2010, while movies have decreased by over 2000 titles.
- Key questions:
  - What are the implications of this shift towards TV shows?
  - How does content type vary across regions?
  - (Optional) Can clustering uncover latent themes in the content?

## Business Objectives
1. **Exploratory Analysis**: Identify patterns, trends, and anomalies in Netflix's content offerings.
2. **Regional Analysis**: Analyze content distribution across countries to inform localized strategies.
3. **Content Strategy Evaluation**: Assess Netflix's pivot towards TV shows and its alignment with business goals.
4. **Clustering (Optional)**: Use unsupervised learning to group similar content based on textual features for better categorization.

## Dataset Overview
- **Source**: Flixable (2019)
- **Size**: 7787 rows, 12 columns
- **Columns**: `show_id`, `type`, `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `rating`, `duration`, `listed_in`, `description`
- **Challenges**: Missing data (e.g., 2389 missing directors, 507 missing countries)

## Key Findings
### 1. Content Evolution
- **Movies vs. TV Shows**:
  - Movies peaked at 1497 titles in 2018 but dropped sharply by 2020 (over 2000 fewer titles since 2010).
  - TV shows nearly tripled, peaking at 737 titles in 2019.
  - The percentage of TV shows added rose from 0% in 2010 to a peak of 40% in 2014, stabilizing around 30-35% by 2020.
  - **Insight**: Netflix is prioritizing TV shows to cater to serialized storytelling preferences, but the decline in movies risks alienating movie-focused audiences.

### 2. Regional Variability
- **Top Countries**:
  - United States: Over 1800 titles, favoring movies.
  - India: 852 titles, also favoring movies.
  - Japan and the Philippines: More balanced mix of movies and TV shows.
- **Ratings**:
  - U.S. and India have a high proportion of TV-MA and NR content.
  - Smaller markets (e.g., Nigeria) have fewer titles, often with NR ratings.
  - **Insight**: Regional preferences vary, offering opportunities for tailored content strategies.

### 3. Content Characteristics
- **Ratings Distribution**: TV-MA (2863 titles) and TV-14 (1931 titles) dominate, focusing on mature and teen audiences.
- **Duration Trends**: Movies average 90-100 minutes; TV shows typically have 1-2 seasons, ideal for binge-watching.
- **Genres**: Dramas, comedies, and international movies lead, with documentaries and kids' TV also significant.
- **Insight**: Netflix curates accessible, binge-friendly content with broad appeal.

## Visualizations
Below are key visualizations from the analysis:
- **Yearly Content Trends**: Movies vs. TV Shows (Line Chart)
- **Yearly Percentage of TV Shows**: Percentage of TV Shows Added Over Time (Line Chart)
- **Content Type by Country**: Distribution of Movies and TV Shows in Top 15 Countries
- **Content Rating Distribution**: Ratings Across Top Countries
- **Genre Distribution**: Treemap of Genres in Top Countries

*Note*: Visualizations are generated in the notebook using Plotly and Seaborn.

## Business Recommendations
1. **Balance Content Mix**:
   - Increase movie offerings in regions like the U.S. and India to retain movie audiences while growing TV shows.
2. **Localize Strategies**:
   - Tailor content by region (e.g., more TV shows in Japan, more movies in the U.S.).
3. **Leverage Clustering (Future Work)**:
   - Use clustering to uncover latent themes, improving content categorization and recommendations.

## How to Run the Project
### Prerequisites
- Python 3.x
- Libraries: `pandas`, `numpy`, `seaborn`, `matplotlib`, `plotly`, `wordcloud`

### Steps
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Place the dataset (`NETFLIX MOVIES AND TV SHOWS CLUSTERING.csv`) in the project directory.
4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Netflix_EDA_final.ipynb
   ```
5. Follow the notebook to explore the analysis and visualizations.

## Future Work
- Integrate external data (IMDB, Rotten Tomatoes) for deeper insights.
- Implement clustering algorithms to group content based on textual features.
- Expand regional analysis to include more countries and viewer demographics.

## Conclusion
Netflix’s shift towards TV shows aligns with viewer preferences for serialized content, but the decline in movies calls for a balanced approach. Regional differences highlight the need for localized strategies, and understanding content characteristics can guide future investments to enhance Netflix’s global appeal and subscriber retention.

---

**Author**: [Your Name]  
**Date**: May 2025  
**License**: MIT