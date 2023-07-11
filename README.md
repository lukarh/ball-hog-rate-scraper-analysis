# nba-ball-hog-rate-analysis

### Motivation

In the modern NBA era, there often discussions that X player dominants the ball too much or a lot, Y player doesn't need the ball in his hands to be an effective scorer, or Z player needs to be on the ball more or off the ball more if V player comes in- the examples go on and on. Often times, these discussions are wrapped around mental estimates based on observations from players, however, we can actually calculate "ball-hog rate", or in other words, how often the player has the ball in their hands when they are on the floor, using publicly available data from various sources. The official stats.nba.com has insightful tracking data on how long a player has held the ball for (in minutes) by game and total. Except this data is quite meaningless if we can't normalize these rates to account for various playing time, role, and opportunity that each player is subjected to by game. Therefore, we have to source data from pbpstats.com to create meaningful insights with this tracking data. 

## Languages, Tools, and Libraries/Packages

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white) ![Atom](https://img.shields.io/badge/Atom-%2366595C.svg?style=for-the-badge&logo=atom&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![Selenium](https://img.shields.io/badge/-selenium-%43B02A?style=for-the-badge&logo=selenium&logoColor=white)

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

![westbrook_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/53a88a76-51b2-4c51-8120-c398c2d52071)

![curry_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/9adf6796-1ce7-447d-8178-1fcedd990704)

![cp3_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/be316a4f-118e-4994-bf21-b2f918251e5f)

![durant_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/d430de72-0168-4e7f-b3de-de4bb7984500)

![lebron_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/d1e72573-7fc1-4532-a129-15f01640f435)

![jokic_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/61fa718a-d8d6-425d-8c69-80f95c4899b0)

![irving_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/f0f4d3a8-d9e9-4949-86fe-6a6ffc3f0fd5)

![pg13_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/473c140e-0133-48ec-9e3f-99ec9357b61a)

![leonard_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/58479070-a754-410f-955d-0c32aa41fa69)

![butler_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/2f226247-5b5b-4e38-9769-67a0cf0b1262)

![lowry_rs_hog_progression_2013-23](https://github.com/lukarh/ball-hog-rate-analysis/assets/65103724/8ea4bec8-02d7-42b3-a1ce-43e88ee3ccd7)


