# fantasyFootball
ml for fantasy football draft.

Trained four XGB models for RB, QB, WR, TE using nfl_data_py data.
The process begins with data cleaning to remove non-active players,
removed 85% correlated feature,
each model has different features.
a wrapper like  feature selection on permutated feature sets,
Then I used 5-fold CV hyperparameter tuning, 10-fold CV validation.
The final model use 5 years data 2016, 2017, 2018, 2019, 2020 to predict 2021 fantasy score ppr.
The performance of the QB model MAE is around 4.66.
Future improved would include the rookie data, kicker model, and defense team model.