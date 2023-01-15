# Results from training (with 15 KFolds)
=========================================================

## Random Forests:
___________________________________________________________________________________________________________
18-12  11h33

Features:
    ["delay_in_seconds","avg_temperature","avg_atm_pressure","record_date_month","record_date_day","record_date_isWeekend","record_date_hour","N101","IC5","Affected_Count"]

HyperParameters:

{random_state=13032001,
 n_estimators=1822,
 criterion='entropy',
 max_features='auto',
 class_weight='balanced',
 max_depth= 40,
 min_samples_split=2,
 min_samples_leaf=1,
 n_jobs=-1,
 bootstrap= False}

Notes:
-> Now using magnitude of the delay to scale delay in seconds

Accuracy: 0.9408048767330205
Public: 0.95844

___________________________________________________________________________________________________________
18-12 11h45

Features:
    ["delay_in_seconds","avg_temperature","avg_atm_pressure","record_date_month","record_date_day","record_date_isWeekend","record_date_hour","N101","IC5","Affected_Count"]

HyperParameters:

{random_state=13032001,
 n_estimators=1777,
 criterion='entropy',
 max_features='auto',
 class_weight='balanced',
 max_depth= 34,
 min_samples_split=2,
 min_samples_leaf=1,
 n_jobs=-1,
 bootstrap= False}

Notes:
-> Now using magnitude of the delay to scale delay in seconds

Accuracy: 0.9410044775314237
Public: 0.95844



___________________________________________________________________________________________________________
18-12 11h56

Features:
    ["delay_in_seconds","avg_temperature","avg_atm_pressure","dayYear","record_date_isWeekend","record_date_hour","N101","IC5","Affected_Count"]

HyperParameters:

{random_state=13032001,
 n_estimators=1777,
 criterion='entropy',
 max_features='auto',
 class_weight='balanced',
 max_depth= 34,
 min_samples_split=2,
 min_samples_leaf=1,
 n_jobs=-1,
 bootstrap= False}

Notes:
-> Now using magnitude of the delay to scale delay in seconds

0.9410074745404086
Public: 0.95844

_____________________________________________________________________________________________________________

Features: 
["delay_in_seconds","avg_temperature","avg_atm_pressure","record_date_month","dayYear","record_date_isWeekend","record_date_hour","N101","IC5","Affected_Count"]


HyperParameters:

{random_state=13032001,
 n_estimators=1777,
 criterion='entropy',
 max_features='auto',
 class_weight='balanced',
 max_depth= 34,
 min_samples_split=2,
 min_samples_leaf=1,
 n_jobs=-1,
 bootstrap= False}

0.942
0.914

_____________________________________________________________________________________________________________
Features:
["delay_in_seconds","avg_temperature","avg_atm_pressure","record_date_month","record_date_day","dayYear","record_date_isWeekend","record_date_hour","N101","IC5","Affected_Count"]

HyperParameters:

{random_state=13032001,
 n_estimators=1777,
 criterion='entropy',
 max_features='auto',
 class_weight='balanced',
 max_depth= 34,
 min_samples_split=2,
 min_samples_leaf=1,
 n_jobs=-1,
 bootstrap= False}

-> Without delay treat
0.9427999999999999
0.96398

_____________________________________________________________________________________________________________
Features:
["delay_in_seconds","avg_temperature","avg_atm_pressure","record_date_month","record_date_day","dayYear","record_date_isWeekend","record_date_hour","N101","IC5","Affected_Count"]

HyperParameters:

{random_state=13032001,
 n_estimators=1777,
 criterion='entropy',
 max_features='auto',
 class_weight='balanced',
 max_depth= 34,
 min_samples_split=2,
 min_samples_leaf=1,
 n_jobs=-1,
 bootstrap= False}

-> With delay treat
0.940
0.97783


_____________________________________________________________________________________________________________
Features:
[["delay_in_seconds","avg_atm_pressure","record_date_month","record_date_day","dayYear","record_date_isWeekend","record_date_hour","N101","Affected_Count"]]

HyperParameters:

    return RandomForestClassifier(random_state=13122001,
                            n_estimators=1800,
                            criterion='entropy',
                            max_features='auto',
                            class_weight='balanced',
                            max_depth= 40,
                            min_samples_split=3,
                            min_samples_leaf=1,
                            n_jobs=-1,
                            bootstrap= False)

-> With delay treat
0.9442
96.67