# nba-ball-hog-rate-analysis

### Motivation

In the modern NBA era, there often discussions that X player dominants the ball too much or a lot, Y player doesn't need the ball in his hands to be an effective scorer, or Z player needs to be on the ball more or off the ball more if V player comes in- the examples go on and on. Often times, these discussions are wrapped around mental estimates based on observations from players, however, we can actually calculate "ball-hog rate", or in other words, how often the player has the ball in their hands when they are on the floor, using publicly available data from various sources. The official stats.nba.com has insightful tracking data on how long a player has held the ball for (in minutes) by game and total. Except this data is quite meaningless if we can't normalize these rates to account for various playing time, role, and opportunity that each player is subjected to. Therefore, we have to source data from pbpstats.com to create meaningful insights with this data and get an accurate sense of ball-hog responsibility that each player has on each team. 

### How To Calculate Ball-Hog Rate

**Ball-Hog Rate:** The percent / proportion amount of time spent on offense with the ball in their hands when they are on the floor.

$BHR=\frac{T}{P\times A}=\frac{min\times\frac{60s}{min}}{possessions\times\frac{s}{possessions}}$

**$T$**: Total Time Spent with the Ball in their Hand (mins): provided by [stats.nba.com](https://www.nba.com/stats/players/touches?dir=D&sort=TIME_OF_POSS)

**$P$**: Total Number of Offensive Possessions Played (possessions): provided by [pbpstats.com](https://www.pbpstats.com/totals/nba/player?Season=2022-23&SeasonType=Regular%2BSeason)

**$A$**: Average Seconds Per Possession with x Player on the floor (seconds / possessions): provided by [pbpstats.com](https://www.pbpstats.com/on-off/nba/stat?Season=2022-23&SeasonType=Regular%2BSeason&TeamId=1610612737&Stat=SecondsPerPossOff)
