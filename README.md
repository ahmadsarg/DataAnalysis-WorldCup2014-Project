# DataAnalysis-WorldCup2014-Project
### Project Description
The project involves analyzing historical international football match data to derive insights into team performances, focusing specifically on teams that participated in the FIFA World Cup 2022. The dataset includes various match statistics, including scores, FIFA rankings, and detailed player performance metrics. The primary objectives are to:

1. Assess the impact of home advantage on match outcomes.
2. Analyze the performance metrics of teams, particularly focusing on defense, midfield, and offense scores.
3. Identify the top-performing teams in various aspects (defense, midfield, offense) leading up to the World Cup 2022.
4. Examine the relationship between team performance metrics and the number of goals scored.

### Techniques Used

#### 1. Data Cleaning and Preparation
- *Handling Missing Values*: 
  - Columns with missing values were identified, and missing values were filled with the mean values for each team. This technique ensures that the analysis is not biased by missing data while maintaining the integrity of team-specific performance metrics.

- *Date Conversion*: 
  - The date column was converted from string to datetime format using pd.to_datetime to facilitate time-series analysis and ensure accurate sorting.

- *Dropping Unnecessary Columns*: 
  - Columns such as home_team_total_fifa_points, away_team_total_fifa_points, city, country, home_team_continent, and away_team_continent were dropped to simplify the dataset and focus on relevant features.

#### 2. Data Exploration and Visualization
- *Pie Chart for Home Advantage*: 
  - The proportion of home team wins, losses, and draws in non-neutral locations was visualized using a pie chart to assess the home team advantage.

- *Bar Plots for Team Performance*: 
  - Bar plots were used to visualize the top 10 teams based on their defense, midfield, and offense scores. This visualization helps in identifying the strengths of different teams in various aspects of the game.

#### 3. Feature Engineering
- *Combining Home and Away Team Metrics*: 
  - Home and away team performance metrics were combined into a single dataframe to facilitate analysis. This was done by concatenating the dataframes and renaming columns appropriately.

- *Filtering for FIFA 2022 Teams*: 
  - A subset of the data was created to focus on matches involving the teams that participated in the FIFA World Cup 2022. This subset was used for further detailed analysis.

#### 4. Analysis and Insights
- *Ranking Teams*: 
  - The latest FIFA rankings for each team were identified by selecting the most recent match data for each team. This helped in creating a ranking of the top teams participating in the World Cup.

- *Top 10 Teams in Defense, Midfield, and Offense*: 
  - Teams were ranked based on their mean scores in defense, midfield, and offense. This ranking was used to identify the strengths of the top teams.

- *Goals Scored Analysis*: 
  - The total number of goals scored by each team was calculated by summing the home and away scores. This analysis aimed to relate team performance metrics with their goal-scoring capabilities.
