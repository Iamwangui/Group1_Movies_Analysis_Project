 GROUP 1
 
 18th DECEMBER 2025


 OUTLINE:
          -Introduction and Objectives of the project\
          -Business Problem\
          -Data Understanding\
          -Methods\
          -Findings\
          -Recommendations\



INTRODUCTION AND OBJECTIVES OF THE PROJECT:

Using data from IMDB and Movie Budget Datasets, we set out to provide insights on movie 
genres, production budgets, and release-times of various movies.
The goal is to guide the launch of a new movie studio for our company.


BUSINESS PROBLEM:

The company’s management wants to enter the movie production industry but lacks experience in identifying what types of films are most likely to succeed.

This analysis aims to support management by answering the following key business questions:

  1. Which movie genres are the most profitable and well-received by audiences?

  2. Which genres perform well despite lower production budgets?

  3. Does the timing of a movie’s release impact its box office performance?


DATA UNDERSTANDING:

The analysis uses 2 datasets (IMDB Database and Movie Budgets dataset)that provide complementary information about movies:

The IMDB Database contains:

Movie Basics Table: Contains movie titles, genres, and release dates.

Movie Ratings Table: Includes average audience ratings and number of votes for each movie.

The Movie Budgets Dataset: Provides production budgets and the revenue figures.

These datasets will be merged to create a unified view of each movie’s genre, financial performance, audience reception, and release timing.     


 METHODS:
 
~ Loading data : We used pandas and sqlite3 to access and manipulate our datasets.
~ Data Cleaning : - Removal of null values and duplicates,if any.
                  - Stripping away non-numeric symbols like $ and commas.
                  - Changing text to float or numeric dtypes.
                  - Accessing the datetime object
~ Merging the two datasets using pandas.
~ Creating new features ie the Profit and release month columns.
~ Analysis : We used descriptive analysis to evaluate Profit, Cost of Production, and Timing,
             through aggregate values of grouped column means,counts and medians.
             We then used matplotlib and sns to offer an overview of these aggregations using plots.


FINDINGS:

A.
* Action-Adventure-Thriller leads profitability: This combination tops the list with $911M average profit among movies rated >=7, driven by broad appeal and potential.
* Family-Fantasy-Musical ranks second: Achieves $844M average profit, highlighting the strong commercial success of uplifting, family-friendly content with musical elements.
* Adventure dominates top performers: Appears in 8 of the top 10 genre combinations, serving as a key driver of high profits through escapism and excitement.
* Sci-Fi boosts profits: Combinations like Action-Adventure-Sci-Fi (approximately $630M) and Adventure-Drama-Sci-Fi (approximately $524M) show speculative elements enhance financial returns when paired with strong narratives.

B.

PROFIT MARTIN VS AUDIENCE RATING

From the table, there are movies that are well received e.g 8.5 ratings that had high profit margin. Although some with low ratings like 6.1 rating get high profit margin despite there weak reception.This shows that finanacial success does not align with what audience love or highly rate.


GENRE VS MOST PROFITABLE

Genres like (Action, Sci-Fi) and (Adventure,Animation, Comedy) drive the highest profits. Horror stands out as a cost-effective genre,since it has low budget and generates high revenue hence a high Profit margin despite the ratings.


GENRE VS AUDIENCE RATINGS

The top-rated genres are Documentary-based especially those with Drama, Crime, History, and Sport.
Action, Documentary, Drama leads with an average rating of 8.7, followed by Crime, Documentary at 8.25.
These genres are not the most profitable, but they are deeply appreciated by viewers(High ratings).


C.
 TOP 3 MONTHS FOR AVERAGE REVENUE:
  • Jun: $123.3M average revenue | 213% ROI
  • Nov: $109.7M average revenue | 401% ROI
  • May: $104.6M average revenue | 213% ROI

 WORST 3 MONTHS FOR AVERAGE REVENUE:
  • Sep: $29.4M average revenue | 151% ROI
  • Aug: $38.5M average revenue | 310% ROI
  • Oct: $39.4M average revenue | 440% ROI

 BEST SEASONS FOR RELEASE:
  • Summer: $86.2M average revenue
  • Spring: $80.7M average revenue

 WORST SEASONS FOR RELEASE:
  • Winter: $56.1M average revenue
  • Fall: $58.2M average revenue

 SUCCESS RATE ANALYSIS:
  • Highest success rate: Nov (70.2% of movies profitable)
  • Lowest success rate: Dec (55.6% of movies profitable)

 HIGH-BUDGET MOVIES (>$100M):
  • Best month for big budgets: Apr ($618.4M average revenue)






RECOMMENDATIONS:

A.
* Prioritize Action-Adventure-Thriller projects: Focus research, development and marketing resources in order to maximize returns on high-rated films.
* Increase investment in Family-Fantasy-Musicals: Develop more animated and musicals with fantasy themes to capture family audiences.
* Build films around Adventure cores: Combine Adventure with Family, Sci-Fi, or Fantasy elements to broaden appeal and boost profitability.
* Strategically integrate Sci-Fi: Adding visual effects elements to Action or Drama-Adventure films while managing budgets for stronger commercial outcomes.


B.
Therefore;

The most profitable genres are Action,adventure,Sci-Fi yet the are not rated as the top on the list.

Documentary genres receive high ratings suggesting real world content matter to the audience.

The company will determine whether the primary business objective is for commercial success or audience rating.This decision will guide the choice of genre and where to invest.




C.
1. MAXIMUM GROSS REVENUE
   • PRIME WINDOW: May & June (Summer Peak)
     - June leads with $123.3M average revenue per film.
     - School is out and 'vacation spending' is at its annual peak.
     - Reserve this for your highest-budget ($100M+) visual spectacles.
     - Success here requires a massive marketing to beat competitors.

2. HIGHEST PROFIT MARGINS (ROI)
   • PRIME WINDOW: October & November
    - October ROI hits 440%; November boasts a 70.2% success rate.
    - October is fueled by low-budget Horror fans (Halloween).
    - November captures the 'Family Thanksgiving' and 'Award Season' crowds.
    - Launch mid-budget dramas in Nov and low-budget Horror in Oct.
    - This maximizes profit with significantly less financial risk.

3. HIGH-BUDGET OPPORTUNITY
   • PRIME WINDOW: April
    - Big-budget movies (>$100M) average $618.4M in revenue here.
    - It's the 'Early Summer' slot. You capture the audience's hunger for
      blockbusters before the June/July market becomes oversaturated.
    - If you have a high-confidence 'Tentpole' film, release in April to
      own the market before the 'Summer Wars' begin.

4. RISK MITIGATION
   • AVOID WINDOW: September & January
    - September is the weakest month ($29.4M avg revenue).
    - Sept. is 'Back-to-School' (no time); Jan. is 'Holiday Hangover' (no money).
    - Do not launch original IP or high-priority films here. Use these
      months only for experimental films or contractual 'dumping'.

 FINAL SUMMARY
   - For GROSS:   Invest heavily in June/May.
   - For PROFIT:  Go Targeted in October/November.
   - For SAFETY:  Early release in April




