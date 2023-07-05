# nba-ball-hog-rate-analysis

### Motivation

In the modern NBA era, there often discussions that X player dominants the ball too much or a lot, Y player doesn't need the ball in his hands to be an effective scorer, or Z player needs to be on the ball more or off the ball more if V player comes in- the examples go on and on. Often times, these discussions are wrapped around mental estimates based on observations from players, however, we can actually calculate "ball-hog rate", or in other words, how often the player has the ball in their hands when they are on the floor, using publicly available data from various sources. The official stats.nba.com has insightful tracking data on how long a player has held the ball for (in minutes) by game and total. Except this data is quite meaningless if we can't normalize these rates to account for various playing time, role, and opportunity that each player is subjected to by game. Therefore, we have to source data from pbpstats.com to create meaningful insights with this tracking data. 

### How To Calculate Ball-Hog Rate

**Ball-Hog Rate:** The percent / proportion amount of time spent on offense with the ball in their hands when they are on the floor.

$BHR=\frac{T}{P\times A}=\frac{min\times\frac{60s}{min}}{possessions\times\frac{s}{possessions}}$

**$T$**: Total Time Spent with the Ball in their Hand (mins): provided by [stats.nba.com](https://www.nba.com/stats/players/touches?dir=D&sort=TIME_OF_POSS)

**$P$**: Total Number of Offensive Possessions Played (possessions): provided by [pbpstats.com](https://www.pbpstats.com/totals/nba/player?Season=2022-23&SeasonType=Regular%2BSeason)

**$A$**: Average Seconds Per Possession with x Player on the floor (seconds / possessions): provided by [pbpstats.com](https://www.pbpstats.com/on-off/nba/stat?Season=2022-23&SeasonType=Regular%2BSeason&TeamId=1610612737&Stat=SecondsPerPossOff)

### Ball-Hog Rate Analysis

#### How Teams Divide the Ball-Handling Responsibilities amongst their starters:

![2022-23_ball_hog_rates_by_team](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/0b0fc317-b9a3-4164-ba3f-646f097b9839)

#### Ball-Dominant Guards used to dominate the league in the early modern tracking era, but you have to be REALLY good to demand that type of responsibility

![image](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/a139011c-a5b1-4728-8994-ea6b67031e8a)

#### How Star Players have seen their Ball-Handling Responsibilities change over the years:

![lebron_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/05e07489-f01f-4633-b8bf-c538ab0c9361)

![westbrook_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/e9ad424b-dce3-4c98-8bb3-b384af8a4824)

![curry_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/56950eeb-ae10-4449-b194-6f39756cc515)

![durant_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/b9829cae-8e97-4a80-aa57-4292029f700e)

![pg13_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/10e782be-31b1-4cbe-8587-a6339a6e915d)

![jokic_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/2c1cf4c6-4e44-48cc-9527-b54e321683f3)

![irving_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/e7d1a122-f2b4-426f-921e-9299ba67e3d8)

