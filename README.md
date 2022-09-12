# fantasyFootball
ml for fantasy football draft.


* The final model use 5 years data 2016, 2017, 2018, 2019, 2020 to predict 2021 fantasy score ppr.
* The process begins with data cleaning to remove non-active or injured player matches.
* Each model RB, QB, WR, TE has different features. I removed 85% correlated feature.
* I used a wrapper like  feature selection on permutated feature sets.
* Then I used 5-fold CV hyperparameter tuning, 10-fold CV validation.
* The performance of the QB model MAE is around 4.66.
* Find the highest median prediction as ranking.  This ensures good performance and take into account of outliers.
* Then matches to current year 2022 player matches. Ignore players that changed teams because situation changes.  
* Did not use rookie data, kicker data, and defense team data.  Those data are not available in this data.  It could be included in the future.