# The Winning Formula
## *A systematic strategy for success in the movie industry*

In this exercise, our group was charged with developing a strategy that Microsoft could use to successfully break into the movie industry. Our approach to this included gathering data about the movie industry that could be examined to reveal valuable insights, which we combined in order to develop *The Winning Formula*. *The Winning Formula* provides a clear course of action that will allow Microsoft to effectively designate their resources in order to secure success.

## Methodology
Our research methodology was guided by the first three steps in the OSMEN system. First, we focused on obtaining a sizable database of movies. Next, we focused on scrubbing the data in order to improve the quality of our insights. Finally, we performed exploratory data analysis (EDA) to reveal the insights provided by our data. Based on these insights, we created visualizations that illustrate the value of specific approaches. These approaches were combined in order to develop *The Winning Formula*.

## The Data
We collected the data that informed our analysis from an internet database called **The-Numbers.com**. The Numbers is a website that aggregates a wealth of data from movies all around the world. This website has a feature called *Report Builder* that allows the user to create reports based on a variety of available criteria, and tailors the information based on the preference of user. In order to improve efficiency, we used Python to automate the process of using *Report Builder* to gather our data.

The database that we created is comprised of approximately 1000 recent (2010-2019) high-grossing films.     
Our database contains the following information about these movies:   
* Release Year
* Genre (e.g. Action, Adventure, Comedy, Horror, etc.)
* Creative Type (e.g. Science Fiction, Kids Fiction, Fantasy, Factual, etc.)
* Theatrical Distributor (i.e. studio)
* Production Method (e.g. Live Action, Animated, etc.)
* Source (e.g. Original Screenplay, Based on literature, Spin-off, Remake, etc.)
* Production Budgets
* Domestic Box-Office Gross
* International Box-Office Gross
* Worldwide Box-Office Gross

#### Data Limitations
Every effort was made to ensure the quality and consistency of the data. However, we recognize that our analysis might be limited due to certain characteristics of the data that we selected. The following points should be considered:  

1) This data set does not examine profits that might be made from Pay-Per-View, Streaming Services, Cable, DVD, and merchandise.     
2) This data set includes Production Budget, but does not provide a breakdown of post-production costs, such as marketing, studio overhead, etc.  
3) This data set only includes 1000 of the most successful movies from the past decade.

## Navigating the Repo

### Part 1: Data Acquisition and Cleaning (Part_1_Data_Acquisition_and_Cleaning.jpynb)

#### Data Acquisition
Our data acquisition technique involved scraping data from a website called the-numbers.com. The numbers aggregates data from movie worldwide and stores them in a central database. We used a simple web scraper in order to obtain data from this website.

#### Data Cleaning
Our data cleaning techniques were selected in order to create a clean master data set that could be easily analyzed. To accomplish this, we performed the following actions:    
* Remove any unnecessary columns, such as extra indices.
* Removing non-numeric characters from columns with financial data so that those values could be operated upon as integers.
* Renaming columns by removing spaces to improve the ease by which this column could be operated upon using dot notation.
* Removing extreme outliers in financial data categories to prevent skewing averages

#### Feature Engineering
Based on the data available in our database we engineered the following features to improve our analysis:   
* Net Profits - Based on the difference between Budget and Worldwide Gross, which serves to indicate the profits generated after accounting for expenses.
* Return on Investment (ROI) - A ratio that compares the gain or loss from an investment relative to its cost (e.g. the amount earned relative to the amount spent)

### Part 2: Recommendations and Visualizations (Part_2_Recommendation_Report__with_Visualizations.ipynb)
Includes data analysis, visualizations, and recommendations justified by the data.

#### The Strategy
Based on information and insights provided by our database, we developed **The Winning Formula**, in order to create a systematic approach to project development that will increase the chances of movie success.

#### What is The Winning Formula?
The Winning Formula prescribes that Microsoft maximize profitability by perusing two different kinds of projects: Low-Risk/Lower-Reward projects and High-Risk/High-Reward projects. The Winning Formula provides a step-by-step guide to developing films in both categories based on the data. 


#### Summary of The Winning Formula   
#### These steps were developed based on the following questions:       
**Step One**     
*What kind of film should we make?*     
Choosing a genre and a production method    

**Step Two**    
*How much should we spend?*       
Determining an appropriate budget that will manage costs while maximizing returns   

**Step Three**     
*Who is winning in each category?*   
Discovering potential competition   

