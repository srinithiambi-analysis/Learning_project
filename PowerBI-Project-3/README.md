What Makes a Book Commercially Successful?
Power BI Dashboard Project | MBA Business Analytics

The Question I Wanted to Answer
As someone who loves books, I always wondered —
why do some books sell thousands of copies while others don't?
Is it the genre? The author's reputation? The publisher? The price?
This project uses a dataset of 1,041 books to find out.

The Dataset

Source: Kaggle — Books Data Clean
1,041 books after cleaning
Time period: 570 AD to 2015
Key columns used: Genre, Author Rating, Publisher, Units Sold, Gross Sales, Avg Rating, Sale Price, Publishing Year


How I Worked Through It
I followed a 3 stage process:
Stage 1 — Clean the Data
Before any analysis, I had to fix the data.
Problems I found:
ProblemRows affectedWhat I didBlank book names23Removed — unusable for analysisNegative publishing years5Removed — impossible valuesZero publisher revenue despite valid sales372Excluded column — data pipeline error confirmedBlank language values53Replaced with "Unknown"Columns stored as text instead of numbers8 columnsFixed data types in Power Query
What I learned here: 60–70% of real analyst work is cleaning and understanding data before touching any chart.

Stage 2 — Explore the Data
Before building the dashboard I used pivot tables in Excel to find patterns.
What I checked:

Which genre has the highest ratings and sales?
Do famous authors actually sell more than intermediate ones?
Which publisher makes the most money?
Does a higher price mean more reader engagement?
Has the reading market grown over the years?

Two honest limitations I found:

Genre Fiction makes up 77% of the dataset — genre comparisons are not fully fair
Only 30 books (3%) are by Novice authors — not enough data to advise brand new authors reliably


Stage 3 — Build the Dashboard
VisualWhat it showsKPI cardsTotal units sold · Gross sales · Avg ratingBar chartGenre vs average ratingColumn chartAuthor rating vs units soldHorizontal barTop 10 books by units soldScatter plotPublisher — units sold vs gross salesScatter plot + trend lineSale price vs book ratings countLine chartUnits sold trend by publishing year

What I Found
Finding 1 — You don't need to be famous to sell
9 out of 10 top selling books were written by Excellent or Intermediate authors.
One Novice author — Jane Green — sold 61,128 units and ranked in the top 3.
Famous authors do not appear in the top 10 at all.
So what? Reputation alone does not decide commercial success. Quality matters more than fame.


Finding 2 — Pick your publisher based on your goal
PublisherUnits SoldStrategyAmazon Digital Services6M+High volume, low price — best for reachPenguin Group USA918KLower volume, premium price — best for income per book
So what? If you want a large audience go Amazon. If you want higher income per book go Penguin.


Finding 3 — The reading market is growing not shrinking
Book sales were flat for centuries then spiked sharply after 2000.
The biggest peak was 2011–2013 — when social media became mainstream.
So what? It is the best time in history to be a new author. The audience is bigger than ever.


Finding 4 — Price does not affect reader engagement
Books at $0.99 and books at $12.99 get similar ratings counts.
The trend line on the scatter plot is nearly flat — confirming no relationship.
So what? Don't underprice your book out of fear of losing readers. Price it based on your publisher's strategy.


Finding 5 — Fiction gives you the biggest audience
Despite the data imbalance, Fiction consistently attracts the highest reader engagement and ratings.
So what? For an emerging author, Fiction gives you the largest existing audience to write for.
