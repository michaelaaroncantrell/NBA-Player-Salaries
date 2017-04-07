# NBA-Player-Salaries
This repository contains the presentations and notebooks for my second Metis project, using linear regression to analyze NBA player salaries. In get_2016_data.ipynb I use BeautifulSoup to scrape [http://www.basketball-reference.com](http://www.basketball-reference.com) for player salaries and performance statistics. Then, in regression.ipynb, I build several linear regression models with and without regularization. 

My most surprising finding was that, once you restrict to features that player's can actually improve, the most correlated feature with salary is defensive rebounds.

![Defensive Rebounds](https://github.com/michaelaaroncantrell/NBA-Player-Salaries/blob/master/images/DRB-scatter.png)

In fact, defensive rebounds are much more correlated with salary than 3 Point Percentage.

![Three Point Percentage](https://github.com/michaelaaroncantrell/NBA-Player-Salaries/blob/master/images/3PP-scatter.png)

Also interesting was how the distribution of salaries on a given team compared to the NBA's total distribution. For example, the Philadelphia 76ers are all paid very poorly compared to their peers, while the Houston Rockets have no middle class.

![Salary by Team](https://github.com/michaelaaroncantrell/NBA-Player-Salaries/blob/master/images/salary-by-team.png)

Of course my models didn't account for all of the variance in player salary, with most models accounting for about half (R-squared about 0.5). Interestingly enough, taking a look at the players that my model predicted were most over and underpaid, CJ McCollum, the player my model indicated was most *under paid* actually won the most improved player of the year award in 2016, and his salary went up 700% the following year, to approximately what my model predicted he deserved.

![Most Underpaid Players](https://github.com/michaelaaroncantrell/NBA-Player-Salaries/blob/master/images/signif-underpaid.png)