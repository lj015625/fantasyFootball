# fantasyFootball
ml for fantasy football draft.


* The final model use 5 years data 2016, 2017, 2018, 2019, 2020 to predict 2021 fantasy score ppr. The idea is to get stable good performance at each week.
* The process begins with data cleaning to remove non-active or injured player matches.
* Each model RB, QB, WR, TE have different sets of features. I removed 85% correlated feature.
* I used a wrapper like  feature selection on permutated feature sets.
* Then I used 5-fold CV hyperparameter tuning, 10-fold CV validation.
* The performance of the QB model MAE is around 4.66.
* Find the highest median prediction as ranking.  This ensures good performance and not affected by outliers performance.
* Then matches to current year 2022 player matches. Ignore players that changed teams because situation changes.  
* Did not use rookie data, kicker data, and defense team data.  Those data are not available in this data. But it could be included in the future.
* Another future idea is to train a model to predict injuries or inactive status and take that into considerations.  Since injuries really would affect weekly matchup.