(Fig. 2.1.1)   
![df_heatmap](https://github.com/xinegan88/some_files/blob/master/heatmap.png)

### The Categories   
#### Slow-but-Steady
#### Low-Risk/Lower-Reward (Fig. 2.1.1)    
Low-risk/low-reward projects provide a solid foundation for studios to build revenue.   
* They have lower up-front costs (budget) and provide modest returns.     
* The actual net profits tend to be lower thatn high-risk/high-reward projects, however the ROI and profit margins are generally higher.     

Horror, Thriller/Suspense, Drama, and Comedy are the top genres in this category (Fig. 2.1.1)    

**These are the "bread and butter" movies that studios can produce in order to build wealth in a slow-but-steady way. Films like this allow a studios to become financially viable to allow for the persuit of high-risk/high-reward projects.**     

#### Go Big or Go Home!   
#### High-Risk/High-Reward (Fig. 2.2.1)
High-risk/high-reward projects projects generate smaller profit margins, but larger actual net profits.     
* These films are generally more expensive to create, and subsequently carry a larger financial risk.     
* When these movies are done right, they provide high-revenues which enrich the studios, while simultaneously earning the studio acclaim.    

(Fig 2.2.1)      
![df_heatmap](https://github.com/xinegan88/some_files/blob/master/genre_all_profit.png)

### The Recommendations
#### High-Risk/High-Reward
**What kind of movie should we make?**     
When choosing high-risk/high-reward projects, action and adventure moves that are live-action and superhero oriented do exetremely well.        
(Fig 2.2.4)      
![df_heatmap](https://github.com/xinegan88/some_files/blob/master/hr_ct.png)

**How much should we spend?**     
Historically, budgets below 2 billion dollars seem to be the safest, but there is more competition in that range.    
While there is little connection between an increase in spending an increase in ROI, actual returns sky-rocket as budgets increase.      
(Fig 2.3.1)    
![df_heatmap](https://github.com/xinegan88/some_files/blob/master/hr_budget_roi.png)

While there is little connection between an increase in spending an increase in ROI, actual returns sky-rocket as budgets increase.(Fig 2.3.2)    
![df_heatmap](https://github.com/xinegan88/some_files/blob/master/hr_budget_net.png)

**Who are we competing with?**     
Walt Disney seems to have mastered making a few high-risk films that earn a lot of money, especially when it comes to to actions movies that are live-action/animation hybrids centered around superheroes, or animated musicals.
![df_heatmap](https://github.com/xinegan88/some_files/blob/master/wd_net.png)

### Low-Risk/Low-Reward
**What kind of movie should we make?**     
When choosing low-risk/low-reward projects, live-action movies in horror, thriller-suspense, comedy, and drama are clear winners in ROI. (Fig 2.2.4)      
![df_heatmap](https://github.com/xinegan88/some_files/blob/master/lr_budget_roi.png)

**How much should we spend?**     
Historically, budgets below 75 million dollars seem to have good returns, but above that amount, ROI seems to tank. (Fig 2.3.3)     
While there is little connection between an increase in spending an increase in ROI, actual returns sky-rocket as budgets increase.         
(Fig 2.3.3)    
![df_heatmap](https://github.com/xinegan88/some_files/blob/master/hr_budget_roi.png)

**Who are we competing with?**
Warner Bros churns out a lot films, with an impressive net and ROI. (Fig. 2.4.1)    
They seem to have a clear advantage in comedy.  (Fig. 2.4.2)     
(Fig. 2.4.2)     
![df_heatmap](https://github.com/xinegan88/some_files/blob/master/wb_net.png)

#### How should the categories be divided?
(Fig. 2.4.1)     
![df_heatmap](https://github.com/xinegan88/the-winning-formula/blob/master/images/dist_roi_net.png)     

Among all of the studios, Universal seems to have mastered a balance of high-risk/high-reward films with low-risk/low-reward films. By examining Universal's genre breakdown, it seems to indicate that approximately 35% are high-risk projects, and 60% are low-risk projects with the remaining 5% being represented by other genres. Based on this, we recommend choosing 35% high-risk projects and 65% low-risk projects.      
(Fig. 2.4.4)     
![df_heatmap](https://github.com/xinegan88/some_files/blob/master/universal_net.png)

### Part 3: Additional Files 
a) A PDF of our presentation of The Winning Formula for non-technical stake-holders. (presentation.pdf)       
b) A copy of our master dataframe (master_df.csv)      
c) A folder of visualization images (/images)   
## Future Work   
Additional analysis can build upon the insights explored in this report. Some ideas for future work include:   

**1) Addressing Data Limitations**    
In the *Data Limitations* section above, we pointed out that there are additional costs and additional revenue that might improve the accuracy of this analysis. In the future, obtaining data related to this expanded set of financial factors can reveal a more nuanced projection of profitability. 

**2) What is the impact of “award-worthiness”?**   
Do award-winning films turn more profit?  
What is the ROI on winning a major award?  

**3) What is the best way to leverage the international market?**   
Is there ever justification to release only domestically?   
Are there opportunities for joint-ventures with international firms, similar to Netflix’s model?  

**4) How do successful film studios pivot into television?**    
Should we consider a separate television division?
Do these firms start with TV or with film?
