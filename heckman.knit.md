---
title: "Heckman Selection Model Analysis"
output: html_document
---




```
## 
## 
## ==================================================================================================== 
## ANALYZING DATASET 1/8: Offense Grades
## ==================================================================================================== 
## 
## Reading data: processed_predict_ccafd_off_grades.csv.csv.gz
## Reading data: processed_predict_ccfd_off_grades.csv.csv.gz
## 
## Phase 1: Validation Phase
## 
## Running 2 test iterations with best parameters...
## 
## Test Results over 2 iterations:
## Mean AUC: 0.8838176 
## SD AUC: 0.002146579 
## 95% CI: 0.8796103 to 0.8880249 
## 
## 
##  ================================================================================ 
## MODEL: Player Model with GIMR 
## ================================================================================ 
## 
## 
## Player Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.4399       3.5395    ***
## ydstogo                             -0.1115     -12.6779    ***
## posteam_timeouts_remaining           0.0124       1.3550       
## defteam_timeouts_remaining           0.0093       1.0414       
## rush_attempt                         0.1562       7.9594    ***
## week                                 0.0072       0.7223       
## temp                                -0.0091      -0.8632       
## wind                                 0.0109       1.0434       
## vegas_wp                             0.0182       1.6255      .
## spread_line                         -0.0026      -0.2090       
## total_line                           0.0267       2.1229     **
## prep_days                            0.0070       0.8980       
## overall_win_pct                      0.0076       0.5749       
## team_win_pct                         0.0160       1.1138       
## prev_win_pct                        -0.0348      -2.7477    ***
## prev_shotgun_rate                    0.0116       0.5300       
## prev_singleback_rate                 0.0100       0.6057       
## prev_empty_rate                      0.0094       0.7748       
## prev_iform_rate                      0.0031       0.2015       
## prev_shotgun_success                 0.0054       0.4595       
## prev_singleback_success              0.0078       0.6581       
## prev_empty_success                   0.0054       0.4880       
## prev_iform_success                   0.0223       2.2229     **
## prev_stop_rate_run                   0.0004       0.0371       
## prev_stop_rate_pass                 -0.0339      -3.2954    ***
## shotgun_rate                         0.0180       1.3129       
## singleback_rate                      0.0062       0.5201       
## empty_rate                          -0.0009      -0.0769       
## iform_rate                          -0.0167      -1.5848      .
## shotgun_success                     -0.0195      -2.1881     **
## singleback_success                  -0.0078      -0.8417       
## empty_success                       -0.0068      -0.7018       
## iform_success                       -0.0125      -1.3051       
## def_stop_rate_run                    0.0161       1.7245      *
## def_stop_rate_pass                  -0.0103      -1.0914       
## avg_pass_rushers                    -0.0104      -0.9335       
## avg_box_defenders                   -0.0067      -0.6332       
## cover0_rate                          0.0014       0.1194       
## cover1_rate                         -0.0099      -0.5550       
## cover2_rate                         -0.0051      -0.3836       
## cover3_rate                          0.0264       1.4483      .
## cover4_rate                          0.0144       1.0701       
## cover6_rate                         -0.0062      -0.5132       
## two_man_rate                         0.0143       1.5258      .
## prevent_rate                         0.0213       2.6500    ***
## roof_outdoors                       -0.0114      -0.4726       
## posteam_type_home                   -0.0202      -1.2888       
## QB_short_grades_pass_12w             0.0339       2.4529     **
## QB_medium_grades_pass_12w           -0.0042      -0.3010       
## QB_deep_grades_pass_12w             -0.0197      -1.5593      .
## RB_grades_pass_block_12w             0.0128       1.4673      .
## RB_grades_run_12w                    0.0011       0.0787       
## RB_grades_pass_route_12w            -0.0040      -0.2936       
## WR1_short_grades_pass_route_12w      -0.0079      -0.5890       
## WR1_medium_grades_pass_route_12w      -0.0060      -0.4635       
## WR1_deep_grades_pass_route_12w       0.0037       0.3227       
## WR2_short_grades_pass_route_12w      -0.0040      -0.2105       
## WR2_medium_grades_pass_route_12w      -0.0053      -0.2840       
## WR2_deep_grades_pass_route_12w       0.0078       0.5094       
## WR3_short_grades_pass_route_12w      -0.0045      -0.2600       
## WR3_medium_grades_pass_route_12w       0.0094       0.5403       
## WR3_deep_grades_pass_route_12w       0.0144       0.9876       
## TE1_short_grades_pass_route_12w       0.0055       0.5427       
## TE1_medium_grades_pass_route_12w       0.0186       1.8414      *
## TE1_deep_grades_pass_route_12w      -0.0143      -1.6067      .
## DL1_grades_defense_12w              -0.0172      -2.1254     **
## DL2_grades_defense_12w               0.0039       0.4471       
## DL3_grades_defense_12w               0.0127       1.0929       
## DL4_grades_defense_12w              -0.0285      -2.3687     **
## LB1_grades_defense_12w               0.0048       0.5706       
## LB2_grades_defense_12w               0.0027       0.3099       
## LB3_grades_defense_12w              -0.0139      -1.1689       
## LB4_grades_defense_12w              -0.0011      -0.0998       
## CB1_grades_defense_12w              -0.0142      -1.5956      .
## CB2_grades_defense_12w              -0.0060      -0.6460       
## CB3_grades_defense_12w               0.0147       1.3815       
## S1_grades_defense_12w               -0.0066      -0.8504       
## S2_grades_defense_12w                0.0045       0.5105       
## S3_grades_defense_12w                0.0081       0.8472       
## OL_grades_pass_block_12w            -0.0030      -0.2811       
## OL_grades_run_block_12w             -0.0041      -0.4022       
## yardline_1_10                       -0.0625      -2.3498     **
## yardline_11_20                       0.0130       0.4466       
## yardline_21_30                       0.0039       0.1398       
## yardline_41_50                       0.0495       2.0484     **
## yardline_51_60                       0.0185       0.6385       
## yardline_61_70                       0.0480       1.4908      .
## yardline_71_80                       0.0735       1.8442      *
## yardline_81_90                       0.1392       2.3299     **
## yardline_91_100                      0.1134       1.0925       
## year2017_team_ARI                    0.0564       0.3030       
## year2017_team_BUF                   -0.1229      -0.6283       
## year2017_team_CHI                    0.0012       0.0072       
## year2017_team_CLE                    0.1487       0.7488       
## year2017_team_DAL                   -0.1654      -0.9753       
## year2017_team_DET                   -0.0912      -0.5270       
## year2017_team_GB                     0.3301       2.0127     **
## year2017_team_HOU                    0.3377       1.6364      .
## year2017_team_MIA                   -0.2348      -1.3342       
## year2017_team_MIN                   -0.1261      -0.7052       
## year2017_team_NE                    -0.0196      -0.1077       
## year2017_team_SF                     0.3947       1.9953     **
## year2017_team_BAL                   -0.0070      -0.0364       
## year2017_team_DEN                   -0.0234      -0.1287       
## year2017_team_LA                     0.0560       0.3072       
## year2017_team_NYG                   -0.0705      -0.4158       
## year2017_team_OAK                   -0.1024      -0.5705       
## year2017_team_SEA                    0.1234       0.6578       
## year2017_team_CAR                    0.1152       0.5374       
## year2017_team_CIN                    0.1409       0.6969       
## year2017_team_IND                    0.1516       0.8385       
## year2017_team_NO                     0.1143       0.5160       
## year2017_team_PHI                    0.0345       0.1938       
## year2017_team_PIT                   -0.1502      -0.8878       
## year2017_team_TEN                    0.0528       0.2451       
## year2017_team_WAS                    0.0419       0.2158       
## year2017_team_KC                     0.2906       1.5236      .
## year2017_team_LAC                    0.0133       0.0709       
## year2017_team_NYJ                    0.1588       0.7481       
## year2017_team_TB                     0.0450       0.1933       
## year2017_team_ATL                   -0.0123      -0.0636       
## year2017_team_JAX                    0.0851       0.4230       
## year2018_team_ARI                    0.0989       0.6778       
## year2018_team_BAL                    0.0603       0.4125       
## year2018_team_CAR                    0.0535       0.3640       
## year2018_team_CLE                   -0.0468      -0.3347       
## year2018_team_DET                    0.1209       0.8694       
## year2018_team_HOU                    0.2442       1.4881      .
## year2018_team_IND                   -0.1014      -0.7599       
## year2018_team_KC                     0.1153       0.8447       
## year2018_team_NYG                    0.1083       0.6308       
## year2018_team_OAK                   -0.1412      -0.8481       
## year2018_team_PHI                    0.0993       0.6804       
## year2018_team_SEA                   -0.0774      -0.4434       
## year2018_team_BUF                   -0.0917      -0.5659       
## year2018_team_CHI                    0.0049       0.0382       
## year2018_team_CIN                   -0.0443      -0.2695       
## year2018_team_DAL                   -0.0401      -0.2725       
## year2018_team_DEN                    0.0446       0.3080       
## year2018_team_GB                     0.0055       0.0322       
## year2018_team_LAC                    0.0336       0.2288       
## year2018_team_NE                    -0.0886      -0.5570       
## year2018_team_NO                     0.0990       0.7258       
## year2018_team_PIT                    0.0980       0.5389       
## year2018_team_SF                     0.0334       0.2298       
## year2018_team_MIA                    0.0802       0.5684       
## year2018_team_MIN                    0.0283       0.1784       
## year2018_team_NYJ                    0.1708       0.7706       
## year2018_team_TB                     0.0418       0.2515       
## year2018_team_ATL                    0.0728       0.5314       
## year2018_team_JAX                    0.0640       0.4205       
## year2018_team_LA                    -0.1588      -1.0152       
## year2018_team_TEN                    0.1483       0.9410       
## year2018_team_WAS                    0.0177       0.0885       
## year2019_team_ARI                   -0.0965      -0.6119       
## year2019_team_BUF                   -0.1329      -1.0499       
## year2019_team_CHI                    0.0571       0.3900       
## year2019_team_CLE                    0.0997       0.6722       
## year2019_team_DAL                   -0.0386      -0.2351       
## year2019_team_IND                   -0.0675      -0.5173       
## year2019_team_JAX                    0.0917       0.6073       
## year2019_team_KC                    -0.0149      -0.1104       
## year2019_team_LAC                   -0.1038      -0.7139       
## year2019_team_MIN                   -0.0748      -0.5214       
## year2019_team_NE                    -0.0378      -0.2272       
## year2019_team_NO                    -0.1967      -1.2970       
## year2019_team_PHI                    0.0665       0.4517       
## year2019_team_SEA                    0.0260       0.1350       
## year2019_team_SF                    -0.0102      -0.0772       
## year2019_team_TB                    -0.1407      -0.9972       
## year2019_team_BAL                    0.0150       0.1058       
## year2019_team_CAR                   -0.0853      -0.5249       
## year2019_team_DEN                    0.1109       0.7856       
## year2019_team_DET                   -0.1101      -0.7118       
## year2019_team_HOU                    0.0055       0.0364       
## year2019_team_LA                    -0.1060      -0.6674       
## year2019_team_MIA                   -0.3035      -1.9469      *
## year2019_team_NYG                   -0.1533      -0.9524       
## year2019_team_NYJ                   -0.2327      -1.8071      *
## year2019_team_OAK                   -0.0545      -0.3612       
## year2019_team_PIT                   -0.3000      -2.4507     **
## year2019_team_TEN                   -0.1842      -1.3358       
## year2019_team_CIN                    0.0549       0.3929       
## year2019_team_WAS                   -0.0651      -0.4349       
## year2019_team_ATL                    0.0111       0.0718       
## year2019_team_GB                    -0.0588      -0.3977       
## year2020_team_ATL                    0.0509       0.3322       
## year2020_team_BAL                    0.0597       0.3887       
## year2020_team_BUF                   -0.0232      -0.1279       
## year2020_team_CAR                    0.1131       0.6991       
## year2020_team_CIN                    0.0662       0.4456       
## year2020_team_DEN                   -0.0958      -0.5723       
## year2020_team_DET                   -0.1589      -1.0271       
## year2020_team_JAX                   -0.1487      -0.9344       
## year2020_team_KC                     0.0465       0.2860       
## year2020_team_LA                    -0.2008      -1.1547       
## year2020_team_MIN                    0.1554       1.0995       
## year2020_team_NE                    -0.0461      -0.2956       
## year2020_team_NO                     0.0242       0.1675       
## year2020_team_NYG                    0.0157       0.1050       
## year2020_team_SF                     0.0799       0.4788       
## year2020_team_WAS                    0.0188       0.1304       
## year2020_team_CHI                    0.0233       0.1470       
## year2020_team_DAL                   -0.0461      -0.3069       
## year2020_team_GB                    -0.0439      -0.2532       
## year2020_team_HOU                   -0.1094      -0.6883       
## year2020_team_MIA                   -0.1779      -1.1094       
## year2020_team_NYJ                   -0.0132      -0.0777       
## year2020_team_TB                     0.0324       0.2030       
## year2020_team_TEN                   -0.1112      -0.6768       
## year2020_team_ARI                    0.0746       0.4441       
## year2020_team_CLE                   -0.2570      -1.4966      .
## year2020_team_IND                   -0.1465      -0.8937       
## year2020_team_LAC                   -0.0003      -0.0017       
## year2020_team_PHI                    0.0933       0.6394       
## year2020_team_SEA                   -0.0427      -0.2602       
## year2020_team_LV                     0.0940       0.6104       
## year2020_team_PIT                   -0.1102      -0.6774       
## year2021_team_ATL                   -0.2258      -1.7824      *
## year2021_team_BUF                    0.0441       0.3543       
## year2021_team_CIN                   -0.2442      -1.9909     **
## year2021_team_DAL                   -0.1022      -0.7261       
## year2021_team_DEN                    0.0444       0.3299       
## year2021_team_DET                   -0.0921      -0.6853       
## year2021_team_KC                     0.0113       0.0901       
## year2021_team_LA                     0.0010       0.0071       
## year2021_team_LV                     0.0332       0.2272       
## year2021_team_MIN                   -0.0372      -0.2886       
## year2021_team_NE                     0.0410       0.3028       
## year2021_team_NO                    -0.0156      -0.1165       
## year2021_team_NYG                   -0.0154      -0.1180       
## year2021_team_SF                    -0.0156      -0.1130       
## year2021_team_TEN                   -0.0821      -0.6786       
## year2021_team_ARI                    0.0820       0.6931       
## year2021_team_BAL                    0.1186       0.6723       
## year2021_team_CAR                   -0.0781      -0.6666       
## year2021_team_CHI                   -0.2285      -1.8501      *
## year2021_team_GB                     0.0887       0.7217       
## year2021_team_IND                   -0.0321      -0.2443       
## year2021_team_LAC                    0.0223       0.1563       
## year2021_team_MIA                    0.0174       0.1145       
## year2021_team_NYJ                   -0.0340      -0.2362       
## year2021_team_PHI                   -0.1833      -1.4385       
## year2021_team_SEA                   -0.2114      -1.4375       
## year2021_team_TB                     0.0357       0.2535       
## year2021_team_WAS                   -0.0728      -0.5950       
## year2021_team_CLE                   -0.1178      -0.9444       
## year2021_team_HOU                   -0.0974      -0.6756       
## year2021_team_JAX                   -0.0512      -0.3532       
## year2021_team_PIT                    0.0364       0.2726       
## year2022_team_ARI                   -0.1534      -1.1832       
## year2022_team_ATL                   -0.2642      -2.0351     **
## year2022_team_CAR                    0.1324       0.9148       
## year2022_team_CHI                   -0.0929      -0.5816       
## year2022_team_CIN                   -0.1352      -0.9047       
## year2022_team_HOU                   -0.0486      -0.3531       
## year2022_team_IND                   -0.1166      -0.8735       
## year2022_team_LAC                   -0.0917      -0.6883       
## year2022_team_MIA                   -0.1832      -1.5031      .
## year2022_team_SEA                   -0.0532      -0.4026       
## year2022_team_TB                     0.0254       0.1991       
## year2022_team_TEN                    0.1499       1.2946       
## year2022_team_WAS                   -0.0201      -0.1557       
## year2022_team_BAL                   -0.2035      -1.4296       
## year2022_team_BUF                    0.0263       0.2070       
## year2022_team_DAL                   -0.0010      -0.0059       
## year2022_team_DET                   -0.0921      -0.7409       
## year2022_team_GB                    -0.1495      -1.0673       
## year2022_team_JAX                   -0.1411      -1.2510       
## year2022_team_KC                    -0.1430      -0.8654       
## year2022_team_LA                     0.1575       1.2017       
## year2022_team_LV                     0.1400       0.9699       
## year2022_team_NO                    -0.0594      -0.3924       
## year2022_team_PHI                    0.0366       0.2873       
## year2022_team_PIT                    0.1887       1.5025      .
## year2022_team_DEN                    0.0228       0.1893       
## year2022_team_MIN                   -0.1191      -0.7765       
## year2022_team_NE                     0.0061       0.0426       
## year2022_team_NYJ                   -0.1136      -0.8887       
## year2022_team_NYG                   -0.0826      -0.5706       
## year2022_team_SF                    -0.1838      -1.0541       
## year2023_team_BAL                   -0.0587      -0.4518       
## year2023_team_CHI                   -0.1661      -1.2154       
## year2023_team_CLE                   -0.1143      -0.7697       
## year2023_team_GB                     0.0239       0.1787       
## year2023_team_IND                    0.0687       0.5496       
## year2023_team_KC                     0.0286       0.2059       
## year2023_team_LAC                    0.0462       0.3313       
## year2023_team_LV                     0.0114       0.0899       
## year2023_team_MIA                    0.0590       0.4442       
## year2023_team_MIN                    0.1232       1.0281       
## year2023_team_NO                    -0.0499      -0.3616       
## year2023_team_NYG                    0.0097       0.0718       
## year2023_team_SEA                   -0.2727      -2.2558     **
## year2023_team_SF                     0.0398       0.2616       
## year2023_team_WAS                    0.1782       1.4333       
## year2023_team_ATL                   -0.1079      -0.7468       
## year2023_team_BUF                   -0.1086      -0.7394       
## year2023_team_CAR                    0.0378       0.3030       
## year2023_team_DAL                    0.0996       0.7191       
## year2023_team_DEN                    0.0071       0.0551       
## year2023_team_HOU                   -0.0497      -0.3193       
## year2023_team_LA                    -0.0152      -0.1037       
## year2023_team_NE                     0.0269       0.2029       
## year2023_team_PHI                   -0.0473      -0.3628       
## year2023_team_PIT                   -0.0037      -0.0236       
## year2023_team_TEN                   -0.0051      -0.0351       
## year2023_team_ARI                   -0.1903      -1.3648       
## year2023_team_CIN                   -0.1728      -1.1227       
## year2023_team_DET                    0.0337       0.2744       
## year2023_team_TB                     0.0818       0.6036       
## year2023_team_JAX                   -0.0844      -0.5705       
## year2023_team_NYJ                    0.1791       1.3160       
## is_first_half                       -0.0123      -0.6890       
## time_in_half                         0.0161       1.6370      .
## home_attendance                     -0.0351      -0.4710       
## GIMR                                 0.0571       2.2735     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.112072 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.39
## prev_singleback_rate                                   5.37
## cover1_rate                                            6.05
## cover3_rate                                            6.39
## WR2_short_grades_pass_route_12w                        7.52
## WR2_medium_grades_pass_route_12w                       7.06
## WR3_short_grades_pass_route_12w                        5.91
## WR3_medium_grades_pass_route_12w                       5.92
## home_attendance                                       13.68
## 
## 
##  ================================================================================ 
## MODEL: Starter Model with GIMR 
## ================================================================================ 
## 
## 
## Starter Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.4205       3.3632    ***
## ydstogo                             -0.1098     -12.7893    ***
## posteam_timeouts_remaining           0.0093       1.0155       
## defteam_timeouts_remaining           0.0088       0.9902       
## rush_attempt                         0.1396       7.3735    ***
## week                                 0.0082       0.8126       
## temp                                -0.0069      -0.6555       
## wind                                 0.0074       0.6941       
## vegas_wp                             0.0106       0.9654       
## spread_line                         -0.0085      -0.6838       
## total_line                           0.0315       2.3706     **
## prep_days                            0.0075       0.9606       
## overall_win_pct                      0.0010       0.0742       
## team_win_pct                         0.0208       1.4510      .
## prev_win_pct                        -0.0290      -2.2769     **
## prev_shotgun_rate                   -0.0023      -0.1046       
## prev_singleback_rate                 0.0051       0.3065       
## prev_empty_rate                      0.0095       0.7764       
## prev_iform_rate                     -0.0007      -0.0465       
## prev_shotgun_success                 0.0054       0.4538       
## prev_singleback_success              0.0004       0.0317       
## prev_empty_success                  -0.0019      -0.1684       
## prev_iform_success                   0.0339       3.3353    ***
## prev_stop_rate_run                  -0.0016      -0.1426       
## prev_stop_rate_pass                 -0.0337      -3.3159    ***
## shotgun_rate                         0.0174       1.2578       
## singleback_rate                      0.0079       0.6560       
## empty_rate                           0.0011       0.0956       
## iform_rate                          -0.0148      -1.4011       
## shotgun_success                     -0.0200      -2.2045     **
## singleback_success                  -0.0106      -1.1358       
## empty_success                       -0.0090      -0.9178       
## iform_success                       -0.0116      -1.1950       
## def_stop_rate_run                    0.0150       1.5907      .
## def_stop_rate_pass                  -0.0124      -1.3017       
## avg_pass_rushers                    -0.0114      -1.0267       
## avg_box_defenders                   -0.0042      -0.4062       
## cover0_rate                         -0.0060      -0.5300       
## cover1_rate                         -0.0036      -0.2033       
## cover2_rate                         -0.0013      -0.0982       
## cover3_rate                          0.0219       1.1968       
## cover4_rate                          0.0136       1.0113       
## cover6_rate                         -0.0070      -0.5783       
## two_man_rate                         0.0156       1.6512      *
## prevent_rate                         0.0226       2.7871    ***
## roof_outdoors                       -0.0003      -0.0132       
## posteam_type_home                   -0.0266      -1.6830      *
## starter_QB_short_grades_pass_12w       0.0303       2.0168     **
## starter_QB_medium_grades_pass_12w      -0.0163      -1.2582       
## starter_QB_deep_grades_pass_12w      -0.0104      -0.8570       
## starter_RB_grades_pass_block_12w      -0.0204      -2.2076     **
## starter_RB_grades_run_12w           -0.0006      -0.0354       
## starter_RB_grades_pass_route_12w       0.0110       0.6420       
## starter_WR1_short_grades_pass_route_12w       0.0033       0.2567       
## starter_WR1_medium_grades_pass_route_12w       0.0183       1.5077      .
## starter_WR1_deep_grades_pass_route_12w       0.0034       0.3147       
## starter_WR2_short_grades_pass_route_12w      -0.0140      -1.2045       
## starter_WR2_medium_grades_pass_route_12w       0.0104       0.9500       
## starter_WR2_deep_grades_pass_route_12w       0.0043       0.4094       
## starter_WR3_short_grades_pass_route_12w      -0.0163      -1.5355      .
## starter_WR3_medium_grades_pass_route_12w       0.0070       0.7074       
## starter_WR3_deep_grades_pass_route_12w       0.0039       0.4102       
## starter_TE1_short_grades_pass_route_12w       0.0067       0.6136       
## starter_TE1_medium_grades_pass_route_12w      -0.0192      -1.9057      *
## starter_TE1_deep_grades_pass_route_12w       0.0001       0.0074       
## starter_DL1_grades_defense_12w       0.0024       0.2057       
## starter_DL2_grades_defense_12w       0.0122       1.0478       
## starter_DL3_grades_defense_12w      -0.0033      -0.2864       
## starter_DL4_grades_defense_12w       0.0040       0.4154       
## starter_LB1_grades_defense_12w       0.0029       0.2570       
## starter_LB2_grades_defense_12w       0.0185       1.6244      .
## starter_LB3_grades_defense_12w       0.0110       1.1152       
## starter_LB4_grades_defense_12w      -0.0260      -3.0290    ***
## starter_CB1_grades_defense_12w      -0.0064      -0.5074       
## starter_CB2_grades_defense_12w      -0.0052      -0.4256       
## starter_CB3_grades_defense_12w      -0.0107      -1.1057       
## starter_S1_grades_defense_12w       -0.0031      -0.2579       
## starter_S2_grades_defense_12w       -0.0104      -0.9228       
## starter_S3_grades_defense_12w       -0.0045      -0.5255       
## starter_OL_grades_pass_block_12w       0.0478       2.6502    ***
## starter_OL_grades_run_block_12w      -0.0375      -1.8650      *
## yardline_1_10                       -0.0575      -2.2307     **
## yardline_11_20                       0.0004       0.0127       
## yardline_21_30                      -0.0018      -0.0655       
## yardline_41_50                       0.0471       1.9497      *
## yardline_51_60                       0.0157       0.5434       
## yardline_61_70                       0.0490       1.5169      .
## yardline_71_80                       0.0677       1.6736      *
## yardline_81_90                       0.1336       2.2414     **
## yardline_91_100                      0.1123       1.0637       
## year2017_team_ARI                    0.0580       0.3117       
## year2017_team_BUF                   -0.1454      -0.7439       
## year2017_team_CHI                   -0.0008      -0.0049       
## year2017_team_CLE                    0.1489       0.7263       
## year2017_team_DAL                   -0.1795      -1.0456       
## year2017_team_DET                   -0.0805      -0.4621       
## year2017_team_GB                     0.3023       1.8223      *
## year2017_team_HOU                    0.3540       1.6479      *
## year2017_team_MIA                   -0.1850      -1.0440       
## year2017_team_MIN                   -0.1467      -0.8259       
## year2017_team_NE                    -0.0364      -0.1946       
## year2017_team_SF                     0.3768       1.8935      *
## year2017_team_BAL                   -0.0036      -0.0187       
## year2017_team_DEN                    0.0370       0.2025       
## year2017_team_LA                     0.0730       0.3915       
## year2017_team_NYG                   -0.0733      -0.4303       
## year2017_team_OAK                   -0.0127      -0.0678       
## year2017_team_SEA                    0.1161       0.6151       
## year2017_team_CAR                    0.0467       0.2044       
## year2017_team_CIN                    0.1067       0.5257       
## year2017_team_IND                    0.1930       1.0403       
## year2017_team_NO                     0.0508       0.2334       
## year2017_team_PHI                    0.0136       0.0749       
## year2017_team_PIT                   -0.1692      -1.0049       
## year2017_team_TEN                    0.0240       0.1108       
## year2017_team_WAS                    0.0146       0.0771       
## year2017_team_KC                     0.2804       1.4323       
## year2017_team_LAC                   -0.0037      -0.0189       
## year2017_team_NYJ                    0.1541       0.7204       
## year2017_team_TB                     0.0463       0.1943       
## year2017_team_ATL                   -0.0334      -0.1735       
## year2017_team_JAX                    0.1198       0.5952       
## year2018_team_ARI                    0.1497       1.0241       
## year2018_team_BAL                    0.0549       0.3722       
## year2018_team_CAR                   -0.0214      -0.1427       
## year2018_team_CLE                   -0.0663      -0.4774       
## year2018_team_DET                    0.0121       0.0847       
## year2018_team_HOU                    0.1280       0.7777       
## year2018_team_IND                   -0.1346      -0.9717       
## year2018_team_KC                     0.0360       0.2580       
## year2018_team_NYG                    0.0598       0.3453       
## year2018_team_OAK                   -0.0705      -0.4132       
## year2018_team_PHI                    0.0211       0.1454       
## year2018_team_SEA                   -0.0691      -0.4124       
## year2018_team_BUF                   -0.0944      -0.5803       
## year2018_team_CHI                   -0.0144      -0.1077       
## year2018_team_CIN                   -0.1248      -0.7487       
## year2018_team_DAL                   -0.0460      -0.3060       
## year2018_team_DEN                    0.0466       0.3153       
## year2018_team_GB                    -0.0392      -0.2308       
## year2018_team_LAC                    0.0652       0.4514       
## year2018_team_NE                    -0.1489      -0.9145       
## year2018_team_NO                     0.0383       0.2746       
## year2018_team_PIT                    0.0257       0.1313       
## year2018_team_SF                     0.0195       0.1288       
## year2018_team_MIA                    0.0871       0.6254       
## year2018_team_MIN                    0.0194       0.1229       
## year2018_team_NYJ                    0.1541       0.6967       
## year2018_team_TB                     0.0036       0.0221       
## year2018_team_ATL                    0.0426       0.2957       
## year2018_team_JAX                   -0.0164      -0.1073       
## year2018_team_LA                    -0.1904      -1.2315       
## year2018_team_TEN                    0.1012       0.6215       
## year2018_team_WAS                   -0.0146      -0.0733       
## year2019_team_ARI                   -0.1353      -0.8791       
## year2019_team_BUF                   -0.1318      -1.0536       
## year2019_team_CHI                    0.0728       0.4984       
## year2019_team_CLE                    0.0885       0.5763       
## year2019_team_DAL                   -0.0287      -0.1721       
## year2019_team_IND                   -0.0565      -0.4182       
## year2019_team_JAX                    0.1339       0.8645       
## year2019_team_KC                     0.0000       0.0003       
## year2019_team_LAC                   -0.0892      -0.6416       
## year2019_team_MIN                   -0.0876      -0.6155       
## year2019_team_NE                    -0.0393      -0.2335       
## year2019_team_NO                    -0.1766      -1.1566       
## year2019_team_PHI                    0.0652       0.4411       
## year2019_team_SEA                    0.0361       0.1855       
## year2019_team_SF                    -0.0687      -0.5064       
## year2019_team_TB                    -0.1335      -0.9682       
## year2019_team_BAL                    0.0155       0.1103       
## year2019_team_CAR                   -0.1061      -0.6524       
## year2019_team_DEN                    0.1079       0.7307       
## year2019_team_DET                   -0.1117      -0.7500       
## year2019_team_HOU                   -0.0549      -0.3812       
## year2019_team_LA                    -0.1430      -0.8583       
## year2019_team_MIA                   -0.2921      -1.8364      *
## year2019_team_NYG                   -0.1639      -1.0338       
## year2019_team_NYJ                   -0.2215      -1.6695      *
## year2019_team_OAK                    0.0243       0.1500       
## year2019_team_PIT                   -0.3877      -3.1962    ***
## year2019_team_TEN                   -0.1567      -1.1065       
## year2019_team_CIN                    0.0803       0.5380       
## year2019_team_WAS                   -0.0729      -0.4764       
## year2019_team_ATL                   -0.0170      -0.1114       
## year2019_team_GB                    -0.0749      -0.4978       
## year2020_team_ATL                    0.0565       0.3629       
## year2020_team_BAL                    0.0756       0.4950       
## year2020_team_BUF                    0.0397       0.2120       
## year2020_team_CAR                    0.1358       0.8258       
## year2020_team_CIN                    0.0978       0.6515       
## year2020_team_DEN                   -0.0486      -0.2892       
## year2020_team_DET                   -0.1105      -0.7293       
## year2020_team_JAX                   -0.0892      -0.5577       
## year2020_team_KC                     0.0378       0.2290       
## year2020_team_LA                    -0.1800      -1.0385       
## year2020_team_MIN                    0.1919       1.3741       
## year2020_team_NE                    -0.0188      -0.1192       
## year2020_team_NO                     0.0391       0.2645       
## year2020_team_NYG                    0.0579       0.3776       
## year2020_team_SF                     0.0654       0.3871       
## year2020_team_WAS                    0.0334       0.2239       
## year2020_team_CHI                    0.1034       0.6512       
## year2020_team_DAL                    0.0024       0.0158       
## year2020_team_GB                     0.0182       0.1007       
## year2020_team_HOU                   -0.1403      -0.8853       
## year2020_team_MIA                   -0.1064      -0.6490       
## year2020_team_NYJ                    0.0711       0.4151       
## year2020_team_TB                     0.0516       0.3241       
## year2020_team_TEN                   -0.0705      -0.4324       
## year2020_team_ARI                    0.0774       0.4608       
## year2020_team_CLE                   -0.2300      -1.3055       
## year2020_team_IND                   -0.1427      -0.8583       
## year2020_team_LAC                    0.0053       0.0300       
## year2020_team_PHI                    0.1584       1.0761       
## year2020_team_SEA                   -0.0146      -0.0884       
## year2020_team_LV                     0.0934       0.5987       
## year2020_team_PIT                   -0.1357      -0.8181       
## year2021_team_ATL                   -0.1950      -1.5172      .
## year2021_team_BUF                    0.0312       0.2475       
## year2021_team_CIN                   -0.1641      -1.3233       
## year2021_team_DAL                   -0.0886      -0.6527       
## year2021_team_DEN                    0.0729       0.5584       
## year2021_team_DET                   -0.1284      -0.9441       
## year2021_team_KC                     0.0715       0.5740       
## year2021_team_LA                    -0.0214      -0.1601       
## year2021_team_LV                     0.0690       0.4830       
## year2021_team_MIN                   -0.0422      -0.3178       
## year2021_team_NE                     0.0622       0.4611       
## year2021_team_NO                    -0.0027      -0.0195       
## year2021_team_NYG                    0.0681       0.5103       
## year2021_team_SF                     0.0001       0.0011       
## year2021_team_TEN                   -0.0219      -0.1742       
## year2021_team_ARI                    0.1160       0.9585       
## year2021_team_BAL                    0.1711       0.9587       
## year2021_team_CAR                   -0.0048      -0.0407       
## year2021_team_CHI                   -0.2013      -1.5977      .
## year2021_team_GB                     0.1042       0.8440       
## year2021_team_IND                   -0.0300      -0.2224       
## year2021_team_LAC                    0.0243       0.1661       
## year2021_team_MIA                    0.0295       0.1944       
## year2021_team_NYJ                   -0.0296      -0.2068       
## year2021_team_PHI                   -0.1667      -1.3058       
## year2021_team_SEA                   -0.1564      -1.0326       
## year2021_team_TB                     0.0360       0.2547       
## year2021_team_WAS                   -0.0674      -0.5408       
## year2021_team_CLE                   -0.0682      -0.5366       
## year2021_team_HOU                   -0.0585      -0.3989       
## year2021_team_JAX                   -0.0131      -0.0903       
## year2021_team_PIT                    0.0351       0.2576       
## year2022_team_ARI                   -0.1633      -1.2621       
## year2022_team_ATL                   -0.1989      -1.5068      .
## year2022_team_CAR                    0.0912       0.6131       
## year2022_team_CHI                    0.0021       0.0124       
## year2022_team_CIN                   -0.1315      -0.8763       
## year2022_team_HOU                   -0.0338      -0.2425       
## year2022_team_IND                   -0.0877      -0.6546       
## year2022_team_LAC                   -0.1329      -1.0128       
## year2022_team_MIA                   -0.1554      -1.2487       
## year2022_team_SEA                   -0.0081      -0.0597       
## year2022_team_TB                     0.0082       0.0629       
## year2022_team_TEN                    0.1974       1.6904      *
## year2022_team_WAS                    0.0467       0.3633       
## year2022_team_BAL                   -0.2262      -1.5462      .
## year2022_team_BUF                    0.0850       0.6436       
## year2022_team_DAL                    0.0218       0.1280       
## year2022_team_DET                   -0.0051      -0.0405       
## year2022_team_GB                    -0.1154      -0.8298       
## year2022_team_JAX                   -0.1625      -1.4218       
## year2022_team_KC                    -0.1670      -0.9826       
## year2022_team_LA                     0.1738       1.2822       
## year2022_team_LV                     0.1431       0.9762       
## year2022_team_NO                    -0.0474      -0.3028       
## year2022_team_PHI                    0.0633       0.4953       
## year2022_team_PIT                    0.1494       1.1481       
## year2022_team_DEN                    0.0792       0.6703       
## year2022_team_MIN                   -0.1038      -0.6735       
## year2022_team_NE                     0.0207       0.1460       
## year2022_team_NYJ                   -0.1373      -1.0658       
## year2022_team_NYG                   -0.0408      -0.2890       
## year2022_team_SF                    -0.1606      -0.9622       
## year2023_team_BAL                   -0.0413      -0.3093       
## year2023_team_CHI                   -0.1417      -1.0173       
## year2023_team_CLE                   -0.1339      -0.8722       
## year2023_team_GB                    -0.0231      -0.1802       
## year2023_team_IND                    0.1211       0.9365       
## year2023_team_KC                    -0.0072      -0.0509       
## year2023_team_LAC                    0.0700       0.4705       
## year2023_team_LV                     0.0199       0.1566       
## year2023_team_MIA                    0.0497       0.3748       
## year2023_team_MIN                    0.1915       1.6293      .
## year2023_team_NO                    -0.0860      -0.5971       
## year2023_team_NYG                    0.0669       0.4786       
## year2023_team_SEA                   -0.2697      -2.1611     **
## year2023_team_SF                     0.0141       0.0905       
## year2023_team_WAS                    0.1852       1.5333      .
## year2023_team_ATL                   -0.1113      -0.7633       
## year2023_team_BUF                   -0.1017      -0.6709       
## year2023_team_CAR                    0.1135       0.8756       
## year2023_team_DAL                    0.1036       0.6937       
## year2023_team_DEN                    0.0034       0.0268       
## year2023_team_HOU                    0.0173       0.1184       
## year2023_team_LA                     0.0421       0.2839       
## year2023_team_NE                     0.0911       0.6682       
## year2023_team_PHI                   -0.0660      -0.4956       
## year2023_team_PIT                    0.0126       0.0806       
## year2023_team_TEN                   -0.0008      -0.0058       
## year2023_team_ARI                   -0.1432      -1.0287       
## year2023_team_CIN                   -0.1184      -0.7796       
## year2023_team_DET                    0.0151       0.1216       
## year2023_team_TB                     0.0991       0.7121       
## year2023_team_JAX                   -0.1081      -0.7308       
## year2023_team_NYJ                    0.2160       1.5520      .
## is_first_half                       -0.0115      -0.6466       
## time_in_half                         0.0170       1.7383      *
## home_attendance                     -0.0084      -0.1118       
## GIMR                                 0.0505       2.0396     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1111214 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.60
## prev_singleback_rate                                   5.54
## cover1_rate                                            6.07
## cover3_rate                                            6.43
## starter_RB_grades_run_12w                              6.26
## starter_RB_grades_pass_route_12w                       5.83
## starter_OL_grades_pass_block_12w                       6.34
## starter_OL_grades_run_block_12w                        7.94
## home_attendance                                       13.82
## 
## 
##  ================================================================================ 
## MODEL COMPARISON - Adjusted R-squared values
## ================================================================================ 
## 
## Player Model with GIMR: 0.112072 
## Starter Model with GIMR: 0.1111214 
## 
## 
## ==================================================================================================== 
## ANALYZING DATASET 2/8: Offense Yards
## ==================================================================================================== 
## 
## Reading data: processed_predict_ccafd_off_yards.csv.csv.gz
## Reading data: processed_predict_ccfd_off_yards.csv.csv.gz
## 
## Phase 1: Validation Phase
## 
## Running 2 test iterations with best parameters...
## 
## Test Results over 2 iterations:
## Mean AUC: 0.8838284 
## SD AUC: 0.001437615 
## 95% CI: 0.8810107 to 0.8866461 
## 
## 
##  ================================================================================ 
## MODEL: Player Model with GIMR 
## ================================================================================ 
## 
## 
## Player Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.4293       3.4331    ***
## ydstogo                             -0.1104     -12.4659    ***
## posteam_timeouts_remaining           0.0128       1.3985       
## defteam_timeouts_remaining           0.0089       0.9997       
## rush_attempt                         0.1539       7.7846    ***
## week                                 0.0073       0.7277       
## temp                                -0.0089      -0.8417       
## wind                                 0.0095       0.8958       
## vegas_wp                             0.0164       1.4521      .
## spread_line                         -0.0024      -0.1953       
## total_line                           0.0238       1.8297      *
## prep_days                            0.0061       0.7867       
## overall_win_pct                      0.0070       0.5357       
## team_win_pct                         0.0189       1.3178       
## prev_win_pct                        -0.0346      -2.7142    ***
## prev_shotgun_rate                    0.0136       0.6110       
## prev_singleback_rate                 0.0128       0.7489       
## prev_empty_rate                      0.0110       0.8850       
## prev_iform_rate                      0.0074       0.4695       
## prev_shotgun_success                 0.0036       0.3056       
## prev_singleback_success              0.0097       0.8035       
## prev_empty_success                   0.0043       0.3900       
## prev_iform_success                   0.0212       2.1083     **
## prev_stop_rate_run                   0.0003       0.0261       
## prev_stop_rate_pass                 -0.0348      -3.3645    ***
## shotgun_rate                         0.0134       0.9779       
## singleback_rate                      0.0063       0.5264       
## empty_rate                          -0.0043      -0.3870       
## iform_rate                          -0.0203      -1.9059      *
## shotgun_success                     -0.0196      -2.1913     **
## singleback_success                  -0.0057      -0.6192       
## empty_success                       -0.0077      -0.7848       
## iform_success                       -0.0157      -1.6286      .
## def_stop_rate_run                    0.0163       1.7500      *
## def_stop_rate_pass                  -0.0109      -1.1473       
## avg_pass_rushers                    -0.0096      -0.8565       
## avg_box_defenders                   -0.0059      -0.5603       
## cover0_rate                         -0.0004      -0.0387       
## cover1_rate                         -0.0095      -0.5313       
## cover2_rate                         -0.0044      -0.3362       
## cover3_rate                          0.0295       1.6178      .
## cover4_rate                          0.0134       0.9912       
## cover6_rate                         -0.0062      -0.5076       
## two_man_rate                         0.0163       1.7375      *
## prevent_rate                         0.0205       2.5661     **
## roof_outdoors                       -0.0038      -0.1579       
## posteam_type_home                   -0.0208      -1.3309       
## QB_short_yards_12w                   0.0197       1.5299      .
## QB_medium_yards_12w                  0.0067       0.5080       
## QB_deep_yards_12w                   -0.0186      -1.6932      *
## RB_grades_pass_block_12w             0.0123       1.5033      .
## RB_yards_12w                         0.0154       1.8225      *
## RB_short_yards_12w                  -0.0127      -1.4044       
## RB_medium_yards_12w                 -0.0067      -0.8748       
## RB_deep_yards_12w                   -0.0012      -0.1403       
## WR1_grades_pass_block_12w           -0.0031      -0.3746       
## WR1_grades_run_block_12w            -0.0156      -1.5902      .
## WR1_short_yards_12w                 -0.0010      -0.0979       
## WR1_medium_yards_12w                -0.0048      -0.4508       
## WR1_deep_yards_12w                   0.0164       1.7390      *
## WR2_grades_pass_block_12w           -0.0057      -0.6651       
## WR2_grades_run_block_12w            -0.0006      -0.0497       
## WR2_short_yards_12w                  0.0049       0.4491       
## WR2_medium_yards_12w                -0.0187      -1.6354      .
## WR2_deep_yards_12w                   0.0078       0.7933       
## WR3_grades_run_block_12w             0.0071       0.5760       
## WR3_short_yards_12w                  0.0096       0.8683       
## WR3_medium_yards_12w                 0.0014       0.1323       
## WR3_deep_yards_12w                   0.0022       0.2262       
## TE1_grades_pass_block_12w            0.0253       2.4075     **
## TE1_grades_run_block_12w            -0.0093      -0.8620       
## TE1_short_yards_12w                 -0.0079      -0.7839       
## TE1_medium_yards_12w                 0.0047       0.4738       
## TE1_deep_yards_12w                  -0.0044      -0.5264       
## DL1_grades_defense_12w              -0.0159      -1.9558      *
## DL2_grades_defense_12w               0.0033       0.3825       
## DL3_grades_defense_12w               0.0122       1.0486       
## DL4_grades_defense_12w              -0.0304      -2.5055     **
## LB1_grades_defense_12w               0.0054       0.6273       
## LB2_grades_defense_12w               0.0031       0.3593       
## LB3_grades_defense_12w              -0.0183      -1.5322      .
## LB4_grades_defense_12w              -0.0012      -0.1096       
## CB1_grades_defense_12w              -0.0127      -1.3975       
## CB2_grades_defense_12w              -0.0033      -0.3529       
## CB3_grades_defense_12w               0.0160       1.4997      .
## S1_grades_defense_12w               -0.0082      -1.0610       
## S2_grades_defense_12w                0.0054       0.6111       
## S3_grades_defense_12w                0.0089       0.9308       
## OL_grades_pass_block_12w            -0.0036      -0.3383       
## OL_grades_run_block_12w             -0.0038      -0.3679       
## yardline_1_10                       -0.0637      -2.3678     **
## yardline_11_20                       0.0171       0.5885       
## yardline_21_30                       0.0045       0.1597       
## yardline_41_50                       0.0475       1.9549      *
## yardline_51_60                       0.0186       0.6412       
## yardline_61_70                       0.0474       1.4601      .
## yardline_71_80                       0.0710       1.7689      *
## yardline_81_90                       0.1349       2.2450     **
## yardline_91_100                      0.0936       0.8970       
## year2017_team_ARI                    0.1005       0.5366       
## year2017_team_BUF                   -0.1211      -0.6337       
## year2017_team_CHI                    0.0516       0.3007       
## year2017_team_CLE                    0.1948       0.9823       
## year2017_team_DAL                   -0.1605      -0.9465       
## year2017_team_DET                   -0.0469      -0.2697       
## year2017_team_GB                     0.3561       2.1753     **
## year2017_team_HOU                    0.3445       1.6846      *
## year2017_team_MIA                   -0.2239      -1.2692       
## year2017_team_MIN                   -0.0952      -0.5312       
## year2017_team_NE                     0.0028       0.0152       
## year2017_team_SF                     0.3941       2.0204     **
## year2017_team_BAL                    0.0112       0.0584       
## year2017_team_DEN                   -0.0384      -0.2114       
## year2017_team_LA                     0.0566       0.3167       
## year2017_team_NYG                   -0.0529      -0.3093       
## year2017_team_OAK                   -0.0860      -0.4715       
## year2017_team_SEA                    0.1536       0.8193       
## year2017_team_CAR                    0.1445       0.6751       
## year2017_team_CIN                    0.1874       0.9245       
## year2017_team_IND                    0.1562       0.8664       
## year2017_team_NO                     0.0930       0.4186       
## year2017_team_PHI                    0.0720       0.4026       
## year2017_team_PIT                   -0.1491      -0.8939       
## year2017_team_TEN                    0.1352       0.6346       
## year2017_team_WAS                    0.0471       0.2468       
## year2017_team_KC                     0.2920       1.5463      .
## year2017_team_LAC                    0.0177       0.0966       
## year2017_team_NYJ                    0.1692       0.8060       
## year2017_team_TB                     0.0743       0.3226       
## year2017_team_ATL                   -0.0026      -0.0135       
## year2017_team_JAX                    0.0832       0.4242       
## year2018_team_ARI                    0.0761       0.5178       
## year2018_team_BAL                    0.0956       0.6494       
## year2018_team_CAR                    0.0936       0.6280       
## year2018_team_CLE                   -0.0166      -0.1192       
## year2018_team_DET                    0.1203       0.8588       
## year2018_team_HOU                    0.2532       1.5113      .
## year2018_team_IND                   -0.1176      -0.8598       
## year2018_team_KC                     0.1284       0.9403       
## year2018_team_NYG                    0.1089       0.6288       
## year2018_team_OAK                   -0.1324      -0.7810       
## year2018_team_PHI                    0.0983       0.6763       
## year2018_team_SEA                   -0.0695      -0.3963       
## year2018_team_BUF                   -0.0787      -0.4907       
## year2018_team_CHI                   -0.0138      -0.1075       
## year2018_team_CIN                   -0.0270      -0.1633       
## year2018_team_DAL                   -0.0390      -0.2645       
## year2018_team_DEN                    0.0253       0.1739       
## year2018_team_GB                    -0.0091      -0.0541       
## year2018_team_LAC                    0.0245       0.1692       
## year2018_team_NE                    -0.0641      -0.4139       
## year2018_team_NO                     0.0910       0.6808       
## year2018_team_PIT                    0.0720       0.3837       
## year2018_team_SF                     0.0330       0.2160       
## year2018_team_MIA                    0.0951       0.6587       
## year2018_team_MIN                    0.0316       0.1990       
## year2018_team_NYJ                    0.1660       0.7556       
## year2018_team_TB                     0.0344       0.2020       
## year2018_team_ATL                    0.0584       0.4229       
## year2018_team_JAX                    0.0289       0.1860       
## year2018_team_LA                    -0.1527      -0.9386       
## year2018_team_TEN                    0.1376       0.8389       
## year2018_team_WAS                    0.1103       0.5494       
## year2019_team_ARI                   -0.0827      -0.5149       
## year2019_team_BUF                   -0.1269      -0.9909       
## year2019_team_CHI                    0.0888       0.6133       
## year2019_team_CLE                    0.1103       0.7540       
## year2019_team_DAL                   -0.0412      -0.2489       
## year2019_team_IND                   -0.0208      -0.1561       
## year2019_team_JAX                    0.1057       0.6992       
## year2019_team_KC                     0.0228       0.1684       
## year2019_team_LAC                   -0.0895      -0.6188       
## year2019_team_MIN                   -0.0702      -0.4786       
## year2019_team_NE                    -0.0055      -0.0334       
## year2019_team_NO                    -0.2118      -1.3877       
## year2019_team_PHI                    0.0590       0.3949       
## year2019_team_SEA                    0.0214       0.1101       
## year2019_team_SF                    -0.0000      -0.0001       
## year2019_team_TB                    -0.1078      -0.7688       
## year2019_team_BAL                    0.0315       0.2248       
## year2019_team_CAR                   -0.0506      -0.3096       
## year2019_team_DEN                    0.1147       0.8097       
## year2019_team_DET                   -0.0815      -0.5272       
## year2019_team_HOU                    0.0091       0.0610       
## year2019_team_LA                    -0.1173      -0.7494       
## year2019_team_MIA                   -0.2744      -1.7588      *
## year2019_team_NYG                   -0.1503      -0.9261       
## year2019_team_NYJ                   -0.2096      -1.6346      .
## year2019_team_OAK                   -0.0254      -0.1631       
## year2019_team_PIT                   -0.2663      -2.2877     **
## year2019_team_TEN                   -0.1505      -1.0819       
## year2019_team_CIN                    0.0757       0.5294       
## year2019_team_WAS                   -0.0438      -0.2961       
## year2019_team_ATL                    0.0116       0.0742       
## year2019_team_GB                    -0.0607      -0.4143       
## year2020_team_ATL                    0.0831       0.5437       
## year2020_team_BAL                    0.0698       0.4521       
## year2020_team_BUF                   -0.0198      -0.1054       
## year2020_team_CAR                    0.1161       0.6943       
## year2020_team_CIN                    0.1070       0.7108       
## year2020_team_DEN                   -0.0913      -0.5460       
## year2020_team_DET                   -0.1380      -0.8921       
## year2020_team_JAX                   -0.1315      -0.8256       
## year2020_team_KC                     0.0800       0.5007       
## year2020_team_LA                    -0.1847      -1.0461       
## year2020_team_MIN                    0.1702       1.1955       
## year2020_team_NE                    -0.0144      -0.0938       
## year2020_team_NO                     0.0592       0.4082       
## year2020_team_NYG                    0.0147       0.0978       
## year2020_team_SF                     0.1076       0.6495       
## year2020_team_WAS                    0.0366       0.2508       
## year2020_team_CHI                    0.0359       0.2272       
## year2020_team_DAL                   -0.0197      -0.1303       
## year2020_team_GB                    -0.0210      -0.1199       
## year2020_team_HOU                   -0.0829      -0.5203       
## year2020_team_MIA                   -0.1551      -0.9544       
## year2020_team_NYJ                   -0.0239      -0.1418       
## year2020_team_TB                     0.0467       0.2921       
## year2020_team_TEN                   -0.0929      -0.5599       
## year2020_team_ARI                    0.1037       0.6205       
## year2020_team_CLE                   -0.2550      -1.4806      .
## year2020_team_IND                   -0.1553      -0.9434       
## year2020_team_LAC                    0.0410       0.2239       
## year2020_team_PHI                    0.1228       0.8351       
## year2020_team_SEA                   -0.0277      -0.1685       
## year2020_team_LV                     0.1232       0.7976       
## year2020_team_PIT                   -0.1115      -0.6716       
## year2021_team_ATL                   -0.1996      -1.5816      .
## year2021_team_BUF                    0.0592       0.4735       
## year2021_team_CIN                   -0.2313      -1.8739      *
## year2021_team_DAL                   -0.1019      -0.7235       
## year2021_team_DEN                    0.0678       0.5001       
## year2021_team_DET                   -0.0759      -0.5677       
## year2021_team_KC                     0.0323       0.2573       
## year2021_team_LA                     0.0102       0.0768       
## year2021_team_LV                     0.0321       0.2180       
## year2021_team_MIN                   -0.0359      -0.2790       
## year2021_team_NE                     0.0627       0.4614       
## year2021_team_NO                     0.0022       0.0165       
## year2021_team_NYG                    0.0014       0.0104       
## year2021_team_SF                     0.0115       0.0858       
## year2021_team_TEN                   -0.0690      -0.5635       
## year2021_team_ARI                    0.0800       0.6791       
## year2021_team_BAL                    0.1184       0.6580       
## year2021_team_CAR                   -0.0735      -0.6253       
## year2021_team_CHI                   -0.2235      -1.8168      *
## year2021_team_GB                     0.0990       0.8057       
## year2021_team_IND                   -0.0516      -0.3856       
## year2021_team_LAC                    0.0531       0.3666       
## year2021_team_MIA                    0.0211       0.1379       
## year2021_team_NYJ                   -0.0053      -0.0355       
## year2021_team_PHI                   -0.1654      -1.3163       
## year2021_team_SEA                   -0.1654      -1.1012       
## year2021_team_TB                     0.0496       0.3548       
## year2021_team_WAS                   -0.0373      -0.2969       
## year2021_team_CLE                   -0.1042      -0.8157       
## year2021_team_HOU                   -0.0934      -0.6513       
## year2021_team_JAX                   -0.0501      -0.3401       
## year2021_team_PIT                    0.0104       0.0778       
## year2022_team_ARI                   -0.1416      -1.0997       
## year2022_team_ATL                   -0.2884      -2.1989     **
## year2022_team_CAR                    0.1553       1.0837       
## year2022_team_CHI                   -0.0543      -0.3335       
## year2022_team_CIN                   -0.1209      -0.8182       
## year2022_team_HOU                   -0.0523      -0.3753       
## year2022_team_IND                   -0.1185      -0.9142       
## year2022_team_LAC                   -0.0808      -0.6083       
## year2022_team_MIA                   -0.1572      -1.2863       
## year2022_team_SEA                   -0.0633      -0.4872       
## year2022_team_TB                     0.0209       0.1635       
## year2022_team_TEN                    0.1603       1.3782       
## year2022_team_WAS                    0.0003       0.0021       
## year2022_team_BAL                   -0.1735      -1.2157       
## year2022_team_BUF                    0.0412       0.3191       
## year2022_team_DAL                    0.0003       0.0020       
## year2022_team_DET                   -0.1068      -0.8519       
## year2022_team_GB                    -0.1354      -0.9741       
## year2022_team_JAX                   -0.1394      -1.2470       
## year2022_team_KC                    -0.1084      -0.6240       
## year2022_team_LA                     0.1844       1.3907       
## year2022_team_LV                     0.1439       0.9973       
## year2022_team_NO                    -0.0352      -0.2289       
## year2022_team_PHI                    0.0691       0.5377       
## year2022_team_PIT                    0.1941       1.5547      .
## year2022_team_DEN                    0.0513       0.4203       
## year2022_team_MIN                   -0.1062      -0.6887       
## year2022_team_NE                     0.0131       0.0918       
## year2022_team_NYJ                   -0.1199      -0.9360       
## year2022_team_NYG                   -0.0893      -0.6264       
## year2022_team_SF                    -0.1440      -0.8305       
## year2023_team_BAL                   -0.0401      -0.3066       
## year2023_team_CHI                   -0.1584      -1.1625       
## year2023_team_CLE                   -0.1181      -0.8007       
## year2023_team_GB                     0.0431       0.3238       
## year2023_team_IND                    0.0763       0.6094       
## year2023_team_KC                     0.0423       0.2966       
## year2023_team_LAC                    0.0423       0.3060       
## year2023_team_LV                    -0.0160      -0.1267       
## year2023_team_MIA                    0.0535       0.4017       
## year2023_team_MIN                    0.1637       1.3744       
## year2023_team_NO                    -0.0286      -0.2041       
## year2023_team_NYG                    0.0554       0.4126       
## year2023_team_SEA                   -0.2711      -2.2432     **
## year2023_team_SF                     0.0479       0.3105       
## year2023_team_WAS                    0.1666       1.3351       
## year2023_team_ATL                   -0.1084      -0.7460       
## year2023_team_BUF                   -0.0822      -0.5438       
## year2023_team_CAR                    0.0478       0.3794       
## year2023_team_DAL                    0.0835       0.6046       
## year2023_team_DEN                    0.0206       0.1586       
## year2023_team_HOU                   -0.0310      -0.2046       
## year2023_team_LA                    -0.0105      -0.0700       
## year2023_team_NE                     0.0305       0.2326       
## year2023_team_PHI                   -0.0472      -0.3593       
## year2023_team_PIT                   -0.0253      -0.1610       
## year2023_team_TEN                    0.0111       0.0755       
## year2023_team_ARI                   -0.1716      -1.2324       
## year2023_team_CIN                   -0.1432      -0.9293       
## year2023_team_DET                    0.0500       0.4049       
## year2023_team_TB                     0.1042       0.7716       
## year2023_team_JAX                   -0.0673      -0.4552       
## year2023_team_NYJ                    0.1879       1.4245       
## is_first_half                       -0.0159      -0.8852       
## time_in_half                         0.0142       1.4457      .
## home_attendance                     -0.0297      -0.3942       
## GIMR                                 0.0497       2.0460     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.112259 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.66
## prev_singleback_rate                                   5.70
## cover1_rate                                            6.10
## cover3_rate                                            6.49
## home_attendance                                       13.85
## 
## 
##  ================================================================================ 
## MODEL: Starter Model with GIMR 
## ================================================================================ 
## 
## 
## Starter Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.3919       3.1624    ***
## ydstogo                             -0.1092     -12.6768    ***
## posteam_timeouts_remaining           0.0117       1.2842       
## defteam_timeouts_remaining           0.0069       0.7744       
## rush_attempt                         0.1396       7.3890    ***
## week                                 0.0094       0.9349       
## temp                                -0.0108      -1.0144       
## wind                                 0.0041       0.3850       
## vegas_wp                             0.0101       0.9171       
## spread_line                         -0.0109      -0.8692       
## total_line                           0.0330       2.4610     **
## prep_days                            0.0064       0.8323       
## overall_win_pct                      0.0033       0.2515       
## team_win_pct                         0.0196       1.3755       
## prev_win_pct                        -0.0279      -2.1656     **
## prev_shotgun_rate                    0.0014       0.0638       
## prev_singleback_rate                 0.0003       0.0181       
## prev_empty_rate                      0.0063       0.5044       
## prev_iform_rate                     -0.0028      -0.1734       
## prev_shotgun_success                 0.0024       0.2028       
## prev_singleback_success              0.0072       0.5865       
## prev_empty_success                   0.0041       0.3683       
## prev_iform_success                   0.0279       2.7855    ***
## prev_stop_rate_run                  -0.0007      -0.0629       
## prev_stop_rate_pass                 -0.0340      -3.3393    ***
## shotgun_rate                         0.0128       0.9284       
## singleback_rate                      0.0068       0.5735       
## empty_rate                          -0.0035      -0.3117       
## iform_rate                          -0.0174      -1.6253      .
## shotgun_success                     -0.0215      -2.3803     **
## singleback_success                  -0.0092      -0.9878       
## empty_success                       -0.0074      -0.7607       
## iform_success                       -0.0171      -1.7522      *
## def_stop_rate_run                    0.0170       1.8378      *
## def_stop_rate_pass                  -0.0123      -1.2981       
## avg_pass_rushers                    -0.0126      -1.1381       
## avg_box_defenders                   -0.0050      -0.4780       
## cover0_rate                          0.0018       0.1576       
## cover1_rate                         -0.0071      -0.3989       
## cover2_rate                         -0.0000      -0.0011       
## cover3_rate                          0.0235       1.2834       
## cover4_rate                          0.0125       0.9297       
## cover6_rate                         -0.0053      -0.4393       
## two_man_rate                         0.0168       1.7837      *
## prevent_rate                         0.0194       2.3868     **
## roof_outdoors                        0.0022       0.0897       
## posteam_type_home                   -0.0232      -1.4702      .
## starter_QB_short_yards_12w           0.0198       1.6489      *
## starter_QB_medium_yards_12w          0.0309       2.4453     **
## starter_QB_deep_yards_12w           -0.0380      -3.3414    ***
## starter_RB_grades_pass_block_12w      -0.0136      -1.4595      .
## starter_RB_yards_12w                 0.0004       0.0475       
## starter_RB_short_yards_12w          -0.0077      -0.8398       
## starter_RB_medium_yards_12w         -0.0206      -2.4607     **
## starter_RB_deep_yards_12w            0.0059       0.6475       
## starter_WR1_grades_pass_block_12w      -0.0018      -0.2162       
## starter_WR1_grades_run_block_12w       0.0083       0.6005       
## starter_WR1_short_yards_12w         -0.0055      -0.5502       
## starter_WR1_medium_yards_12w        -0.0008      -0.0724       
## starter_WR1_deep_yards_12w           0.0295       3.1244    ***
## starter_WR2_grades_pass_block_12w      -0.0038      -0.4590       
## starter_WR2_grades_run_block_12w      -0.0211      -1.4898      .
## starter_WR2_short_yards_12w         -0.0075      -0.7605       
## starter_WR2_medium_yards_12w        -0.0101      -0.9658       
## starter_WR2_deep_yards_12w           0.0152       1.5815      .
## starter_WR3_grades_pass_block_12w      -0.0056      -0.6617       
## starter_WR3_grades_run_block_12w      -0.0077      -0.5954       
## starter_WR3_short_yards_12w         -0.0120      -1.1931       
## starter_WR3_medium_yards_12w        -0.0180      -1.7125      *
## starter_WR3_deep_yards_12w           0.0138       1.5124      .
## starter_TE1_grades_pass_block_12w       0.0239       2.2152     **
## starter_TE1_grades_run_block_12w      -0.0180      -1.3559       
## starter_TE1_short_yards_12w          0.0034       0.3161       
## starter_TE1_medium_yards_12w        -0.0169      -1.6104      .
## starter_TE1_deep_yards_12w          -0.0106      -1.1365       
## starter_DL1_grades_defense_12w       0.0074       0.6330       
## starter_DL2_grades_defense_12w       0.0108       0.9241       
## starter_DL3_grades_defense_12w       0.0027       0.2347       
## starter_DL4_grades_defense_12w       0.0111       1.1447       
## starter_LB1_grades_defense_12w       0.0047       0.4172       
## starter_LB2_grades_defense_12w       0.0192       1.7017      *
## starter_LB3_grades_defense_12w       0.0110       1.1082       
## starter_LB4_grades_defense_12w      -0.0246      -2.8429    ***
## starter_CB1_grades_defense_12w      -0.0065      -0.5169       
## starter_CB2_grades_defense_12w       0.0044       0.3593       
## starter_CB3_grades_defense_12w      -0.0094      -0.9772       
## starter_S1_grades_defense_12w        0.0008       0.0706       
## starter_S2_grades_defense_12w       -0.0074      -0.6540       
## starter_S3_grades_defense_12w       -0.0053      -0.6273       
## starter_OL_grades_pass_block_12w       0.0414       2.2988     **
## starter_OL_grades_run_block_12w      -0.0290      -1.4430      .
## yardline_1_10                       -0.0535      -2.0708     **
## yardline_11_20                       0.0012       0.0399       
## yardline_21_30                      -0.0003      -0.0097       
## yardline_41_50                       0.0493       2.0487     **
## yardline_51_60                       0.0226       0.7881       
## yardline_61_70                       0.0485       1.4916      .
## yardline_71_80                       0.0700       1.7430      *
## yardline_81_90                       0.1295       2.1798     **
## yardline_91_100                      0.1232       1.1766       
## year2017_team_ARI                    0.0775       0.4198       
## year2017_team_BUF                   -0.0626      -0.3262       
## year2017_team_CHI                    0.0288       0.1676       
## year2017_team_CLE                    0.1667       0.8221       
## year2017_team_DAL                   -0.1461      -0.8389       
## year2017_team_DET                   -0.0617      -0.3587       
## year2017_team_GB                     0.3534       2.1254     **
## year2017_team_HOU                    0.4289       2.0823     **
## year2017_team_MIA                   -0.1592      -0.8974       
## year2017_team_MIN                   -0.1226      -0.6815       
## year2017_team_NE                    -0.0199      -0.1069       
## year2017_team_SF                     0.3778       1.8944      *
## year2017_team_BAL                   -0.0003      -0.0018       
## year2017_team_DEN                    0.0406       0.2233       
## year2017_team_LA                     0.1121       0.6198       
## year2017_team_NYG                   -0.0267      -0.1562       
## year2017_team_OAK                    0.0022       0.0120       
## year2017_team_SEA                    0.1769       0.9407       
## year2017_team_CAR                    0.0257       0.1129       
## year2017_team_CIN                    0.1441       0.7124       
## year2017_team_IND                    0.2055       1.1243       
## year2017_team_NO                     0.0934       0.4292       
## year2017_team_PHI                    0.0445       0.2428       
## year2017_team_PIT                   -0.1756      -1.0300       
## year2017_team_TEN                    0.0945       0.4344       
## year2017_team_WAS                    0.0731       0.3844       
## year2017_team_KC                     0.3089       1.6111      .
## year2017_team_LAC                    0.0435       0.2221       
## year2017_team_NYJ                    0.1812       0.8403       
## year2017_team_TB                     0.0398       0.1688       
## year2017_team_ATL                    0.0152       0.0805       
## year2017_team_JAX                    0.0925       0.4540       
## year2018_team_ARI                    0.2112       1.4249       
## year2018_team_BAL                    0.1033       0.6842       
## year2018_team_CAR                    0.0992       0.6414       
## year2018_team_CLE                   -0.0231      -0.1652       
## year2018_team_DET                    0.1048       0.7162       
## year2018_team_HOU                    0.2094       1.1929       
## year2018_team_IND                   -0.1429      -1.0321       
## year2018_team_KC                     0.0909       0.6452       
## year2018_team_NYG                    0.1302       0.7345       
## year2018_team_OAK                   -0.0158      -0.0934       
## year2018_team_PHI                    0.0381       0.2611       
## year2018_team_SEA                   -0.0515      -0.2901       
## year2018_team_BUF                   -0.0123      -0.0760       
## year2018_team_CHI                    0.0177       0.1318       
## year2018_team_CIN                   -0.0683      -0.4304       
## year2018_team_DAL                    0.0325       0.2136       
## year2018_team_DEN                    0.0195       0.1290       
## year2018_team_GB                    -0.0254      -0.1502       
## year2018_team_LAC                    0.0701       0.4884       
## year2018_team_NE                    -0.0323      -0.2013       
## year2018_team_NO                     0.0815       0.5768       
## year2018_team_PIT                    0.0009       0.0046       
## year2018_team_SF                     0.0300       0.1911       
## year2018_team_MIA                    0.1040       0.7370       
## year2018_team_MIN                    0.0773       0.4736       
## year2018_team_NYJ                    0.1720       0.7875       
## year2018_team_TB                     0.0025       0.0153       
## year2018_team_ATL                    0.0389       0.2710       
## year2018_team_JAX                    0.0028       0.0186       
## year2018_team_LA                    -0.1168      -0.7427       
## year2018_team_TEN                    0.1808       1.0554       
## year2018_team_WAS                    0.1197       0.5901       
## year2019_team_ARI                   -0.0821      -0.5321       
## year2019_team_BUF                   -0.0896      -0.7153       
## year2019_team_CHI                    0.0539       0.3707       
## year2019_team_CLE                    0.1138       0.7320       
## year2019_team_DAL                   -0.0732      -0.4443       
## year2019_team_IND                   -0.0485      -0.3633       
## year2019_team_JAX                    0.1267       0.8334       
## year2019_team_KC                     0.0231       0.1630       
## year2019_team_LAC                   -0.0762      -0.5456       
## year2019_team_MIN                   -0.0881      -0.6041       
## year2019_team_NE                    -0.0131      -0.0777       
## year2019_team_NO                    -0.1975      -1.2875       
## year2019_team_PHI                    0.0628       0.4295       
## year2019_team_SEA                    0.0203       0.1057       
## year2019_team_SF                    -0.0167      -0.1235       
## year2019_team_TB                    -0.1168      -0.8811       
## year2019_team_BAL                    0.0117       0.0828       
## year2019_team_CAR                   -0.1171      -0.6884       
## year2019_team_DEN                    0.0736       0.5143       
## year2019_team_DET                   -0.1183      -0.7560       
## year2019_team_HOU                   -0.0494      -0.3339       
## year2019_team_LA                    -0.1432      -0.8807       
## year2019_team_MIA                   -0.2508      -1.5639      .
## year2019_team_NYG                   -0.1226      -0.7620       
## year2019_team_NYJ                   -0.2149      -1.6319      .
## year2019_team_OAK                    0.0326       0.2085       
## year2019_team_PIT                   -0.3488      -2.8448    ***
## year2019_team_TEN                   -0.1439      -1.0183       
## year2019_team_CIN                    0.1014       0.6815       
## year2019_team_WAS                   -0.0367      -0.2389       
## year2019_team_ATL                    0.0344       0.2235       
## year2019_team_GB                    -0.0343      -0.2188       
## year2020_team_ATL                    0.1250       0.7842       
## year2020_team_BAL                    0.0901       0.5863       
## year2020_team_BUF                    0.0433       0.2308       
## year2020_team_CAR                    0.1879       1.0931       
## year2020_team_CIN                    0.1172       0.7919       
## year2020_team_DEN                   -0.0606      -0.3621       
## year2020_team_DET                   -0.0671      -0.4360       
## year2020_team_JAX                   -0.0724      -0.4476       
## year2020_team_KC                     0.0896       0.5258       
## year2020_team_LA                    -0.1195      -0.6935       
## year2020_team_MIN                    0.1988       1.4187       
## year2020_team_NE                     0.0529       0.3422       
## year2020_team_NO                     0.1007       0.6839       
## year2020_team_NYG                    0.0415       0.2710       
## year2020_team_SF                     0.1515       0.9026       
## year2020_team_WAS                    0.0856       0.5663       
## year2020_team_CHI                    0.1237       0.7864       
## year2020_team_DAL                    0.0409       0.2765       
## year2020_team_GB                     0.0201       0.1144       
## year2020_team_HOU                   -0.1486      -0.9175       
## year2020_team_MIA                   -0.0992      -0.6167       
## year2020_team_NYJ                    0.0946       0.5697       
## year2020_team_TB                     0.0751       0.4768       
## year2020_team_TEN                   -0.0132      -0.0811       
## year2020_team_ARI                    0.1290       0.7704       
## year2020_team_CLE                   -0.1990      -1.1449       
## year2020_team_IND                   -0.1651      -0.9843       
## year2020_team_LAC                    0.0761       0.4333       
## year2020_team_PHI                    0.2146       1.4646      .
## year2020_team_SEA                    0.0144       0.0879       
## year2020_team_LV                     0.1463       0.9276       
## year2020_team_PIT                   -0.1408      -0.8654       
## year2021_team_ATL                   -0.1407      -1.0683       
## year2021_team_BUF                    0.0931       0.7277       
## year2021_team_CIN                   -0.1885      -1.4889      .
## year2021_team_DAL                   -0.0749      -0.5426       
## year2021_team_DEN                    0.1246       0.9657       
## year2021_team_DET                   -0.0807      -0.5829       
## year2021_team_KC                     0.0620       0.4868       
## year2021_team_LA                    -0.0086      -0.0643       
## year2021_team_LV                     0.0909       0.6263       
## year2021_team_MIN                   -0.0057      -0.0419       
## year2021_team_NE                     0.1130       0.8273       
## year2021_team_NO                     0.0614       0.4449       
## year2021_team_NYG                    0.1034       0.7824       
## year2021_team_SF                    -0.0114      -0.0810       
## year2021_team_TEN                    0.0257       0.2023       
## year2021_team_ARI                    0.1279       1.0402       
## year2021_team_BAL                    0.2140       1.1927       
## year2021_team_CAR                    0.0371       0.3063       
## year2021_team_CHI                   -0.1838      -1.4673      .
## year2021_team_GB                     0.1116       0.9019       
## year2021_team_IND                    0.0159       0.1140       
## year2021_team_LAC                    0.0595       0.3990       
## year2021_team_MIA                    0.1213       0.7811       
## year2021_team_NYJ                    0.0240       0.1676       
## year2021_team_PHI                   -0.1552      -1.1922       
## year2021_team_SEA                   -0.1812      -1.1981       
## year2021_team_TB                     0.0238       0.1691       
## year2021_team_WAS                   -0.0321      -0.2586       
## year2021_team_CLE                   -0.0525      -0.4084       
## year2021_team_HOU                   -0.0345      -0.2354       
## year2021_team_JAX                    0.0238       0.1623       
## year2021_team_PIT                    0.0134       0.0986       
## year2022_team_ARI                   -0.0965      -0.7311       
## year2022_team_ATL                   -0.2158      -1.6705      *
## year2022_team_CAR                    0.1660       1.1117       
## year2022_team_CHI                    0.0747       0.4289       
## year2022_team_CIN                   -0.0846      -0.5669       
## year2022_team_HOU                   -0.0178      -0.1256       
## year2022_team_IND                   -0.0899      -0.6745       
## year2022_team_LAC                   -0.1300      -0.9632       
## year2022_team_MIA                   -0.1498      -1.2077       
## year2022_team_SEA                   -0.0091      -0.0674       
## year2022_team_TB                     0.0382       0.2922       
## year2022_team_TEN                    0.2272       1.9487      *
## year2022_team_WAS                    0.0757       0.5815       
## year2022_team_BAL                   -0.1710      -1.1625       
## year2022_team_BUF                    0.0940       0.7026       
## year2022_team_DAL                    0.0419       0.2439       
## year2022_team_DET                   -0.0227      -0.1812       
## year2022_team_GB                    -0.1025      -0.7324       
## year2022_team_JAX                   -0.1510      -1.3056       
## year2022_team_KC                    -0.0698      -0.4150       
## year2022_team_LA                     0.1999       1.4576      .
## year2022_team_LV                     0.1548       1.0846       
## year2022_team_NO                     0.0083       0.0528       
## year2022_team_PHI                    0.0562       0.4337       
## year2022_team_PIT                    0.1731       1.3434       
## year2022_team_DEN                    0.1484       1.2335       
## year2022_team_MIN                   -0.0652      -0.4145       
## year2022_team_NE                     0.0821       0.5801       
## year2022_team_NYJ                   -0.1092      -0.8352       
## year2022_team_NYG                   -0.0540      -0.3849       
## year2022_team_SF                    -0.0571      -0.3199       
## year2023_team_BAL                   -0.0509      -0.3795       
## year2023_team_CHI                   -0.1315      -0.9652       
## year2023_team_CLE                   -0.1750      -1.1481       
## year2023_team_GB                     0.0418       0.3238       
## year2023_team_IND                    0.1255       0.9528       
## year2023_team_KC                    -0.0275      -0.1968       
## year2023_team_LAC                    0.0630       0.4371       
## year2023_team_LV                     0.0341       0.2659       
## year2023_team_MIA                    0.0274       0.2034       
## year2023_team_MIN                    0.2068       1.7489      *
## year2023_team_NO                    -0.0463      -0.3159       
## year2023_team_NYG                    0.1464       1.0491       
## year2023_team_SEA                   -0.2267      -1.8291      *
## year2023_team_SF                     0.0150       0.0966       
## year2023_team_WAS                    0.1858       1.5433      .
## year2023_team_ATL                   -0.0743      -0.4968       
## year2023_team_BUF                   -0.0728      -0.4755       
## year2023_team_CAR                    0.1652       1.2797       
## year2023_team_DAL                    0.1141       0.7609       
## year2023_team_DEN                    0.0166       0.1255       
## year2023_team_HOU                    0.0381       0.2531       
## year2023_team_LA                     0.0782       0.5264       
## year2023_team_NE                     0.1058       0.7823       
## year2023_team_PHI                   -0.0442      -0.3256       
## year2023_team_PIT                    0.0698       0.4309       
## year2023_team_TEN                    0.0372       0.2601       
## year2023_team_ARI                   -0.0787      -0.5589       
## year2023_team_CIN                   -0.0955      -0.6436       
## year2023_team_DET                    0.0630       0.4981       
## year2023_team_TB                     0.1316       0.9454       
## year2023_team_JAX                   -0.0824      -0.5504       
## year2023_team_NYJ                    0.2496       1.7810      *
## is_first_half                       -0.0101      -0.5726       
## time_in_half                         0.0165       1.6925      *
## home_attendance                     -0.0112      -0.1538       
## GIMR                                 0.0476       1.9983     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1159215 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                     10.11
## prev_singleback_rate                                   6.13
## prev_iform_rate                                        5.15
## cover1_rate                                            6.21
## cover3_rate                                            6.54
## starter_OL_grades_pass_block_12w                       6.50
## starter_OL_grades_run_block_12w                        8.19
## home_attendance                                       13.87
## 
## 
##  ================================================================================ 
## MODEL COMPARISON - Adjusted R-squared values
## ================================================================================ 
## 
## Player Model with GIMR: 0.112259 
## Starter Model with GIMR: 0.1159215 
## 
## 
## ==================================================================================================== 
## ANALYZING DATASET 3/8: Offense Tds
## ==================================================================================================== 
## 
## Reading data: processed_predict_ccafd_off_tds.csv.csv.gz
## Reading data: processed_predict_ccfd_off_tds.csv.csv.gz
## 
## Phase 1: Validation Phase
## 
## Running 2 test iterations with best parameters...
## 
## Test Results over 2 iterations:
## Mean AUC: 0.8893453 
## SD AUC: 0.003577065 
## 95% CI: 0.8823343 to 0.8963564 
## 
## 
##  ================================================================================ 
## MODEL: Player Model with GIMR 
## ================================================================================ 
## 
## 
## Player Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.3967       3.1568    ***
## ydstogo                             -0.1117     -12.5817    ***
## posteam_timeouts_remaining           0.0135       1.4690      .
## defteam_timeouts_remaining           0.0088       0.9827       
## rush_attempt                         0.1493       7.6586    ***
## week                                 0.0048       0.4819       
## temp                                -0.0088      -0.8371       
## wind                                 0.0096       0.9114       
## vegas_wp                             0.0166       1.4649      .
## spread_line                         -0.0025      -0.1981       
## total_line                           0.0301       2.3290     **
## prep_days                            0.0062       0.7902       
## overall_win_pct                      0.0138       1.0467       
## team_win_pct                         0.0183       1.2656       
## prev_win_pct                        -0.0336      -2.6441    ***
## prev_shotgun_rate                    0.0183       0.8246       
## prev_singleback_rate                 0.0134       0.7897       
## prev_empty_rate                      0.0138       1.1161       
## prev_iform_rate                      0.0097       0.6183       
## prev_shotgun_success                 0.0040       0.3332       
## prev_singleback_success              0.0079       0.6692       
## prev_empty_success                   0.0052       0.4745       
## prev_iform_success                   0.0188       1.8669      *
## prev_stop_rate_run                   0.0026       0.2239       
## prev_stop_rate_pass                 -0.0356      -3.4518    ***
## shotgun_rate                         0.0165       1.2096       
## singleback_rate                      0.0056       0.4659       
## empty_rate                          -0.0026      -0.2315       
## iform_rate                          -0.0195      -1.8507      *
## shotgun_success                     -0.0205      -2.2706     **
## singleback_success                  -0.0092      -1.0006       
## empty_success                       -0.0095      -0.9801       
## iform_success                       -0.0184      -1.8902      *
## def_stop_rate_run                    0.0159       1.7039      *
## def_stop_rate_pass                  -0.0088      -0.9282       
## avg_pass_rushers                    -0.0100      -0.8968       
## avg_box_defenders                   -0.0055      -0.5257       
## cover0_rate                         -0.0034      -0.2978       
## cover1_rate                         -0.0107      -0.5945       
## cover2_rate                         -0.0035      -0.2636       
## cover3_rate                          0.0271       1.4740      .
## cover4_rate                          0.0133       0.9869       
## cover6_rate                         -0.0059      -0.4841       
## two_man_rate                         0.0139       1.4779      .
## prevent_rate                         0.0204       2.5480     **
## roof_outdoors                       -0.0024      -0.0999       
## posteam_type_home                   -0.0235      -1.4995      .
## QB_short_touchdowns_12w              0.0041       0.4170       
## QB_medium_touchdowns_12w             0.0007       0.0707       
## QB_deep_touchdowns_12w              -0.0141      -1.5104      .
## RB_grades_pass_block_12w             0.0141       1.7952      *
## RB_touchdowns_12w                    0.0033       0.4172       
## RB_short_touchdowns_12w             -0.0105      -1.3066       
## RB_medium_touchdowns_12w            -0.0037      -0.5687       
## WR1_grades_pass_block_12w           -0.0060      -0.7354       
## WR1_touchdowns_12w                  -0.0120      -1.4671      .
## WR1_short_touchdowns_12w            -0.0089      -1.0016       
## WR1_medium_touchdowns_12w            0.0044       0.5034       
## WR2_grades_pass_block_12w           -0.0054      -0.6597       
## WR2_touchdowns_12w                  -0.0165      -2.1122     **
## WR2_short_touchdowns_12w            -0.0083      -0.9792       
## WR2_medium_touchdowns_12w            0.0087       1.0831       
## WR3_touchdowns_12w                   0.0036       0.4673       
## WR3_short_touchdowns_12w             0.0018       0.2281       
## WR3_medium_touchdowns_12w            0.0069       0.8383       
## TE1_grades_pass_block_12w            0.0261       2.4820     **
## TE1_grades_run_block_12w            -0.0107      -0.9957       
## TE1_short_touchdowns_12w            -0.0019      -0.2243       
## TE1_medium_touchdowns_12w            0.0014       0.1724       
## DL1_grades_defense_12w              -0.0154      -1.8882      *
## DL2_grades_defense_12w               0.0037       0.4328       
## DL3_grades_defense_12w               0.0112       0.9650       
## DL4_grades_defense_12w              -0.0294      -2.4691     **
## LB1_grades_defense_12w               0.0048       0.5630       
## LB2_grades_defense_12w               0.0025       0.2876       
## LB3_grades_defense_12w              -0.0178      -1.5245      .
## LB4_grades_defense_12w              -0.0011      -0.1004       
## CB1_grades_defense_12w              -0.0175      -2.0728     **
## CB2_grades_defense_12w              -0.0066      -0.7188       
## CB3_grades_defense_12w               0.0199       1.9553      *
## S1_grades_defense_12w               -0.0078      -1.0118       
## S2_grades_defense_12w                0.0056       0.6298       
## S3_grades_defense_12w                0.0106       1.1000       
## OL_grades_pass_block_12w            -0.0029      -0.2731       
## OL_grades_run_block_12w             -0.0031      -0.2983       
## yardline_1_10                       -0.0588      -2.2141     **
## yardline_11_20                       0.0176       0.6037       
## yardline_21_30                       0.0055       0.1933       
## yardline_41_50                       0.0480       1.9838     **
## yardline_51_60                       0.0215       0.7406       
## yardline_61_70                       0.0539       1.6485      *
## yardline_71_80                       0.0749       1.8713      *
## yardline_81_90                       0.1436       2.3711     **
## yardline_91_100                      0.0996       0.9537       
## year2017_team_ARI                    0.0666       0.3513       
## year2017_team_BUF                   -0.1288      -0.6658       
## year2017_team_CHI                    0.0224       0.1285       
## year2017_team_CLE                    0.1759       0.8983       
## year2017_team_DAL                   -0.1604      -0.9326       
## year2017_team_DET                   -0.0355      -0.2049       
## year2017_team_GB                     0.3469       2.1226     **
## year2017_team_HOU                    0.3378       1.6396      .
## year2017_team_MIA                   -0.1951      -1.1029       
## year2017_team_MIN                   -0.1063      -0.5949       
## year2017_team_NE                    -0.0269      -0.1463       
## year2017_team_SF                     0.3867       2.0004     **
## year2017_team_BAL                    0.0341       0.1756       
## year2017_team_DEN                   -0.0213      -0.1164       
## year2017_team_LA                     0.0682       0.3759       
## year2017_team_NYG                   -0.0516      -0.3038       
## year2017_team_OAK                   -0.1098      -0.6086       
## year2017_team_SEA                    0.1363       0.7368       
## year2017_team_CAR                    0.1119       0.5185       
## year2017_team_CIN                    0.1585       0.7892       
## year2017_team_IND                    0.1703       0.9314       
## year2017_team_NO                     0.0865       0.3802       
## year2017_team_PHI                    0.0406       0.2250       
## year2017_team_PIT                   -0.1302      -0.7750       
## year2017_team_TEN                    0.1024       0.4771       
## year2017_team_WAS                    0.0455       0.2364       
## year2017_team_KC                     0.2751       1.4568      .
## year2017_team_LAC                   -0.0132      -0.0721       
## year2017_team_NYJ                    0.1495       0.6967       
## year2017_team_TB                     0.0467       0.2047       
## year2017_team_ATL                   -0.0344      -0.1768       
## year2017_team_JAX                    0.0850       0.4354       
## year2018_team_ARI                    0.0899       0.6199       
## year2018_team_BAL                    0.0819       0.5563       
## year2018_team_CAR                    0.0728       0.5017       
## year2018_team_CLE                   -0.0132      -0.0948       
## year2018_team_DET                    0.1311       0.9224       
## year2018_team_HOU                    0.2385       1.4239       
## year2018_team_IND                   -0.1008      -0.7450       
## year2018_team_KC                     0.1356       0.9836       
## year2018_team_NYG                    0.1324       0.7494       
## year2018_team_OAK                   -0.1246      -0.7278       
## year2018_team_PHI                    0.1042       0.7135       
## year2018_team_SEA                   -0.0447      -0.2558       
## year2018_team_BUF                   -0.0872      -0.5515       
## year2018_team_CHI                    0.0140       0.1079       
## year2018_team_CIN                   -0.0230      -0.1344       
## year2018_team_DAL                   -0.0122      -0.0830       
## year2018_team_DEN                    0.0674       0.4691       
## year2018_team_GB                     0.0163       0.0967       
## year2018_team_LAC                    0.0369       0.2491       
## year2018_team_NE                    -0.0741      -0.4731       
## year2018_team_NO                     0.1030       0.7557       
## year2018_team_PIT                    0.0905       0.4751       
## year2018_team_SF                     0.0509       0.3329       
## year2018_team_MIA                    0.1036       0.7296       
## year2018_team_MIN                    0.0514       0.3194       
## year2018_team_NYJ                    0.1828       0.8306       
## year2018_team_TB                     0.0808       0.4825       
## year2018_team_ATL                    0.0547       0.3967       
## year2018_team_JAX                    0.0690       0.4504       
## year2018_team_LA                    -0.1419      -0.8788       
## year2018_team_TEN                    0.1335       0.8458       
## year2018_team_WAS                    0.1314       0.6530       
## year2019_team_ARI                   -0.0639      -0.4077       
## year2019_team_BUF                   -0.1177      -0.9148       
## year2019_team_CHI                    0.1228       0.8357       
## year2019_team_CLE                    0.1183       0.8155       
## year2019_team_DAL                   -0.0084      -0.0510       
## year2019_team_IND                   -0.0542      -0.4079       
## year2019_team_JAX                    0.1226       0.8146       
## year2019_team_KC                     0.0227       0.1670       
## year2019_team_LAC                   -0.0815      -0.5528       
## year2019_team_MIN                   -0.0411      -0.2813       
## year2019_team_NE                    -0.0004      -0.0022       
## year2019_team_NO                    -0.1920      -1.2601       
## year2019_team_PHI                    0.0916       0.6124       
## year2019_team_SEA                    0.0526       0.2650       
## year2019_team_SF                     0.0249       0.1859       
## year2019_team_TB                    -0.0964      -0.6861       
## year2019_team_BAL                    0.0561       0.3970       
## year2019_team_CAR                   -0.0813      -0.4980       
## year2019_team_DEN                    0.1652       1.1609       
## year2019_team_DET                   -0.0803      -0.5311       
## year2019_team_HOU                    0.0206       0.1378       
## year2019_team_LA                    -0.0737      -0.4672       
## year2019_team_MIA                   -0.3154      -2.0245     **
## year2019_team_NYG                   -0.1297      -0.8104       
## year2019_team_NYJ                   -0.1719      -1.2975       
## year2019_team_OAK                   -0.0320      -0.2144       
## year2019_team_PIT                   -0.2723      -2.1793     **
## year2019_team_TEN                   -0.1604      -1.1341       
## year2019_team_CIN                    0.0824       0.5716       
## year2019_team_WAS                   -0.0339      -0.2273       
## year2019_team_ATL                    0.0164       0.1045       
## year2019_team_GB                    -0.0505      -0.3412       
## year2020_team_ATL                    0.0757       0.4909       
## year2020_team_BAL                    0.0921       0.5977       
## year2020_team_BUF                   -0.0128      -0.0688       
## year2020_team_CAR                    0.1317       0.8160       
## year2020_team_CIN                    0.1347       0.8869       
## year2020_team_DEN                   -0.0738      -0.4418       
## year2020_team_DET                   -0.1136      -0.7314       
## year2020_team_JAX                   -0.0970      -0.6122       
## year2020_team_KC                     0.0865       0.5340       
## year2020_team_LA                    -0.1572      -0.8972       
## year2020_team_MIN                    0.1959       1.3706       
## year2020_team_NE                    -0.0138      -0.0899       
## year2020_team_NO                     0.0620       0.4279       
## year2020_team_NYG                    0.0502       0.3310       
## year2020_team_SF                     0.1469       0.8724       
## year2020_team_WAS                    0.0418       0.2918       
## year2020_team_CHI                    0.0743       0.4618       
## year2020_team_DAL                   -0.0139      -0.0927       
## year2020_team_GB                     0.0097       0.0541       
## year2020_team_HOU                   -0.0868      -0.5383       
## year2020_team_MIA                   -0.1200      -0.7505       
## year2020_team_NYJ                   -0.0008      -0.0051       
## year2020_team_TB                     0.0740       0.4526       
## year2020_team_TEN                   -0.0583      -0.3557       
## year2020_team_ARI                    0.0903       0.5430       
## year2020_team_CLE                   -0.2226      -1.2802       
## year2020_team_IND                   -0.1227      -0.7450       
## year2020_team_LAC                    0.0287       0.1580       
## year2020_team_PHI                    0.1353       0.9235       
## year2020_team_SEA                   -0.0097      -0.0597       
## year2020_team_LV                     0.1270       0.8017       
## year2020_team_PIT                   -0.0936      -0.5736       
## year2021_team_ATL                   -0.2124      -1.6824      *
## year2021_team_BUF                    0.0825       0.6537       
## year2021_team_CIN                   -0.1946      -1.6109      .
## year2021_team_DAL                   -0.0986      -0.7140       
## year2021_team_DEN                    0.0924       0.6796       
## year2021_team_DET                   -0.0556      -0.4144       
## year2021_team_KC                     0.0315       0.2514       
## year2021_team_LA                     0.0365       0.2689       
## year2021_team_LV                     0.0496       0.3336       
## year2021_team_MIN                   -0.0255      -0.1974       
## year2021_team_NE                     0.0787       0.5759       
## year2021_team_NO                     0.0102       0.0756       
## year2021_team_NYG                    0.0061       0.0460       
## year2021_team_SF                     0.0160       0.1152       
## year2021_team_TEN                   -0.0373      -0.3035       
## year2021_team_ARI                    0.0925       0.7680       
## year2021_team_BAL                    0.1736       0.9687       
## year2021_team_CAR                   -0.0800      -0.6772       
## year2021_team_CHI                   -0.1968      -1.5725      .
## year2021_team_GB                     0.1144       0.9351       
## year2021_team_IND                   -0.0270      -0.2008       
## year2021_team_LAC                    0.0817       0.5624       
## year2021_team_MIA                    0.0544       0.3522       
## year2021_team_NYJ                   -0.0113      -0.0748       
## year2021_team_PHI                   -0.1664      -1.3153       
## year2021_team_SEA                   -0.1719      -1.1505       
## year2021_team_TB                     0.1039       0.7443       
## year2021_team_WAS                   -0.0488      -0.3915       
## year2021_team_CLE                   -0.0760      -0.5941       
## year2021_team_HOU                   -0.0789      -0.5447       
## year2021_team_JAX                   -0.0226      -0.1535       
## year2021_team_PIT                    0.0751       0.5745       
## year2022_team_ARI                   -0.1464      -1.1440       
## year2022_team_ATL                   -0.2701      -2.0299     **
## year2022_team_CAR                    0.1383       0.9333       
## year2022_team_CHI                   -0.0652      -0.4072       
## year2022_team_CIN                   -0.1061      -0.7208       
## year2022_team_HOU                   -0.0317      -0.2296       
## year2022_team_IND                   -0.0917      -0.6883       
## year2022_team_LAC                   -0.0371      -0.2782       
## year2022_team_MIA                   -0.1579      -1.2842       
## year2022_team_SEA                   -0.0335      -0.2522       
## year2022_team_TB                     0.0434       0.3378       
## year2022_team_TEN                    0.1851       1.5823      .
## year2022_team_WAS                    0.0194       0.1480       
## year2022_team_BAL                   -0.1649      -1.1471       
## year2022_team_BUF                    0.0432       0.3348       
## year2022_team_DAL                    0.0071       0.0430       
## year2022_team_DET                   -0.0639      -0.5067       
## year2022_team_GB                    -0.0838      -0.5953       
## year2022_team_JAX                   -0.1354      -1.2011       
## year2022_team_KC                    -0.1087      -0.6311       
## year2022_team_LA                     0.2208       1.6329      .
## year2022_team_LV                     0.1780       1.2356       
## year2022_team_NO                    -0.0413      -0.2676       
## year2022_team_PHI                    0.0724       0.5641       
## year2022_team_PIT                    0.2272       1.8020      *
## year2022_team_DEN                    0.0498       0.4082       
## year2022_team_MIN                   -0.0836      -0.5348       
## year2022_team_NE                     0.0300       0.2074       
## year2022_team_NYJ                   -0.0826      -0.6332       
## year2022_team_NYG                   -0.0512      -0.3563       
## year2022_team_SF                    -0.1615      -0.9572       
## year2023_team_BAL                   -0.0282      -0.2161       
## year2023_team_CHI                   -0.1260      -0.9085       
## year2023_team_CLE                   -0.1205      -0.8083       
## year2023_team_GB                     0.0435       0.3246       
## year2023_team_IND                    0.0983       0.7782       
## year2023_team_KC                     0.0565       0.4042       
## year2023_team_LAC                    0.0629       0.4470       
## year2023_team_LV                     0.0109       0.0878       
## year2023_team_MIA                    0.0745       0.5622       
## year2023_team_MIN                    0.1657       1.3812       
## year2023_team_NO                    -0.0354      -0.2493       
## year2023_team_NYG                    0.0836       0.6224       
## year2023_team_SEA                   -0.2781      -2.2742     **
## year2023_team_SF                     0.0708       0.4586       
## year2023_team_WAS                    0.2073       1.6447      .
## year2023_team_ATL                   -0.0928      -0.6353       
## year2023_team_BUF                   -0.0752      -0.5000       
## year2023_team_CAR                    0.0966       0.7645       
## year2023_team_DAL                    0.0957       0.6756       
## year2023_team_DEN                    0.0203       0.1579       
## year2023_team_HOU                   -0.0164      -0.1078       
## year2023_team_LA                     0.0174       0.1175       
## year2023_team_NE                     0.0515       0.3870       
## year2023_team_PHI                   -0.0263      -0.2010       
## year2023_team_PIT                    0.0183       0.1166       
## year2023_team_TEN                    0.0290       0.1950       
## year2023_team_ARI                   -0.1417      -0.9981       
## year2023_team_CIN                   -0.1297      -0.8567       
## year2023_team_DET                    0.0611       0.4942       
## year2023_team_TB                     0.1449       1.0665       
## year2023_team_JAX                   -0.0617      -0.4131       
## year2023_team_NYJ                    0.2104       1.5399      .
## is_first_half                       -0.0079      -0.4423       
## time_in_half                         0.0165       1.6732      *
## home_attendance                     -0.0251      -0.3352       
## GIMR                                 0.0557       2.3935     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1117194 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.50
## prev_singleback_rate                                   5.59
## cover1_rate                                            6.14
## cover3_rate                                            6.49
## home_attendance                                       13.67
## 
## 
##  ================================================================================ 
## MODEL: Starter Model with GIMR 
## ================================================================================ 
## 
## 
## Starter Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.4029       3.2380    ***
## ydstogo                             -0.1094     -12.5627    ***
## posteam_timeouts_remaining           0.0115       1.2600       
## defteam_timeouts_remaining           0.0085       0.9522       
## rush_attempt                         0.1382       7.3141    ***
## week                                 0.0058       0.5753       
## temp                                -0.0067      -0.6292       
## wind                                 0.0082       0.7675       
## vegas_wp                             0.0092       0.8350       
## spread_line                         -0.0103      -0.8337       
## total_line                           0.0379       2.8614    ***
## prep_days                            0.0080       1.0275       
## overall_win_pct                      0.0090       0.6774       
## team_win_pct                         0.0255       1.7712      *
## prev_win_pct                        -0.0292      -2.2733     **
## prev_shotgun_rate                    0.0132       0.5882       
## prev_singleback_rate                 0.0132       0.7667       
## prev_empty_rate                      0.0126       1.0152       
## prev_iform_rate                      0.0049       0.3048       
## prev_shotgun_success                 0.0051       0.4303       
## prev_singleback_success              0.0039       0.3213       
## prev_empty_success                  -0.0006      -0.0501       
## prev_iform_success                   0.0257       2.5320     **
## prev_stop_rate_run                  -0.0004      -0.0337       
## prev_stop_rate_pass                 -0.0330      -3.2308    ***
## shotgun_rate                         0.0137       0.9921       
## singleback_rate                      0.0075       0.6218       
## empty_rate                           0.0005       0.0456       
## iform_rate                          -0.0196      -1.8541      *
## shotgun_success                     -0.0198      -2.1809     **
## singleback_success                  -0.0120      -1.2892       
## empty_success                       -0.0076      -0.7710       
## iform_success                       -0.0187      -1.9146      *
## def_stop_rate_run                    0.0160       1.7156      *
## def_stop_rate_pass                  -0.0071      -0.7425       
## avg_pass_rushers                    -0.0110      -0.9972       
## avg_box_defenders                   -0.0055      -0.5300       
## cover0_rate                         -0.0057      -0.5005       
## cover1_rate                         -0.0114      -0.6325       
## cover2_rate                         -0.0055      -0.4197       
## cover3_rate                          0.0159       0.8626       
## cover4_rate                          0.0099       0.7381       
## cover6_rate                         -0.0096      -0.7901       
## two_man_rate                         0.0139       1.4835      .
## prevent_rate                         0.0205       2.4804     **
## roof_outdoors                        0.0035       0.1451       
## posteam_type_home                   -0.0211      -1.3389       
## starter_QB_short_touchdowns_12w       0.0322       3.0508    ***
## starter_QB_medium_touchdowns_12w      -0.0143      -1.3135       
## starter_QB_deep_touchdowns_12w      -0.0142      -1.5054      .
## starter_RB_grades_pass_block_12w      -0.0116      -1.2596       
## starter_RB_touchdowns_12w           -0.0048      -0.5556       
## starter_RB_short_touchdowns_12w      -0.0145      -1.6241      .
## starter_RB_medium_touchdowns_12w      -0.0082      -1.0217       
## starter_WR1_grades_pass_block_12w      -0.0006      -0.0764       
## starter_WR1_touchdowns_12w          -0.0145      -1.7575      *
## starter_WR1_short_touchdowns_12w      -0.0156      -1.7722      *
## starter_WR1_medium_touchdowns_12w       0.0146       1.6339      .
## starter_WR2_grades_pass_block_12w      -0.0039      -0.4707       
## starter_WR2_touchdowns_12w          -0.0107      -1.3293       
## starter_WR2_short_touchdowns_12w      -0.0240      -2.8578    ***
## starter_WR2_medium_touchdowns_12w       0.0037       0.4094       
## starter_WR3_grades_pass_block_12w      -0.0090      -1.0768       
## starter_WR3_touchdowns_12w          -0.0038      -0.4862       
## starter_WR3_short_touchdowns_12w      -0.0228      -2.6315    ***
## starter_WR3_medium_touchdowns_12w      -0.0035      -0.4158       
## starter_TE1_grades_pass_block_12w       0.0205       1.8920      *
## starter_TE1_grades_run_block_12w      -0.0168      -1.2808       
## starter_TE1_short_touchdowns_12w      -0.0133      -1.4368       
## starter_TE1_medium_touchdowns_12w       0.0027       0.3064       
## starter_DL1_grades_defense_12w       0.0068       0.6000       
## starter_DL2_grades_defense_12w       0.0133       1.1683       
## starter_DL3_grades_defense_12w       0.0021       0.1824       
## starter_DL4_grades_defense_12w       0.0075       0.7752       
## starter_LB1_grades_defense_12w       0.0047       0.4196       
## starter_LB2_grades_defense_12w       0.0190       1.6980      *
## starter_LB3_grades_defense_12w       0.0114       1.1464       
## starter_LB4_grades_defense_12w      -0.0252      -2.9342    ***
## starter_CB1_grades_defense_12w      -0.0075      -0.5953       
## starter_CB2_grades_defense_12w       0.0006       0.0503       
## starter_CB3_grades_defense_12w      -0.0075      -0.7967       
## starter_S1_grades_defense_12w       -0.0023      -0.1958       
## starter_S2_grades_defense_12w       -0.0091      -0.8121       
## starter_S3_grades_defense_12w       -0.0053      -0.6210       
## starter_OL_grades_pass_block_12w       0.0448       2.4976     **
## starter_OL_grades_run_block_12w      -0.0303      -1.5272      .
## yardline_1_10                       -0.0558      -2.1519     **
## yardline_11_20                       0.0051       0.1753       
## yardline_21_30                       0.0011       0.0401       
## yardline_41_50                       0.0467       1.9413      *
## yardline_51_60                       0.0188       0.6483       
## yardline_61_70                       0.0521       1.5982      .
## yardline_71_80                       0.0723       1.7840      *
## yardline_81_90                       0.1264       2.1233     **
## yardline_91_100                      0.1313       1.2253       
## year2017_team_ARI                    0.0609       0.3213       
## year2017_team_BUF                   -0.1464      -0.7641       
## year2017_team_CHI                   -0.0327      -0.1890       
## year2017_team_CLE                    0.0724       0.3671       
## year2017_team_DAL                   -0.2079      -1.2010       
## year2017_team_DET                   -0.0917      -0.5377       
## year2017_team_GB                     0.3209       1.9308      *
## year2017_team_HOU                    0.3665       1.7122      *
## year2017_team_MIA                   -0.2014      -1.1330       
## year2017_team_MIN                   -0.1708      -0.9581       
## year2017_team_NE                    -0.0794      -0.4264       
## year2017_team_SF                     0.3171       1.6055      .
## year2017_team_BAL                    0.0256       0.1327       
## year2017_team_DEN                   -0.0084      -0.0457       
## year2017_team_LA                     0.0429       0.2311       
## year2017_team_NYG                   -0.0626      -0.3663       
## year2017_team_OAK                   -0.0521      -0.2793       
## year2017_team_SEA                    0.0836       0.4454       
## year2017_team_CAR                   -0.0441      -0.1962       
## year2017_team_CIN                    0.0544       0.2694       
## year2017_team_IND                    0.1718       0.9346       
## year2017_team_NO                    -0.0122      -0.0577       
## year2017_team_PHI                   -0.0202      -0.1104       
## year2017_team_PIT                   -0.2003      -1.2128       
## year2017_team_TEN                   -0.0028      -0.0128       
## year2017_team_WAS                   -0.0041      -0.0218       
## year2017_team_KC                     0.2326       1.1795       
## year2017_team_LAC                   -0.0315      -0.1615       
## year2017_team_NYJ                    0.1156       0.5430       
## year2017_team_TB                     0.0133       0.0563       
## year2017_team_ATL                   -0.0380      -0.2007       
## year2017_team_JAX                    0.0657       0.3262       
## year2018_team_ARI                    0.1610       1.0985       
## year2018_team_BAL                    0.0579       0.3921       
## year2018_team_CAR                    0.0518       0.3429       
## year2018_team_CLE                    0.0032       0.0232       
## year2018_team_DET                    0.1047       0.7251       
## year2018_team_HOU                    0.1547       0.9441       
## year2018_team_IND                   -0.1183      -0.8551       
## year2018_team_KC                     0.0983       0.6779       
## year2018_team_NYG                    0.1261       0.7356       
## year2018_team_OAK                   -0.0283      -0.1660       
## year2018_team_PHI                    0.0513       0.3491       
## year2018_team_SEA                   -0.0388      -0.2218       
## year2018_team_BUF                   -0.0741      -0.4622       
## year2018_team_CHI                   -0.0130      -0.0984       
## year2018_team_CIN                   -0.0546      -0.3331       
## year2018_team_DAL                   -0.0071      -0.0469       
## year2018_team_DEN                    0.0465       0.3090       
## year2018_team_GB                    -0.0033      -0.0191       
## year2018_team_LAC                    0.0869       0.6043       
## year2018_team_NE                    -0.1552      -0.9993       
## year2018_team_NO                     0.0899       0.6444       
## year2018_team_PIT                    0.0205       0.1041       
## year2018_team_SF                     0.0849       0.5453       
## year2018_team_MIA                    0.0791       0.5667       
## year2018_team_MIN                    0.0738       0.4719       
## year2018_team_NYJ                    0.1371       0.6448       
## year2018_team_TB                     0.0617       0.3741       
## year2018_team_ATL                    0.0540       0.3812       
## year2018_team_JAX                   -0.0094      -0.0614       
## year2018_team_LA                    -0.1119      -0.7106       
## year2018_team_TEN                    0.1372       0.8248       
## year2018_team_WAS                    0.0779       0.3876       
## year2019_team_ARI                   -0.1085      -0.7199       
## year2019_team_BUF                   -0.1278      -1.0124       
## year2019_team_CHI                    0.1436       0.9769       
## year2019_team_CLE                    0.1345       0.8770       
## year2019_team_DAL                   -0.0175      -0.1040       
## year2019_team_IND                   -0.0515      -0.3881       
## year2019_team_JAX                    0.1364       0.8851       
## year2019_team_KC                     0.0236       0.1719       
## year2019_team_LAC                   -0.0653      -0.4728       
## year2019_team_MIN                   -0.0385      -0.2669       
## year2019_team_NE                    -0.0109      -0.0655       
## year2019_team_NO                    -0.1777      -1.1743       
## year2019_team_PHI                    0.0842       0.5632       
## year2019_team_SEA                    0.0414       0.2155       
## year2019_team_SF                    -0.0080      -0.0597       
## year2019_team_TB                    -0.1097      -0.8113       
## year2019_team_BAL                    0.0516       0.3689       
## year2019_team_CAR                   -0.1083      -0.6577       
## year2019_team_DEN                    0.1202       0.8086       
## year2019_team_DET                   -0.0453      -0.3003       
## year2019_team_HOU                   -0.0329      -0.2234       
## year2019_team_LA                    -0.1475      -0.8767       
## year2019_team_MIA                   -0.3216      -2.0406     **
## year2019_team_NYG                   -0.1416      -0.8973       
## year2019_team_NYJ                   -0.1944      -1.5135      .
## year2019_team_OAK                    0.0243       0.1556       
## year2019_team_PIT                   -0.3790      -3.1246    ***
## year2019_team_TEN                   -0.1253      -0.8959       
## year2019_team_CIN                    0.1267       0.8270       
## year2019_team_WAS                   -0.0281      -0.1834       
## year2019_team_ATL                   -0.0015      -0.0096       
## year2019_team_GB                    -0.0689      -0.4554       
## year2020_team_ATL                    0.0895       0.5796       
## year2020_team_BAL                    0.0555       0.3654       
## year2020_team_BUF                    0.0270       0.1458       
## year2020_team_CAR                    0.1766       1.0537       
## year2020_team_CIN                    0.1414       0.9469       
## year2020_team_DEN                   -0.0579      -0.3431       
## year2020_team_DET                   -0.0838      -0.5450       
## year2020_team_JAX                   -0.0778      -0.4881       
## year2020_team_KC                     0.0582       0.3494       
## year2020_team_LA                    -0.1591      -0.9039       
## year2020_team_MIN                    0.2031       1.4479      .
## year2020_team_NE                     0.0102       0.0665       
## year2020_team_NO                     0.0574       0.3904       
## year2020_team_NYG                    0.0550       0.3603       
## year2020_team_SF                     0.1350       0.7875       
## year2020_team_WAS                    0.0370       0.2500       
## year2020_team_CHI                    0.1411       0.9021       
## year2020_team_DAL                    0.0253       0.1706       
## year2020_team_GB                     0.0072       0.0408       
## year2020_team_HOU                   -0.1319      -0.8253       
## year2020_team_MIA                   -0.0995      -0.6101       
## year2020_team_NYJ                    0.0572       0.3379       
## year2020_team_TB                     0.0741       0.4677       
## year2020_team_TEN                   -0.0463      -0.2792       
## year2020_team_ARI                    0.1270       0.7823       
## year2020_team_CLE                   -0.2087      -1.1695       
## year2020_team_IND                   -0.1773      -1.0660       
## year2020_team_LAC                    0.0588       0.3330       
## year2020_team_PHI                    0.1657       1.1343       
## year2020_team_SEA                   -0.0254      -0.1580       
## year2020_team_LV                     0.1164       0.7506       
## year2020_team_PIT                   -0.1399      -0.8593       
## year2021_team_ATL                   -0.1856      -1.4169       
## year2021_team_BUF                    0.0875       0.6979       
## year2021_team_CIN                   -0.1480      -1.1605       
## year2021_team_DAL                   -0.0815      -0.5898       
## year2021_team_DEN                    0.1008       0.7853       
## year2021_team_DET                   -0.1016      -0.7368       
## year2021_team_KC                     0.0754       0.6014       
## year2021_team_LA                     0.0097       0.0728       
## year2021_team_LV                     0.0888       0.6132       
## year2021_team_MIN                   -0.0227      -0.1687       
## year2021_team_NE                     0.0998       0.7364       
## year2021_team_NO                     0.0182       0.1331       
## year2021_team_NYG                    0.1044       0.7856       
## year2021_team_SF                     0.0413       0.2964       
## year2021_team_TEN                    0.0202       0.1618       
## year2021_team_ARI                    0.1329       1.1023       
## year2021_team_BAL                    0.2330       1.3198       
## year2021_team_CAR                   -0.0038      -0.0315       
## year2021_team_CHI                   -0.1487      -1.1759       
## year2021_team_GB                     0.1143       0.9334       
## year2021_team_IND                   -0.0070      -0.0513       
## year2021_team_LAC                    0.0793       0.5449       
## year2021_team_MIA                    0.1261       0.8145       
## year2021_team_NYJ                    0.0132       0.0916       
## year2021_team_PHI                   -0.1536      -1.1889       
## year2021_team_SEA                   -0.1445      -0.9526       
## year2021_team_TB                     0.0583       0.4165       
## year2021_team_WAS                   -0.0661      -0.5308       
## year2021_team_CLE                   -0.0448      -0.3474       
## year2021_team_HOU                   -0.0519      -0.3633       
## year2021_team_JAX                    0.0401       0.2777       
## year2021_team_PIT                    0.0392       0.2966       
## year2022_team_ARI                   -0.1376      -1.0513       
## year2022_team_ATL                   -0.1967      -1.5001      .
## year2022_team_CAR                    0.0944       0.6282       
## year2022_team_CHI                    0.0109       0.0656       
## year2022_team_CIN                   -0.0814      -0.5528       
## year2022_team_HOU                   -0.0153      -0.1099       
## year2022_team_IND                   -0.0835      -0.6360       
## year2022_team_LAC                   -0.0951      -0.7178       
## year2022_team_MIA                   -0.1296      -1.0446       
## year2022_team_SEA                    0.0224       0.1636       
## year2022_team_TB                     0.0499       0.3867       
## year2022_team_TEN                    0.2135       1.8544      *
## year2022_team_WAS                    0.0787       0.6050       
## year2022_team_BAL                   -0.1810      -1.2262       
## year2022_team_BUF                    0.0856       0.6491       
## year2022_team_DAL                    0.0065       0.0390       
## year2022_team_DET                    0.0168       0.1324       
## year2022_team_GB                    -0.0651      -0.4700       
## year2022_team_JAX                   -0.1357      -1.1883       
## year2022_team_KC                    -0.1451      -0.8836       
## year2022_team_LA                     0.1822       1.3720       
## year2022_team_LV                     0.1937       1.3155       
## year2022_team_NO                    -0.0289      -0.1806       
## year2022_team_PHI                    0.0671       0.5180       
## year2022_team_PIT                    0.1843       1.4316       
## year2022_team_DEN                    0.1029       0.8658       
## year2022_team_MIN                   -0.0550      -0.3512       
## year2022_team_NE                     0.0410       0.2890       
## year2022_team_NYJ                   -0.0838      -0.6451       
## year2022_team_NYG                   -0.0315      -0.2222       
## year2022_team_SF                    -0.1142      -0.7324       
## year2023_team_BAL                   -0.0341      -0.2565       
## year2023_team_CHI                   -0.0713      -0.5049       
## year2023_team_CLE                   -0.1538      -1.0019       
## year2023_team_GB                     0.0211       0.1620       
## year2023_team_IND                    0.1087       0.8366       
## year2023_team_KC                     0.0053       0.0378       
## year2023_team_LAC                    0.1096       0.7667       
## year2023_team_LV                     0.0235       0.1890       
## year2023_team_MIA                    0.0639       0.4836       
## year2023_team_MIN                    0.2160       1.8273      *
## year2023_team_NO                    -0.0710      -0.4882       
## year2023_team_NYG                    0.0979       0.7020       
## year2023_team_SEA                   -0.2298      -1.8676      *
## year2023_team_SF                     0.0552       0.3524       
## year2023_team_WAS                    0.2357       1.9420      *
## year2023_team_ATL                   -0.0656      -0.4465       
## year2023_team_BUF                   -0.0602      -0.3882       
## year2023_team_CAR                    0.1625       1.2438       
## year2023_team_DAL                    0.1009       0.6761       
## year2023_team_DEN                   -0.0007      -0.0051       
## year2023_team_HOU                    0.0097       0.0654       
## year2023_team_LA                     0.0570       0.3884       
## year2023_team_NE                     0.0885       0.6443       
## year2023_team_PHI                   -0.0381      -0.2897       
## year2023_team_PIT                    0.0385       0.2512       
## year2023_team_TEN                    0.0509       0.3482       
## year2023_team_ARI                   -0.0696      -0.4894       
## year2023_team_CIN                   -0.0539      -0.3663       
## year2023_team_DET                    0.0893       0.7050       
## year2023_team_TB                     0.1517       1.0832       
## year2023_team_JAX                   -0.0749      -0.5001       
## year2023_team_NYJ                    0.2402       1.7094      *
## is_first_half                       -0.0074      -0.4173       
## time_in_half                         0.0158       1.6126      .
## home_attendance                     -0.0219      -0.2964       
## GIMR                                 0.0478       2.0890     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1140666 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                     10.02
## prev_singleback_rate                                   5.95
## prev_iform_rate                                        5.03
## cover1_rate                                            6.26
## cover3_rate                                            6.52
## starter_OL_grades_pass_block_12w                       6.26
## starter_OL_grades_run_block_12w                        7.81
## home_attendance                                       13.73
## 
## 
##  ================================================================================ 
## MODEL COMPARISON - Adjusted R-squared values
## ================================================================================ 
## 
## Player Model with GIMR: 0.1117194 
## Starter Model with GIMR: 0.1140666 
## 
## 
## ==================================================================================================== 
## ANALYZING DATASET 4/8: Offense First Downs
## ==================================================================================================== 
## 
## Reading data: processed_predict_ccafd_off_first_downs.csv.csv.gz
## Reading data: processed_predict_ccfd_off_first_downs.csv.csv.gz
## 
## Phase 1: Validation Phase
## 
## Running 2 test iterations with best parameters...
## 
## Test Results over 2 iterations:
## Mean AUC: 0.8914674 
## SD AUC: 0.00920124 
## 95% CI: 0.873433 to 0.9095019 
## 
## 
##  ================================================================================ 
## MODEL: Player Model with GIMR 
## ================================================================================ 
## 
## 
## Player Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.4137       3.2722    ***
## ydstogo                             -0.1122     -12.5706    ***
## posteam_timeouts_remaining           0.0126       1.3644       
## defteam_timeouts_remaining           0.0086       0.9651       
## rush_attempt                         0.1512       7.6982    ***
## week                                 0.0046       0.4642       
## temp                                -0.0095      -0.9029       
## wind                                 0.0096       0.9114       
## vegas_wp                             0.0177       1.5461      .
## spread_line                         -0.0032      -0.2583       
## total_line                           0.0297       2.2978     **
## prep_days                            0.0058       0.7454       
## overall_win_pct                      0.0139       1.0510       
## team_win_pct                         0.0170       1.1822       
## prev_win_pct                        -0.0336      -2.6485    ***
## prev_shotgun_rate                    0.0161       0.7281       
## prev_singleback_rate                 0.0116       0.6941       
## prev_empty_rate                      0.0113       0.9157       
## prev_iform_rate                      0.0058       0.3695       
## prev_shotgun_success                 0.0034       0.2814       
## prev_singleback_success              0.0076       0.6430       
## prev_empty_success                   0.0055       0.4933       
## prev_iform_success                   0.0203       2.0161     **
## prev_stop_rate_run                   0.0011       0.0945       
## prev_stop_rate_pass                 -0.0346      -3.3468    ***
## shotgun_rate                         0.0153       1.1214       
## singleback_rate                      0.0057       0.4714       
## empty_rate                          -0.0036      -0.3194       
## iform_rate                          -0.0188      -1.7751      *
## shotgun_success                     -0.0198      -2.1975     **
## singleback_success                  -0.0092      -1.0018       
## empty_success                       -0.0082      -0.8539       
## iform_success                       -0.0162      -1.6842      *
## def_stop_rate_run                    0.0167       1.7861      *
## def_stop_rate_pass                  -0.0085      -0.8906       
## avg_pass_rushers                    -0.0089      -0.7962       
## avg_box_defenders                   -0.0056      -0.5241       
## cover0_rate                         -0.0033      -0.2839       
## cover1_rate                         -0.0152      -0.8483       
## cover2_rate                         -0.0056      -0.4265       
## cover3_rate                          0.0244       1.3337       
## cover4_rate                          0.0127       0.9427       
## cover6_rate                         -0.0068      -0.5583       
## two_man_rate                         0.0142       1.5133      .
## prevent_rate                         0.0198       2.4632     **
## roof_outdoors                       -0.0045      -0.1847       
## posteam_type_home                   -0.0236      -1.5020      .
## QB_short_touchdowns_12w              0.0043       0.4336       
## QB_medium_touchdowns_12w             0.0004       0.0366       
## QB_deep_touchdowns_12w              -0.0159      -1.5198      .
## RB_grades_pass_block_12w             0.0114       1.4157       
## RB_first_downs_12w                   0.0116       1.3866       
## RB_short_touchdowns_12w             -0.0109      -1.3513       
## RB_medium_touchdowns_12w            -0.0046      -0.6908       
## RB_deep_touchdowns_12w              -0.0024      -0.2849       
## WR1_grades_run_block_12w            -0.0150      -1.5739      .
## WR1_short_touchdowns_12w            -0.0097      -1.0873       
## WR1_medium_touchdowns_12w            0.0045       0.5164       
## WR1_deep_touchdowns_12w              0.0021       0.2423       
## WR2_grades_run_block_12w            -0.0050      -0.4437       
## WR2_short_touchdowns_12w            -0.0103      -1.2068       
## WR2_medium_touchdowns_12w            0.0083       0.9953       
## WR2_deep_touchdowns_12w             -0.0054      -0.6392       
## WR3_grades_run_block_12w             0.0096       0.8674       
## WR3_short_touchdowns_12w            -0.0010      -0.1180       
## WR3_medium_touchdowns_12w            0.0039       0.4657       
## WR3_deep_touchdowns_12w              0.0146       1.6792      *
## TE1_grades_pass_block_12w            0.0262       2.4891     **
## TE1_grades_run_block_12w            -0.0103      -0.9579       
## TE1_short_touchdowns_12w            -0.0028      -0.3367       
## TE1_medium_touchdowns_12w            0.0021       0.2509       
## TE1_deep_touchdowns_12w             -0.0003      -0.0400       
## DL1_grades_defense_12w              -0.0158      -1.9400      *
## DL2_grades_defense_12w               0.0029       0.3350       
## DL3_grades_defense_12w               0.0119       1.0195       
## DL4_grades_defense_12w              -0.0308      -2.5505     **
## LB1_grades_defense_12w               0.0052       0.6129       
## LB2_grades_defense_12w               0.0029       0.3408       
## LB3_grades_defense_12w              -0.0179      -1.5002      .
## LB4_grades_defense_12w              -0.0017      -0.1555       
## CB1_grades_defense_12w              -0.0129      -1.4318       
## CB2_grades_defense_12w              -0.0037      -0.3881       
## CB3_grades_defense_12w               0.0172       1.6140      .
## S1_grades_defense_12w               -0.0073      -0.9429       
## S2_grades_defense_12w                0.0050       0.5592       
## S3_grades_defense_12w                0.0099       1.0227       
## OL_grades_pass_block_12w            -0.0025      -0.2321       
## OL_grades_run_block_12w             -0.0063      -0.6028       
## yardline_1_10                       -0.0642      -2.3927     **
## yardline_11_20                       0.0180       0.6151       
## yardline_21_30                       0.0041       0.1446       
## yardline_41_50                       0.0453       1.8651      *
## yardline_51_60                       0.0190       0.6522       
## yardline_61_70                       0.0502       1.5284      .
## yardline_71_80                       0.0766       1.8982      *
## yardline_81_90                       0.1397       2.2962     **
## yardline_91_100                      0.0978       0.9179       
## year2017_team_ARI                    0.0704       0.3727       
## year2017_team_BUF                   -0.1533      -0.7935       
## year2017_team_CHI                    0.0201       0.1158       
## year2017_team_CLE                    0.1627       0.8319       
## year2017_team_DAL                   -0.1790      -1.0450       
## year2017_team_DET                   -0.0339      -0.1964       
## year2017_team_GB                     0.3371       2.0620     **
## year2017_team_HOU                    0.3342       1.6095      .
## year2017_team_MIA                   -0.2042      -1.1506       
## year2017_team_MIN                   -0.1062      -0.5927       
## year2017_team_NE                    -0.0291      -0.1592       
## year2017_team_SF                     0.3793       1.9735     **
## year2017_team_BAL                    0.0176       0.0896       
## year2017_team_DEN                   -0.0316      -0.1736       
## year2017_team_LA                     0.0405       0.2225       
## year2017_team_NYG                   -0.0604      -0.3553       
## year2017_team_OAK                   -0.1013      -0.5611       
## year2017_team_SEA                    0.1175       0.6408       
## year2017_team_CAR                    0.1124       0.5147       
## year2017_team_CIN                    0.1497       0.7505       
## year2017_team_IND                    0.1650       0.8995       
## year2017_team_NO                     0.0723       0.3205       
## year2017_team_PHI                    0.0386       0.2136       
## year2017_team_PIT                   -0.1324      -0.7976       
## year2017_team_TEN                    0.0828       0.3834       
## year2017_team_WAS                    0.0249       0.1295       
## year2017_team_KC                     0.2579       1.3610       
## year2017_team_LAC                   -0.0178      -0.0975       
## year2017_team_NYJ                    0.1446       0.6779       
## year2017_team_TB                     0.0336       0.1486       
## year2017_team_ATL                   -0.0400      -0.2070       
## year2017_team_JAX                    0.0822       0.4214       
## year2018_team_ARI                    0.1028       0.6991       
## year2018_team_BAL                    0.0996       0.6762       
## year2018_team_CAR                    0.0822       0.5613       
## year2018_team_CLE                   -0.0045      -0.0317       
## year2018_team_DET                    0.1498       1.0418       
## year2018_team_HOU                    0.2492       1.5002      .
## year2018_team_IND                   -0.0724      -0.5300       
## year2018_team_KC                     0.1463       1.0704       
## year2018_team_NYG                    0.1515       0.8570       
## year2018_team_OAK                   -0.1173      -0.6881       
## year2018_team_PHI                    0.1242       0.8474       
## year2018_team_SEA                   -0.0514      -0.2901       
## year2018_team_BUF                   -0.0783      -0.4963       
## year2018_team_CHI                    0.0223       0.1724       
## year2018_team_CIN                   -0.0112      -0.0657       
## year2018_team_DAL                   -0.0038      -0.0259       
## year2018_team_DEN                    0.0687       0.4720       
## year2018_team_GB                     0.0397       0.2349       
## year2018_team_LAC                    0.0489       0.3322       
## year2018_team_NE                    -0.0652      -0.4176       
## year2018_team_NO                     0.1137       0.8316       
## year2018_team_PIT                    0.1121       0.5866       
## year2018_team_SF                     0.0724       0.4710       
## year2018_team_MIA                    0.1136       0.7844       
## year2018_team_MIN                    0.0623       0.3880       
## year2018_team_NYJ                    0.2039       0.9261       
## year2018_team_TB                     0.0918       0.5389       
## year2018_team_ATL                    0.0737       0.5289       
## year2018_team_JAX                    0.0873       0.5660       
## year2018_team_LA                    -0.1394      -0.8628       
## year2018_team_TEN                    0.1496       0.9305       
## year2018_team_WAS                    0.1285       0.6365       
## year2019_team_ARI                   -0.0625      -0.3979       
## year2019_team_BUF                   -0.1124      -0.8706       
## year2019_team_CHI                    0.1172       0.7982       
## year2019_team_CLE                    0.1218       0.8171       
## year2019_team_DAL                   -0.0355      -0.2162       
## year2019_team_IND                   -0.0377      -0.2836       
## year2019_team_JAX                    0.1092       0.7067       
## year2019_team_KC                     0.0507       0.3721       
## year2019_team_LAC                   -0.0887      -0.6009       
## year2019_team_MIN                   -0.0301      -0.2047       
## year2019_team_NE                     0.0176       0.1053       
## year2019_team_NO                    -0.1809      -1.1770       
## year2019_team_PHI                    0.0828       0.5531       
## year2019_team_SEA                    0.0385       0.1976       
## year2019_team_SF                     0.0315       0.2334       
## year2019_team_TB                    -0.1026      -0.7173       
## year2019_team_BAL                    0.0486       0.3474       
## year2019_team_CAR                   -0.0803      -0.4952       
## year2019_team_DEN                    0.1900       1.3284       
## year2019_team_DET                   -0.0699      -0.4583       
## year2019_team_HOU                    0.0179       0.1196       
## year2019_team_LA                    -0.0925      -0.5780       
## year2019_team_MIA                   -0.2983      -1.8904      *
## year2019_team_NYG                   -0.1294      -0.8019       
## year2019_team_NYJ                   -0.1881      -1.4418      .
## year2019_team_OAK                   -0.0288      -0.1918       
## year2019_team_PIT                   -0.2690      -2.2490     **
## year2019_team_TEN                   -0.1354      -0.9641       
## year2019_team_CIN                    0.0871       0.6057       
## year2019_team_WAS                   -0.0335      -0.2267       
## year2019_team_ATL                    0.0272       0.1744       
## year2019_team_GB                    -0.0441      -0.2976       
## year2020_team_ATL                    0.0850       0.5521       
## year2020_team_BAL                    0.0892       0.5779       
## year2020_team_BUF                   -0.0020      -0.0108       
## year2020_team_CAR                    0.1241       0.7640       
## year2020_team_CIN                    0.1467       0.9710       
## year2020_team_DEN                   -0.0716      -0.4303       
## year2020_team_DET                   -0.0989      -0.6307       
## year2020_team_JAX                   -0.0862      -0.5451       
## year2020_team_KC                     0.0829       0.5119       
## year2020_team_LA                    -0.1665      -0.9492       
## year2020_team_MIN                    0.2203       1.5294      .
## year2020_team_NE                    -0.0202      -0.1305       
## year2020_team_NO                     0.0633       0.4337       
## year2020_team_NYG                    0.0594       0.3922       
## year2020_team_SF                     0.1164       0.7018       
## year2020_team_WAS                    0.0361       0.2470       
## year2020_team_CHI                    0.0819       0.5094       
## year2020_team_DAL                   -0.0193      -0.1281       
## year2020_team_GB                     0.0258       0.1449       
## year2020_team_HOU                   -0.0710      -0.4350       
## year2020_team_MIA                   -0.1280      -0.7856       
## year2020_team_NYJ                    0.0158       0.0931       
## year2020_team_TB                     0.0730       0.4434       
## year2020_team_TEN                   -0.0358      -0.2161       
## year2020_team_ARI                    0.0954       0.5759       
## year2020_team_CLE                   -0.2265      -1.3001       
## year2020_team_IND                   -0.1293      -0.7886       
## year2020_team_LAC                    0.0250       0.1374       
## year2020_team_PHI                    0.1275       0.8672       
## year2020_team_SEA                   -0.0046      -0.0282       
## year2020_team_LV                     0.1346       0.8600       
## year2020_team_PIT                   -0.1010      -0.6110       
## year2021_team_ATL                   -0.1914      -1.5104      .
## year2021_team_BUF                    0.0739       0.5878       
## year2021_team_CIN                   -0.1994      -1.6151      .
## year2021_team_DAL                   -0.0982      -0.6945       
## year2021_team_DEN                    0.0954       0.6951       
## year2021_team_DET                   -0.0438      -0.3225       
## year2021_team_KC                     0.0465       0.3709       
## year2021_team_LA                     0.0405       0.2959       
## year2021_team_LV                     0.0620       0.4206       
## year2021_team_MIN                   -0.0234      -0.1806       
## year2021_team_NE                     0.0993       0.7231       
## year2021_team_NO                     0.0205       0.1523       
## year2021_team_NYG                    0.0026       0.0195       
## year2021_team_SF                     0.0199       0.1445       
## year2021_team_TEN                   -0.0429      -0.3480       
## year2021_team_ARI                    0.0889       0.7375       
## year2021_team_BAL                    0.1548       0.8536       
## year2021_team_CAR                   -0.0689      -0.5830       
## year2021_team_CHI                   -0.2238      -1.7796      *
## year2021_team_GB                     0.1209       0.9844       
## year2021_team_IND                   -0.0333      -0.2452       
## year2021_team_LAC                    0.0836       0.5679       
## year2021_team_MIA                    0.0423       0.2774       
## year2021_team_NYJ                   -0.0064      -0.0431       
## year2021_team_PHI                   -0.1643      -1.3004       
## year2021_team_SEA                   -0.1642      -1.1043       
## year2021_team_TB                     0.0694       0.4976       
## year2021_team_WAS                   -0.0412      -0.3290       
## year2021_team_CLE                   -0.0844      -0.6598       
## year2021_team_HOU                   -0.0677      -0.4616       
## year2021_team_JAX                   -0.0319      -0.2168       
## year2021_team_PIT                    0.0616       0.4564       
## year2022_team_ARI                   -0.1449      -1.1218       
## year2022_team_ATL                   -0.2750      -2.0569     **
## year2022_team_CAR                    0.1333       0.9038       
## year2022_team_CHI                   -0.0943      -0.5874       
## year2022_team_CIN                   -0.1116      -0.7562       
## year2022_team_HOU                   -0.0381      -0.2733       
## year2022_team_IND                   -0.1016      -0.7592       
## year2022_team_LAC                   -0.0539      -0.4034       
## year2022_team_MIA                   -0.1629      -1.3251       
## year2022_team_SEA                   -0.0477      -0.3654       
## year2022_team_TB                     0.0357       0.2783       
## year2022_team_TEN                    0.1841       1.5713      .
## year2022_team_WAS                    0.0188       0.1413       
## year2022_team_BAL                   -0.1530      -1.0687       
## year2022_team_BUF                    0.0268       0.2075       
## year2022_team_DAL                    0.0009       0.0057       
## year2022_team_DET                   -0.0608      -0.4770       
## year2022_team_GB                    -0.1027      -0.7299       
## year2022_team_JAX                   -0.1403      -1.2360       
## year2022_team_KC                    -0.1095      -0.6311       
## year2022_team_LA                     0.1873       1.4087       
## year2022_team_LV                     0.1664       1.1602       
## year2022_team_NO                    -0.0367      -0.2369       
## year2022_team_PHI                    0.0708       0.5445       
## year2022_team_PIT                    0.2197       1.7367      *
## year2022_team_DEN                    0.0510       0.4185       
## year2022_team_MIN                   -0.1139      -0.7392       
## year2022_team_NE                     0.0411       0.2841       
## year2022_team_NYJ                   -0.0793      -0.6082       
## year2022_team_NYG                   -0.0510      -0.3522       
## year2022_team_SF                    -0.1766      -1.0204       
## year2023_team_BAL                   -0.0465      -0.3541       
## year2023_team_CHI                   -0.1252      -0.8960       
## year2023_team_CLE                   -0.1329      -0.8968       
## year2023_team_GB                     0.0311       0.2323       
## year2023_team_IND                    0.0946       0.7518       
## year2023_team_KC                     0.0516       0.3658       
## year2023_team_LAC                    0.0504       0.3571       
## year2023_team_LV                     0.0112       0.0889       
## year2023_team_MIA                    0.0689       0.5155       
## year2023_team_MIN                    0.1515       1.2719       
## year2023_team_NO                    -0.0328      -0.2313       
## year2023_team_NYG                    0.0792       0.5881       
## year2023_team_SEA                   -0.2830      -2.3166     **
## year2023_team_SF                     0.0619       0.4016       
## year2023_team_WAS                    0.1920       1.5359      .
## year2023_team_ATL                   -0.0957      -0.6516       
## year2023_team_BUF                   -0.0736      -0.4879       
## year2023_team_CAR                    0.0868       0.6883       
## year2023_team_DAL                    0.0880       0.6271       
## year2023_team_DEN                    0.0140       0.1092       
## year2023_team_HOU                   -0.0158      -0.1037       
## year2023_team_LA                     0.0010       0.0071       
## year2023_team_NE                     0.0354       0.2654       
## year2023_team_PHI                   -0.0217      -0.1649       
## year2023_team_PIT                    0.0004       0.0028       
## year2023_team_TEN                    0.0307       0.2071       
## year2023_team_ARI                   -0.1704      -1.2129       
## year2023_team_CIN                   -0.1424      -0.9243       
## year2023_team_DET                    0.0473       0.3802       
## year2023_team_TB                     0.1189       0.8631       
## year2023_team_JAX                   -0.0746      -0.5012       
## year2023_team_NYJ                    0.1987       1.4589      .
## is_first_half                       -0.0097      -0.5337       
## time_in_half                         0.0163       1.6530      *
## home_attendance                     -0.0272      -0.3623       
## GIMR                                 0.0473       2.0757     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1111887 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.51
## prev_singleback_rate                                   5.48
## cover1_rate                                            6.14
## cover3_rate                                            6.50
## home_attendance                                       13.70
## 
## 
##  ================================================================================ 
## MODEL: Starter Model with GIMR 
## ================================================================================ 
## 
## 
## Starter Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.4114       3.3014    ***
## ydstogo                             -0.1090     -12.4943    ***
## posteam_timeouts_remaining           0.0116       1.2652       
## defteam_timeouts_remaining           0.0089       0.9971       
## rush_attempt                         0.1401       7.4062    ***
## week                                 0.0046       0.4590       
## temp                                -0.0089      -0.8375       
## wind                                 0.0046       0.4281       
## vegas_wp                             0.0090       0.8082       
## spread_line                         -0.0121      -0.9685       
## total_line                           0.0362       2.7575    ***
## prep_days                            0.0072       0.9222       
## overall_win_pct                      0.0092       0.6990       
## team_win_pct                         0.0191       1.3224       
## prev_win_pct                        -0.0289      -2.2308     **
## prev_shotgun_rate                    0.0047       0.2105       
## prev_singleback_rate                 0.0052       0.3114       
## prev_empty_rate                      0.0095       0.7676       
## prev_iform_rate                     -0.0015      -0.0980       
## prev_shotgun_success                 0.0044       0.3708       
## prev_singleback_success              0.0010       0.0805       
## prev_empty_success                   0.0020       0.1784       
## prev_iform_success                   0.0279       2.7640    ***
## prev_stop_rate_run                  -0.0002      -0.0185       
## prev_stop_rate_pass                 -0.0317      -3.1127    ***
## shotgun_rate                         0.0144       1.0361       
## singleback_rate                      0.0085       0.7037       
## empty_rate                          -0.0014      -0.1223       
## iform_rate                          -0.0174      -1.6336      .
## shotgun_success                     -0.0205      -2.2707     **
## singleback_success                  -0.0117      -1.2566       
## empty_success                       -0.0055      -0.5632       
## iform_success                       -0.0156      -1.6114      .
## def_stop_rate_run                    0.0156       1.6726      *
## def_stop_rate_pass                  -0.0092      -0.9644       
## avg_pass_rushers                    -0.0107      -0.9687       
## avg_box_defenders                   -0.0036      -0.3460       
## cover0_rate                         -0.0042      -0.3713       
## cover1_rate                         -0.0120      -0.6759       
## cover2_rate                         -0.0041      -0.3145       
## cover3_rate                          0.0182       0.9920       
## cover4_rate                          0.0133       0.9875       
## cover6_rate                         -0.0075      -0.6209       
## two_man_rate                         0.0144       1.5243      .
## prevent_rate                         0.0203       2.4476     **
## roof_outdoors                        0.0012       0.0497       
## posteam_type_home                   -0.0235      -1.4911      .
## starter_QB_short_touchdowns_12w       0.0326       3.0948    ***
## starter_QB_medium_touchdowns_12w      -0.0120      -1.0944       
## starter_QB_deep_touchdowns_12w      -0.0184      -1.4945      .
## starter_RB_grades_pass_block_12w      -0.0153      -1.6473      *
## starter_RB_first_downs_12w          -0.0002      -0.0245       
## starter_RB_short_touchdowns_12w      -0.0146      -1.6238      .
## starter_RB_medium_touchdowns_12w      -0.0096      -1.1849       
## starter_RB_deep_touchdowns_12w       0.0033       0.3689       
## starter_WR1_grades_run_block_12w       0.0094       0.6828       
## starter_WR1_short_touchdowns_12w      -0.0154      -1.7533      *
## starter_WR1_medium_touchdowns_12w       0.0118       1.3158       
## starter_WR1_deep_touchdowns_12w       0.0160       1.6971      *
## starter_WR2_grades_run_block_12w      -0.0196      -1.4021       
## starter_WR2_short_touchdowns_12w      -0.0247      -2.9597    ***
## starter_WR2_medium_touchdowns_12w       0.0031       0.3438       
## starter_WR2_deep_touchdowns_12w      -0.0009      -0.0939       
## starter_WR3_grades_run_block_12w      -0.0100      -0.7738       
## starter_WR3_short_touchdowns_12w      -0.0240      -2.7742    ***
## starter_WR3_medium_touchdowns_12w      -0.0026      -0.3040       
## starter_WR3_deep_touchdowns_12w      -0.0090      -1.0691       
## starter_TE1_grades_pass_block_12w       0.0230       2.1167     **
## starter_TE1_grades_run_block_12w      -0.0183      -1.3756       
## starter_TE1_short_touchdowns_12w      -0.0123      -1.3269       
## starter_TE1_medium_touchdowns_12w       0.0014       0.1601       
## starter_TE1_deep_touchdowns_12w       0.0046       0.5165       
## starter_DL1_grades_defense_12w       0.0082       0.7105       
## starter_DL2_grades_defense_12w       0.0158       1.3535       
## starter_DL3_grades_defense_12w       0.0054       0.4592       
## starter_DL4_grades_defense_12w       0.0071       0.7346       
## starter_LB1_grades_defense_12w       0.0054       0.4805       
## starter_LB2_grades_defense_12w       0.0200       1.7740      *
## starter_LB3_grades_defense_12w       0.0108       1.0853       
## starter_LB4_grades_defense_12w      -0.0250      -2.9107    ***
## starter_CB1_grades_defense_12w      -0.0045      -0.3534       
## starter_CB2_grades_defense_12w       0.0040       0.3260       
## starter_CB3_grades_defense_12w      -0.0063      -0.6575       
## starter_S1_grades_defense_12w        0.0001       0.0107       
## starter_S2_grades_defense_12w       -0.0069      -0.6067       
## starter_S3_grades_defense_12w       -0.0056      -0.6625       
## starter_OL_grades_pass_block_12w       0.0463       2.5814    ***
## starter_OL_grades_run_block_12w      -0.0325      -1.6050      .
## yardline_1_10                       -0.0571      -2.2048     **
## yardline_11_20                       0.0031       0.1052       
## yardline_21_30                      -0.0007      -0.0237       
## yardline_41_50                       0.0443       1.8323      *
## yardline_51_60                       0.0188       0.6473       
## yardline_61_70                       0.0489       1.5039      .
## yardline_71_80                       0.0661       1.6275      .
## yardline_81_90                       0.1254       2.1106     **
## yardline_91_100                      0.1345       1.2542       
## year2017_team_ARI                    0.0774       0.4130       
## year2017_team_BUF                   -0.1282      -0.6718       
## year2017_team_CHI                    0.0016       0.0093       
## year2017_team_CLE                    0.1084       0.5502       
## year2017_team_DAL                   -0.1827      -1.0549       
## year2017_team_DET                   -0.0789      -0.4639       
## year2017_team_GB                     0.3314       2.0099     **
## year2017_team_HOU                    0.3886       1.8053      *
## year2017_team_MIA                   -0.1760      -0.9897       
## year2017_team_MIN                   -0.1390      -0.7792       
## year2017_team_NE                    -0.0591      -0.3171       
## year2017_team_SF                     0.3475       1.7508      *
## year2017_team_BAL                    0.0348       0.1796       
## year2017_team_DEN                    0.0294       0.1611       
## year2017_team_LA                     0.0638       0.3429       
## year2017_team_NYG                   -0.0333      -0.1949       
## year2017_team_OAK                   -0.0333      -0.1789       
## year2017_team_SEA                    0.1091       0.5830       
## year2017_team_CAR                   -0.0213      -0.0947       
## year2017_team_CIN                    0.0919       0.4570       
## year2017_team_IND                    0.2003       1.1014       
## year2017_team_NO                     0.0002       0.0010       
## year2017_team_PHI                    0.0016       0.0086       
## year2017_team_PIT                   -0.1682      -1.0178       
## year2017_team_TEN                    0.0091       0.0415       
## year2017_team_WAS                    0.0178       0.0952       
## year2017_team_KC                     0.2568       1.3155       
## year2017_team_LAC                    0.0040       0.0205       
## year2017_team_NYJ                    0.1307       0.6091       
## year2017_team_TB                     0.0356       0.1518       
## year2017_team_ATL                   -0.0171      -0.0907       
## year2017_team_JAX                    0.0871       0.4348       
## year2018_team_ARI                    0.1675       1.1305       
## year2018_team_BAL                    0.0846       0.5686       
## year2018_team_CAR                    0.0604       0.3994       
## year2018_team_CLE                   -0.0022      -0.0160       
## year2018_team_DET                    0.0892       0.6072       
## year2018_team_HOU                    0.1753       1.0555       
## year2018_team_IND                   -0.0997      -0.7175       
## year2018_team_KC                     0.0996       0.6856       
## year2018_team_NYG                    0.1585       0.9119       
## year2018_team_OAK                   -0.0154      -0.0901       
## year2018_team_PHI                    0.0501       0.3411       
## year2018_team_SEA                   -0.0405      -0.2307       
## year2018_team_BUF                   -0.0715      -0.4427       
## year2018_team_CHI                   -0.0024      -0.0183       
## year2018_team_CIN                   -0.0438      -0.2776       
## year2018_team_DAL                    0.0203       0.1350       
## year2018_team_DEN                    0.0199       0.1320       
## year2018_team_GB                     0.0113       0.0654       
## year2018_team_LAC                    0.0916       0.6355       
## year2018_team_NE                    -0.1229      -0.7812       
## year2018_team_NO                     0.0920       0.6563       
## year2018_team_PIT                    0.0102       0.0518       
## year2018_team_SF                     0.0813       0.5096       
## year2018_team_MIA                    0.0744       0.5164       
## year2018_team_MIN                    0.0703       0.4513       
## year2018_team_NYJ                    0.1318       0.6398       
## year2018_team_TB                     0.0695       0.4240       
## year2018_team_ATL                    0.0959       0.6720       
## year2018_team_JAX                    0.0006       0.0040       
## year2018_team_LA                    -0.1083      -0.6840       
## year2018_team_TEN                    0.1659       0.9928       
## year2018_team_WAS                    0.0936       0.4693       
## year2019_team_ARI                   -0.1116      -0.7344       
## year2019_team_BUF                   -0.0999      -0.7918       
## year2019_team_CHI                    0.1237       0.8418       
## year2019_team_CLE                    0.1480       0.9485       
## year2019_team_DAL                   -0.0214      -0.1300       
## year2019_team_IND                   -0.0446      -0.3334       
## year2019_team_JAX                    0.1402       0.9174       
## year2019_team_KC                     0.0390       0.2831       
## year2019_team_LAC                   -0.0680      -0.4931       
## year2019_team_MIN                   -0.0522      -0.3619       
## year2019_team_NE                     0.0026       0.0158       
## year2019_team_NO                    -0.1632      -1.0706       
## year2019_team_PHI                    0.0567       0.3835       
## year2019_team_SEA                    0.0566       0.2930       
## year2019_team_SF                     0.0011       0.0083       
## year2019_team_TB                    -0.1034      -0.7565       
## year2019_team_BAL                    0.0458       0.3280       
## year2019_team_CAR                   -0.1117      -0.6806       
## year2019_team_DEN                    0.1225       0.8296       
## year2019_team_DET                   -0.0425      -0.2748       
## year2019_team_HOU                   -0.0119      -0.0810       
## year2019_team_LA                    -0.1397      -0.8423       
## year2019_team_MIA                   -0.2991      -1.8814      *
## year2019_team_NYG                   -0.1133      -0.7168       
## year2019_team_NYJ                   -0.1994      -1.5508      .
## year2019_team_OAK                    0.0272       0.1753       
## year2019_team_PIT                   -0.3564      -2.9175    ***
## year2019_team_TEN                   -0.1275      -0.9075       
## year2019_team_CIN                    0.1272       0.8366       
## year2019_team_WAS                   -0.0253      -0.1634       
## year2019_team_ATL                   -0.0007      -0.0043       
## year2019_team_GB                    -0.0641      -0.4185       
## year2020_team_ATL                    0.1159       0.7459       
## year2020_team_BAL                    0.0608       0.3985       
## year2020_team_BUF                    0.0468       0.2540       
## year2020_team_CAR                    0.1903       1.1346       
## year2020_team_CIN                    0.1460       0.9797       
## year2020_team_DEN                   -0.0547      -0.3242       
## year2020_team_DET                   -0.0685      -0.4442       
## year2020_team_JAX                   -0.0826      -0.5175       
## year2020_team_KC                     0.0494       0.2932       
## year2020_team_LA                    -0.1662      -0.9434       
## year2020_team_MIN                    0.2147       1.5205      .
## year2020_team_NE                     0.0164       0.1078       
## year2020_team_NO                     0.0817       0.5533       
## year2020_team_NYG                    0.0542       0.3495       
## year2020_team_SF                     0.1469       0.8683       
## year2020_team_WAS                    0.0509       0.3421       
## year2020_team_CHI                    0.1519       0.9667       
## year2020_team_DAL                    0.0320       0.2153       
## year2020_team_GB                     0.0107       0.0607       
## year2020_team_HOU                   -0.1379      -0.8408       
## year2020_team_MIA                   -0.1075      -0.6595       
## year2020_team_NYJ                    0.0813       0.4767       
## year2020_team_TB                     0.0728       0.4593       
## year2020_team_TEN                   -0.0243      -0.1479       
## year2020_team_ARI                    0.1454       0.8979       
## year2020_team_CLE                   -0.1972      -1.0917       
## year2020_team_IND                   -0.1703      -1.0443       
## year2020_team_LAC                    0.0840       0.4697       
## year2020_team_PHI                    0.1894       1.3041       
## year2020_team_SEA                   -0.0217      -0.1353       
## year2020_team_LV                     0.1498       0.9593       
## year2020_team_PIT                   -0.1282      -0.7828       
## year2021_team_ATL                   -0.1694      -1.2950       
## year2021_team_BUF                    0.1037       0.8289       
## year2021_team_CIN                   -0.1577      -1.2345       
## year2021_team_DAL                   -0.0783      -0.5669       
## year2021_team_DEN                    0.1076       0.8344       
## year2021_team_DET                   -0.0837      -0.6033       
## year2021_team_KC                     0.0559       0.4395       
## year2021_team_LA                     0.0106       0.0797       
## year2021_team_LV                     0.0872       0.6034       
## year2021_team_MIN                   -0.0013      -0.0096       
## year2021_team_NE                     0.1177       0.8667       
## year2021_team_NO                     0.0280       0.2044       
## year2021_team_NYG                    0.0777       0.5836       
## year2021_team_SF                     0.0161       0.1154       
## year2021_team_TEN                    0.0418       0.3325       
## year2021_team_ARI                    0.1353       1.1250       
## year2021_team_BAL                    0.2339       1.3240       
## year2021_team_CAR                    0.0090       0.0758       
## year2021_team_CHI                   -0.1995      -1.5608      .
## year2021_team_GB                     0.1135       0.9168       
## year2021_team_IND                    0.0044       0.0317       
## year2021_team_LAC                    0.0538       0.3639       
## year2021_team_MIA                    0.1147       0.7403       
## year2021_team_NYJ                    0.0030       0.0216       
## year2021_team_PHI                   -0.1650      -1.2783       
## year2021_team_SEA                   -0.1347      -0.8783       
## year2021_team_TB                     0.0283       0.2015       
## year2021_team_WAS                   -0.0652      -0.5204       
## year2021_team_CLE                   -0.0538      -0.4217       
## year2021_team_HOU                   -0.0319      -0.2184       
## year2021_team_JAX                    0.0474       0.3265       
## year2021_team_PIT                    0.0329       0.2415       
## year2022_team_ARI                   -0.1420      -1.0810       
## year2022_team_ATL                   -0.1780      -1.3627       
## year2022_team_CAR                    0.0827       0.5472       
## year2022_team_CHI                    0.0299       0.1778       
## year2022_team_CIN                   -0.0818      -0.5514       
## year2022_team_HOU                   -0.0006      -0.0046       
## year2022_team_IND                   -0.0756      -0.5727       
## year2022_team_LAC                   -0.0958      -0.7192       
## year2022_team_MIA                   -0.1323      -1.0666       
## year2022_team_SEA                    0.0174       0.1286       
## year2022_team_TB                     0.0499       0.3830       
## year2022_team_TEN                    0.2254       1.9702     **
## year2022_team_WAS                    0.0853       0.6491       
## year2022_team_BAL                   -0.1821      -1.2315       
## year2022_team_BUF                    0.0865       0.6482       
## year2022_team_DAL                    0.0118       0.0698       
## year2022_team_DET                    0.0160       0.1260       
## year2022_team_GB                    -0.0602      -0.4252       
## year2022_team_JAX                   -0.1435      -1.2599       
## year2022_team_KC                    -0.1520      -0.9223       
## year2022_team_LA                     0.1869       1.3873       
## year2022_team_LV                     0.1789       1.2293       
## year2022_team_NO                    -0.0142      -0.0889       
## year2022_team_PHI                    0.0685       0.5284       
## year2022_team_PIT                    0.1830       1.4170       
## year2022_team_DEN                    0.0988       0.8151       
## year2022_team_MIN                   -0.0590      -0.3789       
## year2022_team_NE                     0.0409       0.2883       
## year2022_team_NYJ                   -0.1031      -0.7917       
## year2022_team_NYG                   -0.0191      -0.1337       
## year2022_team_SF                    -0.1406      -0.8644       
## year2023_team_BAL                   -0.0537      -0.4027       
## year2023_team_CHI                   -0.1001      -0.7091       
## year2023_team_CLE                   -0.1708      -1.0959       
## year2023_team_GB                     0.0166       0.1265       
## year2023_team_IND                    0.1103       0.8489       
## year2023_team_KC                    -0.0005      -0.0032       
## year2023_team_LAC                    0.1034       0.7189       
## year2023_team_LV                     0.0241       0.1906       
## year2023_team_MIA                    0.0157       0.1163       
## year2023_team_MIN                    0.2250       1.8975      *
## year2023_team_NO                    -0.0721      -0.4911       
## year2023_team_NYG                    0.1030       0.7372       
## year2023_team_SEA                   -0.2221      -1.8058      *
## year2023_team_SF                     0.0374       0.2424       
## year2023_team_WAS                    0.2143       1.7710      *
## year2023_team_ATL                   -0.0831      -0.5626       
## year2023_team_BUF                   -0.0533      -0.3442       
## year2023_team_CAR                    0.1450       1.1178       
## year2023_team_DAL                    0.0948       0.6374       
## year2023_team_DEN                   -0.0051      -0.0392       
## year2023_team_HOU                    0.0425       0.2911       
## year2023_team_LA                     0.0706       0.4752       
## year2023_team_NE                     0.0764       0.5694       
## year2023_team_PHI                   -0.0580      -0.4393       
## year2023_team_PIT                    0.0451       0.2839       
## year2023_team_TEN                    0.0312       0.2160       
## year2023_team_ARI                   -0.0778      -0.5541       
## year2023_team_CIN                   -0.0604      -0.4121       
## year2023_team_DET                    0.0789       0.6261       
## year2023_team_TB                     0.1332       0.9439       
## year2023_team_JAX                   -0.0747      -0.4941       
## year2023_team_NYJ                    0.2214       1.5884      .
## is_first_half                       -0.0073      -0.4088       
## time_in_half                         0.0145       1.4802      .
## home_attendance                     -0.0223      -0.3051       
## GIMR                                 0.0410       1.8224      *
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1136534 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.93
## prev_singleback_rate                                   5.75
## cover1_rate                                            6.20
## cover3_rate                                            6.54
## starter_OL_grades_pass_block_12w                       6.26
## starter_OL_grades_run_block_12w                        8.19
## home_attendance                                       13.72
## 
## 
##  ================================================================================ 
## MODEL COMPARISON - Adjusted R-squared values
## ================================================================================ 
## 
## Player Model with GIMR: 0.1111887 
## Starter Model with GIMR: 0.1136534 
## 
## 
## ==================================================================================================== 
## ANALYZING DATASET 5/8: Defense Stops
## ==================================================================================================== 
## 
## Reading data: processed_predict_ccafd_def_stops.csv.csv.gz
## Reading data: processed_predict_ccfd_def_stops.csv.csv.gz
## 
## Phase 1: Validation Phase
## 
## Running 2 test iterations with best parameters...
## 
## Test Results over 2 iterations:
## Mean AUC: 0.8869594 
## SD AUC: 0.002348521 
## 95% CI: 0.8823563 to 0.8915625 
## 
## 
##  ================================================================================ 
## MODEL: Player Model with GIMR 
## ================================================================================ 
## 
## 
## Player Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.4123       3.2772    ***
## ydstogo                             -0.1129     -12.7781    ***
## posteam_timeouts_remaining           0.0118       1.2897       
## defteam_timeouts_remaining           0.0081       0.9195       
## rush_attempt                         0.1501       7.6577    ***
## week                                 0.0046       0.4636       
## temp                                -0.0124      -1.1675       
## wind                                 0.0099       0.9319       
## vegas_wp                             0.0139       1.2282       
## spread_line                         -0.0033      -0.2632       
## total_line                           0.0225       1.7533      *
## prep_days                            0.0075       0.9593       
## overall_win_pct                      0.0078       0.5842       
## team_win_pct                         0.0186       1.2895       
## prev_win_pct                        -0.0348      -2.7460    ***
## prev_shotgun_rate                    0.0151       0.6877       
## prev_singleback_rate                 0.0122       0.7429       
## prev_empty_rate                      0.0130       1.0788       
## prev_iform_rate                      0.0069       0.4428       
## prev_shotgun_success                 0.0035       0.2955       
## prev_singleback_success              0.0072       0.6065       
## prev_empty_success                   0.0026       0.2309       
## prev_iform_success                   0.0238       2.3754     **
## prev_stop_rate_run                  -0.0011      -0.0962       
## prev_stop_rate_pass                 -0.0377      -3.6157    ***
## shotgun_rate                         0.0121       0.8771       
## singleback_rate                      0.0058       0.4820       
## empty_rate                          -0.0032      -0.2839       
## iform_rate                          -0.0194      -1.8306      *
## shotgun_success                     -0.0181      -2.0201     **
## singleback_success                  -0.0061      -0.6593       
## empty_success                       -0.0073      -0.7654       
## iform_success                       -0.0156      -1.6231      .
## def_stop_rate_run                    0.0149       1.5666      .
## def_stop_rate_pass                  -0.0108      -1.1332       
## avg_pass_rushers                    -0.0065      -0.5701       
## avg_box_defenders                   -0.0016      -0.1504       
## cover0_rate                         -0.0050      -0.4162       
## cover1_rate                         -0.0058      -0.3068       
## cover2_rate                          0.0007       0.0521       
## cover3_rate                          0.0346       1.7656      *
## cover4_rate                          0.0172       1.1922       
## cover6_rate                         -0.0025      -0.1975       
## two_man_rate                         0.0132       1.3715       
## prevent_rate                         0.0196       2.4326     **
## roof_outdoors                       -0.0175      -0.7283       
## posteam_type_home                   -0.0220      -1.4049       
## QB_grades_pass_12w                   0.0100       1.1894       
## RB_grades_run_12w                    0.0046       0.6078       
## WR1_grades_offense_12w              -0.0193      -2.2539     **
## WR2_grades_offense_12w              -0.0061      -0.5992       
## WR3_grades_offense_12w               0.0198       2.0008     **
## TE1_grades_offense_12w               0.0128       1.5912      .
## DL1_grades_stops_12w                -0.0079      -0.9247       
## DL1_productivity_stops_12w          -0.0030      -0.3634       
## DL2_grades_stops_12w                 0.0098       1.1750       
## DL2_productivity_stops_12w          -0.0116      -1.3591       
## DL3_grades_stops_12w                 0.0101       1.0593       
## DL3_productivity_stops_12w          -0.0063      -0.6582       
## DL4_grades_stops_12w                -0.0031      -0.3226       
## DL4_productivity_stops_12w          -0.0207      -2.2047     **
## LB1_grades_stops_12w                -0.0014      -0.1424       
## LB1_productivity_stops_12w          -0.0020      -0.2084       
## LB1_zone_stops_12w                  -0.0025      -0.2492       
## LB1_man_stops_12w                    0.0014       0.1478       
## LB2_grades_stops_12w                -0.0213      -2.1844     **
## LB2_productivity_stops_12w          -0.0102      -1.0162       
## LB2_zone_stops_12w                   0.0104       1.0505       
## LB2_man_stops_12w                   -0.0097      -0.9665       
## LB3_grades_stops_12w                -0.0098      -0.8330       
## LB3_productivity_stops_12w           0.0146       1.4131       
## LB3_zone_stops_12w                   0.0063       0.5911       
## LB3_man_stops_12w                   -0.0098      -1.0130       
## LB4_grades_stops_12w                -0.0019      -0.1729       
## LB4_productivity_stops_12w           0.0144       1.5614      .
## LB4_zone_stops_12w                  -0.0044      -0.4104       
## LB4_man_stops_12w                   -0.0051      -0.5629       
## CB1_grades_stops_12w                 0.0162       1.8279      *
## CB1_zone_stops_12w                   0.0092       1.0412       
## CB1_man_stops_12w                    0.0107       1.2261       
## CB2_grades_stops_12w                -0.0005      -0.0581       
## CB2_zone_stops_12w                   0.0018       0.2084       
## CB2_man_stops_12w                    0.0004       0.0431       
## CB3_grades_stops_12w                 0.0015       0.1780       
## CB3_zone_stops_12w                   0.0038       0.4059       
## CB3_man_stops_12w                    0.0087       1.0354       
## S1_grades_stops_12w                 -0.0050      -0.5305       
## S1_zone_stops_12w                   -0.0021      -0.2412       
## S1_man_stops_12w                     0.0081       0.8724       
## S2_grades_stops_12w                  0.0198       2.1110     **
## S2_zone_stops_12w                   -0.0071      -0.7212       
## S2_man_stops_12w                    -0.0039      -0.4439       
## S3_grades_stops_12w                 -0.0029      -0.2717       
## S3_zone_stops_12w                    0.0011       0.1078       
## S3_man_stops_12w                     0.0121       1.3155       
## OL_grades_offense_12w               -0.0044      -0.5376       
## yardline_1_10                       -0.0563      -2.1189     **
## yardline_11_20                       0.0114       0.3885       
## yardline_21_30                       0.0040       0.1415       
## yardline_41_50                       0.0496       2.0490     **
## yardline_51_60                       0.0193       0.6688       
## yardline_61_70                       0.0453       1.3968       
## yardline_71_80                       0.0738       1.8320      *
## yardline_81_90                       0.1399       2.3326     **
## yardline_91_100                      0.1278       1.2498       
## year2017_team_ARI                    0.1062       0.5646       
## year2017_team_BUF                   -0.0885      -0.4434       
## year2017_team_CHI                    0.0458       0.2580       
## year2017_team_CLE                    0.2232       1.1078       
## year2017_team_DAL                   -0.0944      -0.5332       
## year2017_team_DET                   -0.0520      -0.2896       
## year2017_team_GB                     0.4173       2.4997     **
## year2017_team_HOU                    0.4238       1.9228      *
## year2017_team_MIA                   -0.1441      -0.7931       
## year2017_team_MIN                    0.0038       0.0203       
## year2017_team_NE                     0.0445       0.2311       
## year2017_team_SF                     0.4694       2.4034     **
## year2017_team_BAL                    0.0809       0.4209       
## year2017_team_DEN                    0.0696       0.3777       
## year2017_team_LA                     0.1536       0.7946       
## year2017_team_NYG                    0.0122       0.0689       
## year2017_team_OAK                   -0.0452      -0.2491       
## year2017_team_SEA                    0.1701       0.9160       
## year2017_team_CAR                    0.1486       0.6826       
## year2017_team_CIN                    0.1960       0.9529       
## year2017_team_IND                    0.1960       1.0698       
## year2017_team_NO                     0.1550       0.7099       
## year2017_team_PHI                    0.1008       0.5428       
## year2017_team_PIT                   -0.1072      -0.5824       
## year2017_team_TEN                    0.1508       0.7136       
## year2017_team_WAS                    0.1152       0.5852       
## year2017_team_KC                     0.3679       1.8436      *
## year2017_team_LAC                    0.0415       0.2215       
## year2017_team_NYJ                    0.2207       1.0175       
## year2017_team_TB                     0.1840       0.7455       
## year2017_team_ATL                    0.0367       0.1855       
## year2017_team_JAX                    0.1344       0.6425       
## year2018_team_ARI                    0.0977       0.6620       
## year2018_team_BAL                    0.1342       0.9185       
## year2018_team_CAR                    0.0954       0.6449       
## year2018_team_CLE                   -0.0021      -0.0144       
## year2018_team_DET                    0.1410       0.9825       
## year2018_team_HOU                    0.2450       1.5165      .
## year2018_team_IND                   -0.0878      -0.6430       
## year2018_team_KC                     0.1350       0.9633       
## year2018_team_NYG                    0.1540       0.8958       
## year2018_team_OAK                   -0.0772      -0.4533       
## year2018_team_PHI                    0.1357       0.9261       
## year2018_team_SEA                   -0.0567      -0.3187       
## year2018_team_BUF                   -0.0904      -0.5545       
## year2018_team_CHI                    0.0347       0.2696       
## year2018_team_CIN                    0.0022       0.0135       
## year2018_team_DAL                   -0.0472      -0.3186       
## year2018_team_DEN                    0.0527       0.3594       
## year2018_team_GB                     0.0093       0.0543       
## year2018_team_LAC                    0.0583       0.3905       
## year2018_team_NE                    -0.0636      -0.4050       
## year2018_team_NO                     0.1275       0.9300       
## year2018_team_PIT                    0.1416       0.7443       
## year2018_team_SF                     0.1049       0.6866       
## year2018_team_MIA                    0.1130       0.7815       
## year2018_team_MIN                    0.1004       0.6400       
## year2018_team_NYJ                    0.2127       0.8737       
## year2018_team_TB                     0.1081       0.6559       
## year2018_team_ATL                    0.1414       1.0421       
## year2018_team_JAX                    0.0415       0.2703       
## year2018_team_LA                    -0.0704      -0.4491       
## year2018_team_TEN                    0.1481       0.8809       
## year2018_team_WAS                    0.0152       0.0789       
## year2019_team_ARI                   -0.0428      -0.2878       
## year2019_team_BUF                   -0.0838      -0.6541       
## year2019_team_CHI                    0.1400       0.9529       
## year2019_team_CLE                    0.1347       0.8792       
## year2019_team_DAL                   -0.0034      -0.0209       
## year2019_team_IND                   -0.0495      -0.3644       
## year2019_team_JAX                    0.0900       0.5981       
## year2019_team_KC                     0.0560       0.4215       
## year2019_team_LAC                   -0.0674      -0.4720       
## year2019_team_MIN                    0.0005       0.0037       
## year2019_team_NE                     0.0427       0.2488       
## year2019_team_NO                    -0.1297      -0.8575       
## year2019_team_PHI                    0.0913       0.6177       
## year2019_team_SEA                    0.0507       0.2545       
## year2019_team_SF                     0.0064       0.0485       
## year2019_team_TB                    -0.0971      -0.6948       
## year2019_team_BAL                    0.0580       0.4113       
## year2019_team_CAR                   -0.0362      -0.2255       
## year2019_team_DEN                    0.1640       1.1070       
## year2019_team_DET                   -0.0289      -0.1864       
## year2019_team_HOU                    0.0359       0.2454       
## year2019_team_LA                    -0.0440      -0.2734       
## year2019_team_MIA                   -0.2939      -1.8682      *
## year2019_team_NYG                   -0.1001      -0.6248       
## year2019_team_NYJ                   -0.1798      -1.3422       
## year2019_team_OAK                   -0.0130      -0.0839       
## year2019_team_PIT                   -0.2700      -2.2295     **
## year2019_team_TEN                   -0.1875      -1.3557       
## year2019_team_CIN                    0.1360       0.9627       
## year2019_team_WAS                   -0.0319      -0.2068       
## year2019_team_ATL                    0.0476       0.3031       
## year2019_team_GB                    -0.0036      -0.0240       
## year2020_team_ATL                    0.0868       0.5617       
## year2020_team_BAL                    0.0979       0.6285       
## year2020_team_BUF                    0.0420       0.2273       
## year2020_team_CAR                    0.1386       0.8611       
## year2020_team_CIN                    0.1541       1.0330       
## year2020_team_DEN                   -0.0767      -0.4585       
## year2020_team_DET                   -0.1115      -0.7075       
## year2020_team_JAX                   -0.0769      -0.4823       
## year2020_team_KC                     0.0547       0.3382       
## year2020_team_LA                    -0.1637      -0.9670       
## year2020_team_MIN                    0.1854       1.3024       
## year2020_team_NE                    -0.0296      -0.1896       
## year2020_team_NO                     0.0398       0.2706       
## year2020_team_NYG                    0.0222       0.1456       
## year2020_team_SF                     0.0807       0.4840       
## year2020_team_WAS                    0.0726       0.4869       
## year2020_team_CHI                    0.0606       0.3822       
## year2020_team_DAL                    0.0237       0.1563       
## year2020_team_GB                     0.0260       0.1485       
## year2020_team_HOU                   -0.0292      -0.1832       
## year2020_team_MIA                   -0.1189      -0.7232       
## year2020_team_NYJ                    0.0038       0.0230       
## year2020_team_TB                     0.0899       0.5679       
## year2020_team_TEN                   -0.0712      -0.4328       
## year2020_team_ARI                    0.0992       0.5931       
## year2020_team_CLE                   -0.2083      -1.1630       
## year2020_team_IND                   -0.1550      -0.9242       
## year2020_team_LAC                    0.0821       0.4618       
## year2020_team_PHI                    0.1292       0.8936       
## year2020_team_SEA                   -0.0036      -0.0218       
## year2020_team_LV                     0.1393       0.9130       
## year2020_team_PIT                   -0.0749      -0.4616       
## year2021_team_ATL                   -0.1930      -1.5210      .
## year2021_team_BUF                    0.0550       0.4431       
## year2021_team_CIN                   -0.2421      -1.9551      *
## year2021_team_DAL                   -0.0415      -0.2989       
## year2021_team_DEN                    0.0827       0.5980       
## year2021_team_DET                   -0.0576      -0.4252       
## year2021_team_KC                     0.0562       0.4422       
## year2021_team_LA                     0.0028       0.0205       
## year2021_team_LV                     0.0840       0.5715       
## year2021_team_MIN                    0.0278       0.2135       
## year2021_team_NE                     0.0877       0.6308       
## year2021_team_NO                     0.0249       0.1860       
## year2021_team_NYG                    0.0285       0.2154       
## year2021_team_SF                     0.0131       0.0938       
## year2021_team_TEN                   -0.0258      -0.2104       
## year2021_team_ARI                    0.1309       1.0656       
## year2021_team_BAL                    0.1609       0.9048       
## year2021_team_CAR                   -0.0621      -0.5272       
## year2021_team_CHI                   -0.1964      -1.5608      .
## year2021_team_GB                     0.1260       1.0173       
## year2021_team_IND                    0.0062       0.0472       
## year2021_team_LAC                    0.0597       0.4084       
## year2021_team_MIA                    0.0374       0.2490       
## year2021_team_NYJ                    0.0140       0.0962       
## year2021_team_PHI                   -0.1664      -1.2907       
## year2021_team_SEA                   -0.1807      -1.2207       
## year2021_team_TB                     0.0446       0.3101       
## year2021_team_WAS                   -0.0503      -0.3983       
## year2021_team_CLE                   -0.0700      -0.5596       
## year2021_team_HOU                   -0.0285      -0.1963       
## year2021_team_JAX                   -0.0289      -0.1957       
## year2021_team_PIT                    0.0775       0.5797       
## year2022_team_ARI                   -0.1196      -0.9277       
## year2022_team_ATL                   -0.2428      -1.8050      *
## year2022_team_CAR                    0.1295       0.8687       
## year2022_team_CHI                   -0.0778      -0.4840       
## year2022_team_CIN                   -0.1108      -0.7292       
## year2022_team_HOU                   -0.0329      -0.2325       
## year2022_team_IND                   -0.0505      -0.3685       
## year2022_team_LAC                   -0.0931      -0.7135       
## year2022_team_MIA                   -0.1553      -1.2664       
## year2022_team_SEA                   -0.0170      -0.1282       
## year2022_team_TB                     0.0373       0.2843       
## year2022_team_TEN                    0.1890       1.6124      .
## year2022_team_WAS                    0.0042       0.0319       
## year2022_team_BAL                   -0.1624      -1.1349       
## year2022_team_BUF                    0.0691       0.5394       
## year2022_team_DAL                    0.0381       0.2278       
## year2022_team_DET                   -0.0865      -0.6922       
## year2022_team_GB                    -0.1059      -0.7555       
## year2022_team_JAX                   -0.1139      -0.9847       
## year2022_team_KC                    -0.1026      -0.5997       
## year2022_team_LA                     0.1752       1.3137       
## year2022_team_LV                     0.1914       1.2936       
## year2022_team_NO                    -0.0159      -0.1054       
## year2022_team_PHI                    0.0987       0.7894       
## year2022_team_PIT                    0.1898       1.4622      .
## year2022_team_DEN                    0.0860       0.6955       
## year2022_team_MIN                   -0.1202      -0.8010       
## year2022_team_NE                     0.0689       0.4774       
## year2022_team_NYJ                   -0.1152      -0.8885       
## year2022_team_NYG                   -0.0358      -0.2489       
## year2022_team_SF                    -0.1669      -1.0018       
## year2023_team_BAL                   -0.0399      -0.3046       
## year2023_team_CHI                   -0.1041      -0.7439       
## year2023_team_CLE                   -0.1239      -0.8759       
## year2023_team_GB                     0.0131       0.0981       
## year2023_team_IND                    0.1101       0.8411       
## year2023_team_KC                     0.0479       0.3367       
## year2023_team_LAC                    0.1141       0.8041       
## year2023_team_LV                     0.0355       0.2664       
## year2023_team_MIA                    0.0745       0.5630       
## year2023_team_MIN                    0.1859       1.5477      .
## year2023_team_NO                    -0.0383      -0.2676       
## year2023_team_NYG                    0.0798       0.5849       
## year2023_team_SEA                   -0.2476      -2.0465     **
## year2023_team_SF                     0.0707       0.4582       
## year2023_team_WAS                    0.2325       1.8472      *
## year2023_team_ATL                   -0.0709      -0.4869       
## year2023_team_BUF                   -0.0381      -0.2577       
## year2023_team_CAR                    0.0992       0.7985       
## year2023_team_DAL                    0.1406       0.9881       
## year2023_team_DEN                    0.0208       0.1598       
## year2023_team_HOU                   -0.0084      -0.0553       
## year2023_team_LA                     0.0560       0.3724       
## year2023_team_NE                     0.0786       0.5686       
## year2023_team_PHI                    0.0107       0.0779       
## year2023_team_PIT                    0.0472       0.3038       
## year2023_team_TEN                    0.0598       0.3966       
## year2023_team_ARI                   -0.1419      -0.9963       
## year2023_team_CIN                   -0.1332      -0.8790       
## year2023_team_DET                    0.0496       0.4022       
## year2023_team_TB                     0.0986       0.7184       
## year2023_team_JAX                   -0.0228      -0.1481       
## year2023_team_NYJ                    0.2342       1.6847      *
## is_first_half                       -0.0132      -0.7332       
## time_in_half                         0.0157       1.5813      .
## home_attendance                     -0.0293      -0.3881       
## GIMR                                 0.0487       1.9957     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1100651 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.37
## prev_singleback_rate                                   5.39
## cover1_rate                                            6.72
## cover3_rate                                            7.29
## home_attendance                                       13.97
## 
## 
##  ================================================================================ 
## MODEL: Starter Model with GIMR 
## ================================================================================ 
## 
## 
## Starter Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.3760       2.9639    ***
## ydstogo                             -0.1091     -12.6316    ***
## posteam_timeouts_remaining           0.0094       1.0257       
## defteam_timeouts_remaining           0.0109       1.2198       
## rush_attempt                         0.1430       7.5686    ***
## week                                 0.0023       0.2259       
## temp                                -0.0085      -0.7889       
## wind                                 0.0101       0.9357       
## vegas_wp                             0.0124       1.1240       
## spread_line                         -0.0077      -0.6187       
## total_line                           0.0354       2.7383    ***
## prep_days                            0.0078       0.9973       
## overall_win_pct                      0.0102       0.7773       
## team_win_pct                         0.0197       1.3486       
## prev_win_pct                        -0.0323      -2.4956     **
## prev_shotgun_rate                    0.0153       0.6863       
## prev_singleback_rate                 0.0109       0.6450       
## prev_empty_rate                      0.0114       0.9178       
## prev_iform_rate                      0.0082       0.5174       
## prev_shotgun_success                 0.0038       0.3145       
## prev_singleback_success              0.0083       0.6801       
## prev_empty_success                   0.0041       0.3663       
## prev_iform_success                   0.0258       2.5228     **
## prev_stop_rate_run                   0.0019       0.1690       
## prev_stop_rate_pass                 -0.0355      -3.4989    ***
## shotgun_rate                         0.0160       1.1458       
## singleback_rate                      0.0061       0.5029       
## empty_rate                          -0.0065      -0.5808       
## iform_rate                          -0.0154      -1.4410      .
## shotgun_success                     -0.0257      -2.8021    ***
## singleback_success                  -0.0164      -1.7510      *
## empty_success                       -0.0047      -0.4828       
## iform_success                       -0.0159      -1.6340      .
## def_stop_rate_run                    0.0136       1.4694      .
## def_stop_rate_pass                  -0.0116      -1.2292       
## avg_pass_rushers                    -0.0137      -1.2232       
## avg_box_defenders                   -0.0020      -0.1883       
## cover0_rate                         -0.0035      -0.3088       
## cover1_rate                         -0.0014      -0.0806       
## cover2_rate                         -0.0068      -0.5171       
## cover3_rate                          0.0197       1.0711       
## cover4_rate                          0.0100       0.7388       
## cover6_rate                         -0.0066      -0.5422       
## two_man_rate                         0.0158       1.6907      *
## prevent_rate                         0.0199       2.5231     **
## roof_outdoors                        0.0002       0.0070       
## posteam_type_home                   -0.0174      -1.0999       
## starter_QB_grades_pass_12w          -0.0029      -0.2099       
## starter_RB_grades_run_12w            0.0001       0.0136       
## starter_WR1_grades_offense_12w       0.0258       2.1291     **
## starter_WR2_grades_offense_12w      -0.0062      -0.5256       
## starter_WR3_grades_offense_12w      -0.0106      -1.0827       
## starter_TE1_grades_offense_12w      -0.0054      -0.5053       
## starter_DL1_grades_stops_12w         0.0020       0.2297       
## starter_DL1_productivity_stops_12w       0.0141       1.6592      *
## starter_DL2_grades_stops_12w         0.0095       1.1274       
## starter_DL2_productivity_stops_12w       0.0017       0.2090       
## starter_DL3_grades_stops_12w        -0.0036      -0.4206       
## starter_DL3_productivity_stops_12w       0.0033       0.3917       
## starter_DL4_grades_stops_12w        -0.0020      -0.2226       
## starter_DL4_productivity_stops_12w      -0.0010      -0.1163       
## starter_LB1_grades_stops_12w         0.0333       3.5190    ***
## starter_LB1_productivity_stops_12w       0.0128       1.3234       
## starter_LB1_zone_stops_12w          -0.0139      -1.4900      .
## starter_LB1_man_stops_12w            0.0015       0.1515       
## starter_LB2_grades_stops_12w         0.0123       1.2567       
## starter_LB2_productivity_stops_12w       0.0086       0.8672       
## starter_LB2_zone_stops_12w          -0.0115      -1.2241       
## starter_LB2_man_stops_12w            0.0130       1.3366       
## starter_LB3_grades_stops_12w         0.0179       1.7738      *
## starter_LB3_productivity_stops_12w       0.0139       1.4989      .
## starter_LB3_zone_stops_12w          -0.0059      -0.6053       
## starter_LB3_man_stops_12w           -0.0086      -0.8804       
## starter_LB4_grades_stops_12w        -0.0011      -0.1078       
## starter_LB4_productivity_stops_12w       0.0099       1.0167       
## starter_LB4_zone_stops_12w          -0.0156      -1.5283      .
## starter_LB4_man_stops_12w            0.0053       0.5399       
## starter_CB1_grades_stops_12w        -0.0087      -1.0377       
## starter_CB1_zone_stops_12w          -0.0178      -2.0384     **
## starter_CB1_man_stops_12w            0.0028       0.3362       
## starter_CB2_grades_stops_12w         0.0038       0.4598       
## starter_CB2_zone_stops_12w          -0.0008      -0.0889       
## starter_CB2_man_stops_12w           -0.0130      -1.5847      .
## starter_CB3_grades_stops_12w        -0.0167      -2.0105     **
## starter_CB3_zone_stops_12w          -0.0001      -0.0103       
## starter_CB3_man_stops_12w           -0.0088      -1.0355       
## starter_S1_grades_stops_12w          0.0011       0.1233       
## starter_S1_zone_stops_12w           -0.0028      -0.3113       
## starter_S1_man_stops_12w             0.0005       0.0555       
## starter_S2_grades_stops_12w          0.0078       0.8201       
## starter_S2_zone_stops_12w            0.0028       0.3061       
## starter_S2_man_stops_12w            -0.0040      -0.4679       
## starter_S3_grades_stops_12w          0.0181       1.9653     **
## starter_S3_zone_stops_12w           -0.0112      -1.2388       
## starter_S3_man_stops_12w            -0.0057      -0.6473       
## starter_OL_grades_offense_12w        0.0037       0.2349       
## yardline_1_10                       -0.0574      -2.2150     **
## yardline_11_20                       0.0079       0.2734       
## yardline_21_30                       0.0057       0.2031       
## yardline_41_50                       0.0473       1.9521      *
## yardline_51_60                       0.0155       0.5373       
## yardline_61_70                       0.0483       1.4845      .
## yardline_71_80                       0.0745       1.8573      *
## yardline_81_90                       0.1504       2.5571     **
## yardline_91_100                      0.1350       1.3061       
## year2017_team_ARI                    0.0665       0.3565       
## year2017_team_BUF                   -0.1135      -0.5760       
## year2017_team_CHI                    0.0208       0.1192       
## year2017_team_CLE                    0.1548       0.7518       
## year2017_team_DAL                   -0.1400      -0.8003       
## year2017_team_DET                   -0.0919      -0.5337       
## year2017_team_GB                     0.2821       1.6749      *
## year2017_team_HOU                    0.4209       1.9849     **
## year2017_team_MIA                   -0.1278      -0.7101       
## year2017_team_MIN                   -0.1400      -0.7511       
## year2017_team_NE                     0.0207       0.1095       
## year2017_team_SF                     0.4134       2.0781     **
## year2017_team_BAL                    0.0054       0.0276       
## year2017_team_DEN                   -0.0060      -0.0326       
## year2017_team_LA                     0.0577       0.3071       
## year2017_team_NYG                    0.0129       0.0722       
## year2017_team_OAK                    0.0531       0.2827       
## year2017_team_SEA                    0.1528       0.7994       
## year2017_team_CAR                    0.1390       0.6313       
## year2017_team_CIN                    0.1943       0.9339       
## year2017_team_IND                    0.1353       0.7525       
## year2017_team_NO                     0.0876       0.3926       
## year2017_team_PHI                    0.1378       0.7569       
## year2017_team_PIT                   -0.2220      -1.2590       
## year2017_team_TEN                    0.0830       0.3684       
## year2017_team_WAS                    0.0076       0.0397       
## year2017_team_KC                     0.2986       1.5039      .
## year2017_team_LAC                    0.0201       0.1047       
## year2017_team_NYJ                    0.1684       0.7944       
## year2017_team_TB                     0.0952       0.3990       
## year2017_team_ATL                   -0.0122      -0.0635       
## year2017_team_JAX                    0.0970       0.4692       
## year2018_team_ARI                    0.1000       0.6792       
## year2018_team_BAL                    0.1116       0.7505       
## year2018_team_CAR                    0.1119       0.7537       
## year2018_team_CLE                   -0.0323      -0.2338       
## year2018_team_DET                    0.0237       0.1633       
## year2018_team_HOU                    0.1941       1.1427       
## year2018_team_IND                   -0.0966      -0.6876       
## year2018_team_KC                     0.0572       0.4095       
## year2018_team_NYG                    0.1171       0.6537       
## year2018_team_OAK                   -0.0175      -0.1003       
## year2018_team_PHI                    0.1290       0.8795       
## year2018_team_SEA                   -0.0714      -0.4227       
## year2018_team_BUF                   -0.0104      -0.0650       
## year2018_team_CHI                   -0.0052      -0.0387       
## year2018_team_CIN                   -0.0172      -0.1043       
## year2018_team_DAL                    0.0549       0.3589       
## year2018_team_DEN                    0.0254       0.1687       
## year2018_team_GB                    -0.0346      -0.2033       
## year2018_team_LAC                    0.0926       0.6318       
## year2018_team_NE                    -0.1113      -0.7026       
## year2018_team_NO                     0.1379       0.9860       
## year2018_team_PIT                    0.0793       0.3982       
## year2018_team_SF                     0.0417       0.2525       
## year2018_team_MIA                    0.0502       0.3494       
## year2018_team_MIN                    0.0296       0.1812       
## year2018_team_NYJ                    0.1758       0.8203       
## year2018_team_TB                     0.0923       0.5584       
## year2018_team_ATL                    0.1206       0.8341       
## year2018_team_JAX                    0.1156       0.7594       
## year2018_team_LA                    -0.1749      -1.1035       
## year2018_team_TEN                    0.1955       1.1877       
## year2018_team_WAS                    0.0785       0.3995       
## year2019_team_ARI                   -0.0804      -0.5295       
## year2019_team_BUF                   -0.1241      -0.9616       
## year2019_team_CHI                    0.0882       0.5988       
## year2019_team_CLE                    0.1116       0.7175       
## year2019_team_DAL                   -0.0155      -0.0925       
## year2019_team_IND                   -0.0076      -0.0552       
## year2019_team_JAX                    0.1879       1.2180       
## year2019_team_KC                     0.0188       0.1393       
## year2019_team_LAC                   -0.0807      -0.5691       
## year2019_team_MIN                   -0.0690      -0.4908       
## year2019_team_NE                    -0.0455      -0.2702       
## year2019_team_NO                    -0.1280      -0.8334       
## year2019_team_PHI                    0.0862       0.5892       
## year2019_team_SEA                    0.0701       0.3566       
## year2019_team_SF                     0.0186       0.1356       
## year2019_team_TB                    -0.1220      -0.8532       
## year2019_team_BAL                    0.0638       0.4556       
## year2019_team_CAR                   -0.0057      -0.0348       
## year2019_team_DEN                    0.1429       0.9854       
## year2019_team_DET                   -0.1044      -0.6875       
## year2019_team_HOU                    0.0076       0.0509       
## year2019_team_LA                    -0.0844      -0.5151       
## year2019_team_MIA                   -0.3340      -2.0689     **
## year2019_team_NYG                   -0.1299      -0.8234       
## year2019_team_NYJ                   -0.2042      -1.5720      .
## year2019_team_OAK                    0.0643       0.3966       
## year2019_team_PIT                   -0.3141      -2.4318     **
## year2019_team_TEN                   -0.1390      -0.9632       
## year2019_team_CIN                    0.0934       0.6269       
## year2019_team_WAS                   -0.0774      -0.5124       
## year2019_team_ATL                    0.0272       0.1731       
## year2019_team_GB                    -0.0632      -0.4080       
## year2020_team_ATL                    0.1348       0.8524       
## year2020_team_BAL                    0.1375       0.8660       
## year2020_team_BUF                    0.0985       0.5336       
## year2020_team_CAR                    0.2145       1.3040       
## year2020_team_CIN                    0.1457       0.9848       
## year2020_team_DEN                   -0.0783      -0.4498       
## year2020_team_DET                   -0.0776      -0.4982       
## year2020_team_JAX                   -0.0306      -0.1924       
## year2020_team_KC                     0.0729       0.4385       
## year2020_team_LA                    -0.0895      -0.5266       
## year2020_team_MIN                    0.2337       1.6161      .
## year2020_team_NE                     0.0826       0.5266       
## year2020_team_NO                     0.0641       0.4273       
## year2020_team_NYG                    0.0778       0.5089       
## year2020_team_SF                     0.1254       0.7493       
## year2020_team_WAS                    0.0898       0.5921       
## year2020_team_CHI                    0.1122       0.7001       
## year2020_team_DAL                    0.0493       0.3288       
## year2020_team_GB                     0.1176       0.6389       
## year2020_team_HOU                   -0.1437      -0.8896       
## year2020_team_MIA                   -0.1033      -0.6155       
## year2020_team_NYJ                    0.1172       0.6905       
## year2020_team_TB                     0.1038       0.6292       
## year2020_team_TEN                   -0.0259      -0.1604       
## year2020_team_ARI                    0.1386       0.7919       
## year2020_team_CLE                   -0.1901      -1.0757       
## year2020_team_IND                   -0.0561      -0.3332       
## year2020_team_LAC                    0.0989       0.5585       
## year2020_team_PHI                    0.1678       1.1224       
## year2020_team_SEA                    0.0648       0.3770       
## year2020_team_LV                     0.1524       0.9662       
## year2020_team_PIT                   -0.0596      -0.3612       
## year2021_team_ATL                   -0.1692      -1.2900       
## year2021_team_BUF                    0.0671       0.5324       
## year2021_team_CIN                   -0.1260      -0.9784       
## year2021_team_DAL                   -0.0411      -0.2894       
## year2021_team_DEN                    0.1210       0.8757       
## year2021_team_DET                   -0.0400      -0.2918       
## year2021_team_KC                     0.0668       0.5349       
## year2021_team_LA                     0.0720       0.5256       
## year2021_team_LV                     0.0975       0.6681       
## year2021_team_MIN                   -0.0374      -0.2780       
## year2021_team_NE                     0.0650       0.4702       
## year2021_team_NO                     0.0361       0.2625       
## year2021_team_NYG                    0.0504       0.3776       
## year2021_team_SF                     0.0453       0.3184       
## year2021_team_TEN                    0.0192       0.1522       
## year2021_team_ARI                    0.1010       0.8180       
## year2021_team_BAL                    0.1950       1.0760       
## year2021_team_CAR                   -0.0294      -0.2426       
## year2021_team_CHI                   -0.2204      -1.6988      *
## year2021_team_GB                     0.1371       1.0850       
## year2021_team_IND                   -0.0280      -0.2013       
## year2021_team_LAC                    0.0826       0.5598       
## year2021_team_MIA                    0.0360       0.2324       
## year2021_team_NYJ                   -0.0082      -0.0565       
## year2021_team_PHI                   -0.1342      -1.0354       
## year2021_team_SEA                   -0.1571      -0.9843       
## year2021_team_TB                     0.0643       0.4573       
## year2021_team_WAS                   -0.0085      -0.0664       
## year2021_team_CLE                   -0.0224      -0.1773       
## year2021_team_HOU                   -0.0704      -0.4751       
## year2021_team_JAX                    0.0090       0.0616       
## year2021_team_PIT                    0.0731       0.5374       
## year2022_team_ARI                   -0.1077      -0.8214       
## year2022_team_ATL                   -0.2045      -1.5724      .
## year2022_team_CAR                    0.1445       0.9800       
## year2022_team_CHI                   -0.0346      -0.2203       
## year2022_team_CIN                   -0.0820      -0.5422       
## year2022_team_HOU                    0.0370       0.2635       
## year2022_team_IND                   -0.0626      -0.4636       
## year2022_team_LAC                   -0.1176      -0.8961       
## year2022_team_MIA                   -0.1505      -1.1997       
## year2022_team_SEA                   -0.0110      -0.0827       
## year2022_team_TB                     0.0634       0.4844       
## year2022_team_TEN                    0.2706       2.2756     **
## year2022_team_WAS                    0.0863       0.6631       
## year2022_team_BAL                   -0.1562      -1.0710       
## year2022_team_BUF                    0.0998       0.7416       
## year2022_team_DAL                    0.0611       0.3621       
## year2022_team_DET                   -0.0195      -0.1479       
## year2022_team_GB                    -0.0730      -0.5134       
## year2022_team_JAX                   -0.0972      -0.8389       
## year2022_team_KC                    -0.0609      -0.3678       
## year2022_team_LA                     0.2192       1.5836      .
## year2022_team_LV                     0.2320       1.5505      .
## year2022_team_NO                    -0.0045      -0.0284       
## year2022_team_PHI                    0.0958       0.7433       
## year2022_team_PIT                    0.2064       1.5832      .
## year2022_team_DEN                    0.1108       0.9029       
## year2022_team_MIN                   -0.0506      -0.3240       
## year2022_team_NE                     0.0721       0.5025       
## year2022_team_NYJ                   -0.0879      -0.6772       
## year2022_team_NYG                   -0.0231      -0.1601       
## year2022_team_SF                    -0.1431      -0.8540       
## year2023_team_BAL                    0.0284       0.2117       
## year2023_team_CHI                   -0.0611      -0.4501       
## year2023_team_CLE                   -0.1161      -0.7846       
## year2023_team_GB                     0.0468       0.3529       
## year2023_team_IND                    0.1107       0.8250       
## year2023_team_KC                     0.0798       0.5730       
## year2023_team_LAC                    0.0961       0.6639       
## year2023_team_LV                     0.1433       1.0671       
## year2023_team_MIA                    0.0239       0.1698       
## year2023_team_MIN                    0.2563       2.0818     **
## year2023_team_NO                     0.0023       0.0159       
## year2023_team_NYG                    0.0839       0.6043       
## year2023_team_SEA                   -0.2196      -1.7560      *
## year2023_team_SF                     0.1360       0.8754       
## year2023_team_WAS                    0.2376       1.8835      *
## year2023_team_ATL                   -0.0387      -0.2649       
## year2023_team_BUF                   -0.0269      -0.1770       
## year2023_team_CAR                    0.1483       1.1377       
## year2023_team_DAL                    0.1719       1.1804       
## year2023_team_DEN                    0.0383       0.2892       
## year2023_team_HOU                    0.0808       0.5620       
## year2023_team_LA                     0.0811       0.5272       
## year2023_team_NE                     0.0767       0.5733       
## year2023_team_PHI                   -0.0215      -0.1612       
## year2023_team_PIT                    0.0219       0.1365       
## year2023_team_TEN                    0.0626       0.4137       
## year2023_team_ARI                   -0.0550      -0.3728       
## year2023_team_CIN                   -0.0343      -0.2273       
## year2023_team_DET                    0.0675       0.5363       
## year2023_team_TB                     0.2219       1.5627      .
## year2023_team_JAX                    0.0047       0.0307       
## year2023_team_NYJ                    0.2567       1.8052      *
## is_first_half                       -0.0129      -0.7281       
## time_in_half                         0.0168       1.7153      *
## home_attendance                     -0.0113      -0.1511       
## GIMR                                 0.0493       2.0620     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1117406 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.87
## prev_singleback_rate                                   5.75
## prev_iform_rate                                        5.01
## cover1_rate                                            6.23
## cover3_rate                                            6.49
## starter_OL_grades_offense_12w                          5.01
## home_attendance                                       13.84
## 
## 
##  ================================================================================ 
## MODEL COMPARISON - Adjusted R-squared values
## ================================================================================ 
## 
## Player Model with GIMR: 0.1100651 
## Starter Model with GIMR: 0.1117406 
## 
## 
## ==================================================================================================== 
## ANALYZING DATASET 6/8: Defense Grades
## ==================================================================================================== 
## 
## Reading data: processed_predict_ccafd_def_grades.csv.csv.gz
## Reading data: processed_predict_ccfd_def_grades.csv.csv.gz
## 
## Phase 1: Validation Phase
## 
## Running 2 test iterations with best parameters...
## 
## Test Results over 2 iterations:
## Mean AUC: 0.8845494 
## SD AUC: 0.004346645 
## 95% CI: 0.87603 to 0.8930688 
## 
## 
##  ================================================================================ 
## MODEL: Player Model with GIMR 
## ================================================================================ 
## 
## 
## Player Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.4435       3.5915    ***
## ydstogo                             -0.1114     -12.6111    ***
## posteam_timeouts_remaining           0.0108       1.1823       
## defteam_timeouts_remaining           0.0102       1.1480       
## rush_attempt                         0.1540       7.8579    ***
## week                                 0.0070       0.7043       
## temp                                -0.0103      -0.9806       
## wind                                 0.0093       0.8799       
## vegas_wp                             0.0177       1.5771      .
## spread_line                         -0.0031      -0.2490       
## total_line                           0.0243       1.9230      *
## prep_days                            0.0076       0.9720       
## overall_win_pct                      0.0085       0.6428       
## team_win_pct                         0.0156       1.0879       
## prev_win_pct                        -0.0338      -2.6550    ***
## prev_shotgun_rate                    0.0113       0.5149       
## prev_singleback_rate                 0.0105       0.6337       
## prev_empty_rate                      0.0091       0.7553       
## prev_iform_rate                      0.0039       0.2510       
## prev_shotgun_success                 0.0019       0.1570       
## prev_singleback_success              0.0066       0.5638       
## prev_empty_success                   0.0057       0.5192       
## prev_iform_success                   0.0212       2.1311     **
## prev_stop_rate_run                   0.0004       0.0374       
## prev_stop_rate_pass                 -0.0345      -3.3712    ***
## shotgun_rate                         0.0120       0.8761       
## singleback_rate                      0.0021       0.1743       
## empty_rate                          -0.0048      -0.4363       
## iform_rate                          -0.0202      -1.9266      *
## shotgun_success                     -0.0186      -2.0765     **
## singleback_success                  -0.0085      -0.9252       
## empty_success                       -0.0086      -0.8851       
## iform_success                       -0.0142      -1.4766      .
## def_stop_rate_run                    0.0149       1.5744      .
## def_stop_rate_pass                  -0.0121      -1.2427       
## avg_pass_rushers                    -0.0071      -0.6375       
## avg_box_defenders                   -0.0054      -0.5006       
## cover0_rate                         -0.0030      -0.2619       
## cover1_rate                         -0.0072      -0.3979       
## cover2_rate                         -0.0017      -0.1288       
## cover3_rate                          0.0293       1.5921      .
## cover4_rate                          0.0138       1.0105       
## cover6_rate                         -0.0048      -0.3853       
## two_man_rate                         0.0133       1.3971       
## prevent_rate                         0.0203       2.5431     **
## roof_outdoors                       -0.0132      -0.5467       
## posteam_type_home                   -0.0213      -1.3644       
## QB_grades_pass_12w                   0.0111       1.3363       
## RB_grades_run_12w                    0.0051       0.6834       
## WR1_grades_offense_12w              -0.0128      -1.3816       
## WR2_grades_offense_12w              -0.0064      -0.6108       
## WR3_grades_offense_12w               0.0145       1.4281       
## TE1_grades_offense_12w               0.0130       1.5992      .
## DL1_grades_run_defense_12w          -0.0029      -0.2773       
## DL1_grades_pass_rush_defense_12w      -0.0147      -1.4165       
## DL2_grades_run_defense_12w           0.0104       0.5198       
## DL2_grades_pass_rush_defense_12w      -0.0081      -0.4077       
## DL3_grades_run_defense_12w          -0.0043      -0.1165       
## DL3_grades_pass_rush_defense_12w       0.0154       0.4226       
## DL4_grades_run_defense_12w          -0.0366      -0.7922       
## DL4_grades_pass_rush_defense_12w       0.0092       0.1967       
## LB1_grades_run_defense_12w           0.0038       0.3950       
## LB1_grades_coverage_defense_12w       0.0144       1.5722      .
## LB1_grades_pass_rush_defense_12w      -0.0129      -1.4678      .
## LB2_grades_run_defense_12w           0.0040       0.2173       
## LB2_grades_coverage_defense_12w       0.0278       1.5124      .
## LB2_grades_pass_rush_defense_12w      -0.0323      -1.9413      *
## LB3_grades_run_defense_12w          -0.0361      -1.0554       
## LB3_grades_coverage_defense_12w      -0.0298      -0.9029       
## LB3_grades_pass_rush_defense_12w       0.0517       1.6786      *
## LB4_grades_run_defense_12w           0.0228       0.6096       
## LB4_grades_coverage_defense_12w       0.0165       0.4523       
## LB4_grades_pass_rush_defense_12w      -0.0393      -1.2579       
## CB1_grades_run_defense_12w           0.0120       0.9513       
## CB1_grades_coverage_defense_12w      -0.0214      -1.7274      *
## CB2_grades_run_defense_12w          -0.0044      -0.2760       
## CB2_grades_coverage_defense_12w      -0.0039      -0.2411       
## CB3_grades_run_defense_12w           0.0054       0.1838       
## CB3_grades_coverage_defense_12w       0.0108       0.3678       
## S1_grades_run_defense_12w           -0.0124      -1.1519       
## S1_grades_coverage_defense_12w       0.0042       0.3831       
## S2_grades_run_defense_12w           -0.0208      -0.9076       
## S2_grades_coverage_defense_12w       0.0267       1.1618       
## S3_grades_run_defense_12w           -0.0178      -0.4602       
## S3_grades_coverage_defense_12w       0.0258       0.6699       
## OL_grades_offense_12w               -0.0063      -0.7726       
## yardline_1_10                       -0.0626      -2.3373     **
## yardline_11_20                       0.0104       0.3588       
## yardline_21_30                       0.0017       0.0622       
## yardline_41_50                       0.0473       1.9534      *
## yardline_51_60                       0.0165       0.5700       
## yardline_61_70                       0.0494       1.5211      .
## yardline_71_80                       0.0701       1.7490      *
## yardline_81_90                       0.1294       2.1702     **
## yardline_91_100                      0.0841       0.8290       
## year2017_team_ARI                    0.0762       0.4088       
## year2017_team_BUF                   -0.1265      -0.6541       
## year2017_team_CHI                   -0.0093      -0.0537       
## year2017_team_CLE                    0.1689       0.8547       
## year2017_team_DAL                   -0.1626      -0.9493       
## year2017_team_DET                   -0.0655      -0.3812       
## year2017_team_GB                     0.3327       2.0467     **
## year2017_team_HOU                    0.3404       1.6366      .
## year2017_team_MIA                   -0.2151      -1.2216       
## year2017_team_MIN                   -0.0954      -0.5382       
## year2017_team_NE                     0.0030       0.0163       
## year2017_team_SF                     0.3888       2.0151     **
## year2017_team_BAL                    0.0053       0.0271       
## year2017_team_DEN                    0.0018       0.0100       
## year2017_team_LA                     0.0335       0.1838       
## year2017_team_NYG                   -0.0549      -0.3239       
## year2017_team_OAK                   -0.0870      -0.4872       
## year2017_team_SEA                    0.1174       0.6325       
## year2017_team_CAR                    0.1101       0.5225       
## year2017_team_CIN                    0.1690       0.8426       
## year2017_team_IND                    0.1577       0.8814       
## year2017_team_NO                     0.1233       0.5535       
## year2017_team_PHI                    0.0214       0.1199       
## year2017_team_PIT                   -0.1520      -0.8969       
## year2017_team_TEN                    0.1087       0.5013       
## year2017_team_WAS                    0.0292       0.1512       
## year2017_team_KC                     0.2538       1.3031       
## year2017_team_LAC                   -0.0145      -0.0775       
## year2017_team_NYJ                    0.1748       0.8211       
## year2017_team_TB                     0.0365       0.1581       
## year2017_team_ATL                   -0.0176      -0.0921       
## year2017_team_JAX                    0.0705       0.3528       
## year2018_team_ARI                    0.0590       0.4018       
## year2018_team_BAL                    0.0498       0.3428       
## year2018_team_CAR                    0.0135       0.0955       
## year2018_team_CLE                   -0.0568      -0.4036       
## year2018_team_DET                    0.0963       0.6902       
## year2018_team_HOU                    0.2163       1.3500       
## year2018_team_IND                   -0.1334      -0.9865       
## year2018_team_KC                     0.1051       0.7726       
## year2018_team_NYG                    0.0907       0.5322       
## year2018_team_OAK                   -0.1248      -0.7516       
## year2018_team_PHI                    0.0605       0.4200       
## year2018_team_SEA                   -0.1114      -0.6481       
## year2018_team_BUF                   -0.1330      -0.8429       
## year2018_team_CHI                   -0.0235      -0.1830       
## year2018_team_CIN                   -0.0714      -0.4349       
## year2018_team_DAL                   -0.0576      -0.3907       
## year2018_team_DEN                    0.0168       0.1164       
## year2018_team_GB                    -0.0160      -0.0957       
## year2018_team_LAC                    0.0165       0.1131       
## year2018_team_NE                    -0.0950      -0.6101       
## year2018_team_NO                     0.0741       0.5538       
## year2018_team_PIT                    0.0775       0.4138       
## year2018_team_SF                     0.0176       0.1192       
## year2018_team_MIA                    0.0799       0.5639       
## year2018_team_MIN                    0.0148       0.0957       
## year2018_team_NYJ                    0.1554       0.6906       
## year2018_team_TB                     0.0308       0.1874       
## year2018_team_ATL                    0.0673       0.4928       
## year2018_team_JAX                    0.0539       0.3531       
## year2018_team_LA                    -0.1900      -1.2106       
## year2018_team_TEN                    0.1022       0.6342       
## year2018_team_WAS                    0.0286       0.1459       
## year2019_team_ARI                   -0.1053      -0.6873       
## year2019_team_BUF                   -0.1392      -1.1012       
## year2019_team_CHI                    0.0692       0.4853       
## year2019_team_CLE                    0.0845       0.5791       
## year2019_team_DAL                   -0.0697      -0.4269       
## year2019_team_IND                   -0.0669      -0.5081       
## year2019_team_JAX                    0.0673       0.4454       
## year2019_team_KC                    -0.0221      -0.1657       
## year2019_team_LAC                   -0.1004      -0.6841       
## year2019_team_MIN                   -0.1006      -0.7061       
## year2019_team_NE                    -0.0381      -0.2305       
## year2019_team_NO                    -0.2025      -1.3412       
## year2019_team_PHI                    0.0176       0.1201       
## year2019_team_SEA                    0.0278       0.1455       
## year2019_team_SF                    -0.0340      -0.2569       
## year2019_team_TB                    -0.1405      -1.0338       
## year2019_team_BAL                    0.0122       0.0876       
## year2019_team_CAR                   -0.1041      -0.6376       
## year2019_team_DEN                    0.1115       0.8031       
## year2019_team_DET                   -0.1247      -0.8289       
## year2019_team_HOU                   -0.0220      -0.1479       
## year2019_team_LA                    -0.1068      -0.6755       
## year2019_team_MIA                   -0.3412      -2.1844     **
## year2019_team_NYG                   -0.1469      -0.9078       
## year2019_team_NYJ                   -0.2417      -1.8813      *
## year2019_team_OAK                   -0.0588      -0.3845       
## year2019_team_PIT                   -0.2979      -2.5369     **
## year2019_team_TEN                   -0.1626      -1.1567       
## year2019_team_CIN                    0.0497       0.3541       
## year2019_team_WAS                   -0.0571      -0.3818       
## year2019_team_ATL                   -0.0126      -0.0796       
## year2019_team_GB                    -0.0587      -0.4013       
## year2020_team_ATL                    0.0339       0.2234       
## year2020_team_BAL                    0.0571       0.3733       
## year2020_team_BUF                   -0.0208      -0.1137       
## year2020_team_CAR                    0.1112       0.6946       
## year2020_team_CIN                    0.1015       0.6829       
## year2020_team_DEN                   -0.0942      -0.5694       
## year2020_team_DET                   -0.1332      -0.8653       
## year2020_team_JAX                   -0.1229      -0.7683       
## year2020_team_KC                     0.0069       0.0435       
## year2020_team_LA                    -0.2062      -1.1804       
## year2020_team_MIN                    0.1381       0.9812       
## year2020_team_NE                    -0.0565      -0.3644       
## year2020_team_NO                     0.0354       0.2470       
## year2020_team_NYG                   -0.0131      -0.0882       
## year2020_team_SF                     0.0550       0.3347       
## year2020_team_WAS                    0.0115       0.0798       
## year2020_team_CHI                    0.0437       0.2773       
## year2020_team_DAL                   -0.0451      -0.3019       
## year2020_team_GB                    -0.0230      -0.1326       
## year2020_team_HOU                   -0.1097      -0.7005       
## year2020_team_MIA                   -0.1669      -1.0260       
## year2020_team_NYJ                   -0.0239      -0.1440       
## year2020_team_TB                     0.0233       0.1467       
## year2020_team_TEN                   -0.1032      -0.6345       
## year2020_team_ARI                    0.0697       0.4162       
## year2020_team_CLE                   -0.2942      -1.6946      *
## year2020_team_IND                   -0.1736      -1.0596       
## year2020_team_LAC                    0.0038       0.0212       
## year2020_team_PHI                    0.0756       0.5247       
## year2020_team_SEA                   -0.0528      -0.3270       
## year2020_team_LV                     0.0890       0.5815       
## year2020_team_PIT                   -0.1082      -0.6509       
## year2021_team_ATL                   -0.2253      -1.7911      *
## year2021_team_BUF                    0.0502       0.4059       
## year2021_team_CIN                   -0.2322      -1.9624     **
## year2021_team_DAL                   -0.0981      -0.7024       
## year2021_team_DEN                    0.0555       0.4085       
## year2021_team_DET                   -0.0763      -0.5782       
## year2021_team_KC                     0.0110       0.0895       
## year2021_team_LA                     0.0056       0.0423       
## year2021_team_LV                     0.0452       0.3130       
## year2021_team_MIN                   -0.0381      -0.2997       
## year2021_team_NE                     0.0558       0.4079       
## year2021_team_NO                    -0.0375      -0.2822       
## year2021_team_NYG                   -0.0004      -0.0033       
## year2021_team_SF                    -0.0191      -0.1403       
## year2021_team_TEN                   -0.0655      -0.5315       
## year2021_team_ARI                    0.0883       0.7437       
## year2021_team_BAL                    0.1301       0.7382       
## year2021_team_CAR                   -0.0818      -0.7029       
## year2021_team_CHI                   -0.2050      -1.6455      *
## year2021_team_GB                     0.0962       0.7847       
## year2021_team_IND                   -0.0344      -0.2631       
## year2021_team_LAC                    0.0327       0.2268       
## year2021_team_MIA                    0.0118       0.0787       
## year2021_team_NYJ                   -0.0326      -0.2216       
## year2021_team_PHI                   -0.1853      -1.4969      .
## year2021_team_SEA                   -0.1992      -1.3300       
## year2021_team_TB                     0.0508       0.3643       
## year2021_team_WAS                   -0.0753      -0.6188       
## year2021_team_CLE                   -0.0964      -0.7761       
## year2021_team_HOU                   -0.1007      -0.7079       
## year2021_team_JAX                   -0.0652      -0.4483       
## year2021_team_PIT                    0.0395       0.2978       
## year2022_team_ARI                   -0.1519      -1.1758       
## year2022_team_ATL                   -0.2911      -2.2051     **
## year2022_team_CAR                    0.0858       0.5880       
## year2022_team_CHI                   -0.0858      -0.5250       
## year2022_team_CIN                   -0.1384      -0.9431       
## year2022_team_HOU                   -0.0417      -0.3048       
## year2022_team_IND                   -0.1167      -0.8809       
## year2022_team_LAC                   -0.0930      -0.7080       
## year2022_team_MIA                   -0.1786      -1.4789      .
## year2022_team_SEA                   -0.0537      -0.4094       
## year2022_team_TB                     0.0014       0.0110       
## year2022_team_TEN                    0.1474       1.2764       
## year2022_team_WAS                   -0.0064      -0.0496       
## year2022_team_BAL                   -0.2054      -1.4208       
## year2022_team_BUF                    0.0341       0.2704       
## year2022_team_DAL                   -0.0123      -0.0736       
## year2022_team_DET                   -0.0918      -0.7386       
## year2022_team_GB                    -0.1367      -0.9838       
## year2022_team_JAX                   -0.1284      -1.1458       
## year2022_team_KC                    -0.1521      -0.8904       
## year2022_team_LA                     0.1634       1.2353       
## year2022_team_LV                     0.1356       0.9386       
## year2022_team_NO                    -0.0605      -0.3885       
## year2022_team_PHI                    0.0666       0.5297       
## year2022_team_PIT                    0.1712       1.3349       
## year2022_team_DEN                    0.0165       0.1386       
## year2022_team_MIN                   -0.1217      -0.7907       
## year2022_team_NE                     0.0160       0.1127       
## year2022_team_NYJ                   -0.1247      -0.9784       
## year2022_team_NYG                   -0.0713      -0.4933       
## year2022_team_SF                    -0.2069      -1.1865       
## year2023_team_BAL                   -0.0704      -0.5454       
## year2023_team_CHI                   -0.1632      -1.2013       
## year2023_team_CLE                   -0.1369      -0.9373       
## year2023_team_GB                     0.0056       0.0428       
## year2023_team_IND                    0.0700       0.5532       
## year2023_team_KC                     0.0205       0.1476       
## year2023_team_LAC                    0.0546       0.3853       
## year2023_team_LV                     0.0093       0.0745       
## year2023_team_MIA                    0.0385       0.2909       
## year2023_team_MIN                    0.1188       0.9988       
## year2023_team_NO                    -0.0778      -0.5433       
## year2023_team_NYG                    0.0498       0.3781       
## year2023_team_SEA                   -0.2809      -2.3306     **
## year2023_team_SF                     0.0062       0.0400       
## year2023_team_WAS                    0.1788       1.4569      .
## year2023_team_ATL                   -0.1012      -0.7040       
## year2023_team_BUF                   -0.1013      -0.6873       
## year2023_team_CAR                    0.0611       0.4894       
## year2023_team_DAL                    0.0899       0.6377       
## year2023_team_DEN                    0.0144       0.1128       
## year2023_team_HOU                   -0.0401      -0.2692       
## year2023_team_LA                    -0.0007      -0.0047       
## year2023_team_NE                     0.0153       0.1167       
## year2023_team_PHI                   -0.0474      -0.3644       
## year2023_team_PIT                   -0.0060      -0.0378       
## year2023_team_TEN                   -0.0008      -0.0057       
## year2023_team_ARI                   -0.1894      -1.3669       
## year2023_team_CIN                   -0.1582      -1.0306       
## year2023_team_DET                    0.0053       0.0431       
## year2023_team_TB                     0.0998       0.7435       
## year2023_team_JAX                   -0.0973      -0.6585       
## year2023_team_NYJ                    0.1801       1.3302       
## is_first_half                       -0.0103      -0.5732       
## time_in_half                         0.0162       1.6457      *
## home_attendance                     -0.0302      -0.4067       
## GIMR                                 0.0547       2.2450     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1110219 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.33
## prev_singleback_rate                                   5.39
## cover1_rate                                            6.13
## cover3_rate                                            6.46
## DL2_grades_run_defense_12w                             7.92
## DL2_grades_pass_rush_defense_12w                       7.92
## DL3_grades_run_defense_12w                            25.22
## DL3_grades_pass_rush_defense_12w                      25.04
## DL4_grades_run_defense_12w                            38.50
## DL4_grades_pass_rush_defense_12w                      39.42
## LB2_grades_run_defense_12w                             7.04
## LB2_grades_coverage_defense_12w                        7.13
## LB2_grades_pass_rush_defense_12w                       5.57
## LB3_grades_run_defense_12w                            23.12
## LB3_grades_coverage_defense_12w                       22.15
## LB3_grades_pass_rush_defense_12w                      17.86
## LB4_grades_run_defense_12w                            28.86
## LB4_grades_coverage_defense_12w                       29.37
## LB4_grades_pass_rush_defense_12w                      24.31
## CB2_grades_run_defense_12w                             5.23
## CB2_grades_coverage_defense_12w                        5.43
## CB3_grades_run_defense_12w                            16.21
## CB3_grades_coverage_defense_12w                       16.29
## S2_grades_run_defense_12w                             10.73
## S2_grades_coverage_defense_12w                        10.79
## S3_grades_run_defense_12w                             30.24
## S3_grades_coverage_defense_12w                        30.41
## home_attendance                                       13.83
## 
## 
##  ================================================================================ 
## MODEL: Starter Model with GIMR 
## ================================================================================ 
## 
## 
## Starter Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.4769       3.7579    ***
## ydstogo                             -0.1110     -12.8625    ***
## posteam_timeouts_remaining           0.0122       1.3300       
## defteam_timeouts_remaining           0.0082       0.9240       
## rush_attempt                         0.1377       7.2711    ***
## week                                 0.0062       0.6171       
## temp                                -0.0088      -0.8288       
## wind                                 0.0073       0.6823       
## vegas_wp                             0.0108       0.9842       
## spread_line                         -0.0042      -0.3348       
## total_line                           0.0271       2.0383     **
## prep_days                            0.0070       0.8982       
## overall_win_pct                      0.0100       0.7629       
## team_win_pct                         0.0174       1.2039       
## prev_win_pct                        -0.0351      -2.7405    ***
## prev_shotgun_rate                    0.0188       0.8446       
## prev_singleback_rate                 0.0127       0.7658       
## prev_empty_rate                      0.0159       1.2949       
## prev_iform_rate                      0.0065       0.4102       
## prev_shotgun_success                 0.0056       0.4602       
## prev_singleback_success              0.0106       0.8839       
## prev_empty_success                   0.0007       0.0665       
## prev_iform_success                   0.0243       2.3896     **
## prev_stop_rate_run                   0.0004       0.0348       
## prev_stop_rate_pass                 -0.0380      -3.7467    ***
## shotgun_rate                         0.0124       0.8890       
## singleback_rate                      0.0047       0.3846       
## empty_rate                          -0.0048      -0.4285       
## iform_rate                          -0.0161      -1.5000      .
## shotgun_success                     -0.0208      -2.3117     **
## singleback_success                  -0.0120      -1.2860       
## empty_success                       -0.0081      -0.8236       
## iform_success                       -0.0117      -1.1849       
## def_stop_rate_run                    0.0178       1.8889      *
## def_stop_rate_pass                  -0.0150      -1.5786      .
## avg_pass_rushers                    -0.0123      -1.1023       
## avg_box_defenders                   -0.0036      -0.3408       
## cover0_rate                         -0.0051      -0.4472       
## cover1_rate                         -0.0078      -0.4352       
## cover2_rate                         -0.0025      -0.1911       
## cover3_rate                          0.0219       1.1839       
## cover4_rate                          0.0129       0.9567       
## cover6_rate                         -0.0076      -0.6307       
## two_man_rate                         0.0163       1.7244      *
## prevent_rate                         0.0202       2.5023     **
## roof_outdoors                       -0.0007      -0.0269       
## posteam_type_home                   -0.0224      -1.4164       
## starter_QB_grades_pass_12w          -0.0008      -0.0562       
## starter_RB_grades_run_12w            0.0048       0.5028       
## starter_WR1_grades_offense_12w       0.0287       2.2506     **
## starter_WR2_grades_offense_12w      -0.0051      -0.4253       
## starter_WR3_grades_offense_12w      -0.0124      -1.2502       
## starter_TE1_grades_offense_12w      -0.0031      -0.2903       
## starter_DL1_grades_run_defense_12w      -0.0004      -0.0260       
## starter_DL1_grades_pass_rush_defense_12w       0.0044       0.3090       
## starter_DL2_grades_run_defense_12w       0.0269       1.9143      *
## starter_DL2_grades_pass_rush_defense_12w      -0.0182      -1.3342       
## starter_DL3_grades_run_defense_12w      -0.0045      -0.3098       
## starter_DL3_grades_pass_rush_defense_12w      -0.0013      -0.0906       
## starter_DL4_grades_run_defense_12w       0.0124       0.9057       
## starter_DL4_grades_pass_rush_defense_12w      -0.0053      -0.3865       
## starter_LB1_grades_run_defense_12w       0.0232       1.8036      *
## starter_LB1_grades_coverage_defense_12w      -0.0205      -1.6927      *
## starter_LB1_grades_pass_rush_defense_12w       0.0142       1.2677       
## starter_LB2_grades_run_defense_12w       0.0231       1.7892      *
## starter_LB2_grades_coverage_defense_12w      -0.0214      -1.7693      *
## starter_LB2_grades_pass_rush_defense_12w       0.0136       1.2399       
## starter_LB3_grades_run_defense_12w      -0.0027      -0.2016       
## starter_LB3_grades_coverage_defense_12w       0.0022       0.1736       
## starter_LB3_grades_pass_rush_defense_12w       0.0064       0.5482       
## starter_LB4_grades_run_defense_12w      -0.0212      -1.7387      *
## starter_LB4_grades_coverage_defense_12w       0.0055       0.4504       
## starter_LB4_grades_pass_rush_defense_12w       0.0045       0.4113       
## starter_CB1_grades_run_defense_12w      -0.0110      -0.7881       
## starter_CB1_grades_coverage_defense_12w      -0.0023      -0.1687       
## starter_CB2_grades_run_defense_12w       0.0275       2.1441     **
## starter_CB2_grades_coverage_defense_12w      -0.0182      -1.4110       
## starter_CB3_grades_run_defense_12w      -0.0115      -1.1097       
## starter_CB3_grades_coverage_defense_12w      -0.0066      -0.6035       
## starter_S1_grades_run_defense_12w       0.0009       0.0627       
## starter_S1_grades_coverage_defense_12w      -0.0031      -0.2202       
## starter_S2_grades_run_defense_12w      -0.0104      -0.7395       
## starter_S2_grades_coverage_defense_12w      -0.0071      -0.5576       
## starter_S3_grades_run_defense_12w       0.0034       0.2699       
## starter_S3_grades_coverage_defense_12w      -0.0006      -0.0475       
## starter_OL_grades_offense_12w       -0.0018      -0.1011       
## yardline_1_10                       -0.0645      -2.4929     **
## yardline_11_20                       0.0008       0.0262       
## yardline_21_30                      -0.0005      -0.0164       
## yardline_41_50                       0.0433       1.7835      *
## yardline_51_60                       0.0108       0.3733       
## yardline_61_70                       0.0450       1.3885       
## yardline_71_80                       0.0699       1.7456      *
## yardline_81_90                       0.1318       2.2055     **
## yardline_91_100                      0.1174       1.1130       
## year2017_team_ARI                    0.0136       0.0730       
## year2017_team_BUF                   -0.1658      -0.8507       
## year2017_team_CHI                   -0.0930      -0.5287       
## year2017_team_CLE                    0.0438       0.2154       
## year2017_team_DAL                   -0.1648      -0.9439       
## year2017_team_DET                   -0.1340      -0.7746       
## year2017_team_GB                     0.2423       1.4532      .
## year2017_team_HOU                    0.3308       1.5932      .
## year2017_team_MIA                   -0.2526      -1.4171       
## year2017_team_MIN                   -0.1857      -1.0156       
## year2017_team_NE                    -0.0525      -0.2781       
## year2017_team_SF                     0.3586       1.7373      *
## year2017_team_BAL                   -0.0588      -0.3002       
## year2017_team_DEN                   -0.0976      -0.5316       
## year2017_team_LA                     0.0342       0.1866       
## year2017_team_NYG                   -0.0973      -0.5528       
## year2017_team_OAK                   -0.0596      -0.3165       
## year2017_team_SEA                    0.0713       0.3751       
## year2017_team_CAR                    0.0133       0.0609       
## year2017_team_CIN                    0.0704       0.3431       
## year2017_team_IND                    0.0901       0.4820       
## year2017_team_NO                     0.0248       0.1138       
## year2017_team_PHI                   -0.0215      -0.1195       
## year2017_team_PIT                   -0.1952      -1.1318       
## year2017_team_TEN                   -0.0123      -0.0570       
## year2017_team_WAS                   -0.0127      -0.0660       
## year2017_team_KC                     0.2446       1.2619       
## year2017_team_LAC                   -0.0670      -0.3507       
## year2017_team_NYJ                    0.0503       0.2321       
## year2017_team_TB                     0.0546       0.2256       
## year2017_team_ATL                   -0.1001      -0.5160       
## year2017_team_JAX                    0.0344       0.1677       
## year2018_team_ARI                    0.0232       0.1524       
## year2018_team_BAL                    0.0825       0.5568       
## year2018_team_CAR                    0.0196       0.1309       
## year2018_team_CLE                   -0.0773      -0.5526       
## year2018_team_DET                   -0.0041      -0.0275       
## year2018_team_HOU                    0.1327       0.8171       
## year2018_team_IND                   -0.1695      -1.1727       
## year2018_team_KC                    -0.0129      -0.0909       
## year2018_team_NYG                    0.0351       0.1942       
## year2018_team_OAK                   -0.0833      -0.4898       
## year2018_team_PHI                    0.0471       0.3177       
## year2018_team_SEA                   -0.1502      -0.8905       
## year2018_team_BUF                   -0.1012      -0.6357       
## year2018_team_CHI                   -0.0494      -0.3728       
## year2018_team_CIN                   -0.1144      -0.6810       
## year2018_team_DAL                   -0.0791      -0.5291       
## year2018_team_DEN                   -0.0828      -0.5531       
## year2018_team_GB                    -0.0936      -0.5478       
## year2018_team_LAC                    0.0451       0.3109       
## year2018_team_NE                    -0.1407      -0.8810       
## year2018_team_NO                     0.0647       0.4596       
## year2018_team_PIT                    0.0423       0.2151       
## year2018_team_SF                    -0.0338      -0.2123       
## year2018_team_MIA                    0.0081       0.0548       
## year2018_team_MIN                   -0.0131      -0.0823       
## year2018_team_NYJ                    0.1362       0.6119       
## year2018_team_TB                     0.0081       0.0486       
## year2018_team_ATL                    0.0267       0.1843       
## year2018_team_JAX                    0.0104       0.0686       
## year2018_team_LA                    -0.2069      -1.2885       
## year2018_team_TEN                    0.0973       0.5719       
## year2018_team_WAS                   -0.0435      -0.2312       
## year2019_team_ARI                   -0.1577      -1.0130       
## year2019_team_BUF                   -0.1542      -1.1986       
## year2019_team_CHI                   -0.0066      -0.0444       
## year2019_team_CLE                    0.0218       0.1361       
## year2019_team_DAL                   -0.0883      -0.5216       
## year2019_team_IND                   -0.1116      -0.8241       
## year2019_team_JAX                    0.0608       0.3841       
## year2019_team_KC                    -0.0388      -0.2827       
## year2019_team_LAC                   -0.1641      -1.1651       
## year2019_team_MIN                   -0.1805      -1.2688       
## year2019_team_NE                    -0.0672      -0.3977       
## year2019_team_NO                    -0.2570      -1.6435      .
## year2019_team_PHI                   -0.0012      -0.0081       
## year2019_team_SEA                   -0.0450      -0.2350       
## year2019_team_SF                    -0.0715      -0.5191       
## year2019_team_TB                    -0.2046      -1.4387       
## year2019_team_BAL                    0.0040       0.0272       
## year2019_team_CAR                   -0.1442      -0.8792       
## year2019_team_DEN                    0.0548       0.3809       
## year2019_team_DET                   -0.1548      -1.0169       
## year2019_team_HOU                   -0.0921      -0.6279       
## year2019_team_LA                    -0.2035      -1.2635       
## year2019_team_MIA                   -0.3805      -2.3682     **
## year2019_team_NYG                   -0.2173      -1.3568       
## year2019_team_NYJ                   -0.2826      -2.1007     **
## year2019_team_OAK                   -0.0504      -0.3143       
## year2019_team_PIT                   -0.4306      -3.4838    ***
## year2019_team_TEN                   -0.2174      -1.5187      .
## year2019_team_CIN                    0.0321       0.2166       
## year2019_team_WAS                   -0.1141      -0.7462       
## year2019_team_ATL                   -0.0427      -0.2758       
## year2019_team_GB                    -0.1151      -0.7613       
## year2020_team_ATL                    0.0461       0.2890       
## year2020_team_BAL                    0.0486       0.3137       
## year2020_team_BUF                    0.0030       0.0159       
## year2020_team_CAR                    0.1331       0.8078       
## year2020_team_CIN                    0.0471       0.3144       
## year2020_team_DEN                   -0.0863      -0.4851       
## year2020_team_DET                   -0.1842      -1.2077       
## year2020_team_JAX                   -0.1233      -0.7594       
## year2020_team_KC                    -0.0060      -0.0359       
## year2020_team_LA                    -0.2210      -1.2774       
## year2020_team_MIN                    0.1271       0.8786       
## year2020_team_NE                    -0.0499      -0.3218       
## year2020_team_NO                    -0.0035      -0.0233       
## year2020_team_NYG                   -0.0706      -0.4488       
## year2020_team_SF                     0.0342       0.2038       
## year2020_team_WAS                   -0.0038      -0.0246       
## year2020_team_CHI                    0.0480       0.3042       
## year2020_team_DAL                   -0.0758      -0.5022       
## year2020_team_GB                    -0.0140      -0.0777       
## year2020_team_HOU                   -0.1865      -1.1592       
## year2020_team_MIA                   -0.1697      -0.9990       
## year2020_team_NYJ                   -0.0360      -0.2107       
## year2020_team_TB                     0.0281       0.1737       
## year2020_team_TEN                   -0.1316      -0.8033       
## year2020_team_ARI                    0.0595       0.3425       
## year2020_team_CLE                   -0.3223      -1.8340      *
## year2020_team_IND                   -0.1760      -1.0507       
## year2020_team_LAC                   -0.0114      -0.0634       
## year2020_team_PHI                    0.0650       0.4377       
## year2020_team_SEA                   -0.0797      -0.4752       
## year2020_team_LV                     0.0682       0.4437       
## year2020_team_PIT                   -0.1433      -0.8681       
## year2021_team_ATL                   -0.2818      -2.1511     **
## year2021_team_BUF                   -0.0234      -0.1844       
## year2021_team_CIN                   -0.2434      -1.8704      *
## year2021_team_DAL                   -0.1488      -1.0459       
## year2021_team_DEN                    0.0518       0.3805       
## year2021_team_DET                   -0.1808      -1.3036       
## year2021_team_KC                    -0.0097      -0.0771       
## year2021_team_LA                    -0.0408      -0.3034       
## year2021_team_LV                     0.0089       0.0617       
## year2021_team_MIN                   -0.1081      -0.8086       
## year2021_team_NE                     0.0219       0.1586       
## year2021_team_NO                    -0.0446      -0.3273       
## year2021_team_NYG                   -0.0172      -0.1262       
## year2021_team_SF                    -0.0520      -0.3705       
## year2021_team_TEN                   -0.0544      -0.4286       
## year2021_team_ARI                    0.0751       0.6106       
## year2021_team_BAL                    0.0783       0.4388       
## year2021_team_CAR                   -0.0747      -0.6277       
## year2021_team_CHI                   -0.2819      -2.1899     **
## year2021_team_GB                     0.0341       0.2750       
## year2021_team_IND                   -0.1051      -0.7756       
## year2021_team_LAC                   -0.0214      -0.1445       
## year2021_team_MIA                   -0.0201      -0.1321       
## year2021_team_NYJ                   -0.1029      -0.6995       
## year2021_team_PHI                   -0.2392      -1.8626      *
## year2021_team_SEA                   -0.2573      -1.6271      .
## year2021_team_TB                    -0.0047      -0.0335       
## year2021_team_WAS                   -0.1162      -0.9110       
## year2021_team_CLE                   -0.1077      -0.8612       
## year2021_team_HOU                   -0.1270      -0.8692       
## year2021_team_JAX                   -0.0832      -0.5648       
## year2021_team_PIT                    0.0094       0.0693       
## year2022_team_ARI                   -0.1977      -1.5190      .
## year2022_team_ATL                   -0.3042      -2.3374     **
## year2022_team_CAR                    0.0759       0.5149       
## year2022_team_CHI                   -0.0998      -0.6013       
## year2022_team_CIN                   -0.1192      -0.7992       
## year2022_team_HOU                   -0.0729      -0.5252       
## year2022_team_IND                   -0.1256      -0.9148       
## year2022_team_LAC                   -0.1230      -0.9102       
## year2022_team_MIA                   -0.2068      -1.6610      *
## year2022_team_SEA                   -0.0535      -0.4017       
## year2022_team_TB                     0.0021       0.0161       
## year2022_team_TEN                    0.1739       1.4961      .
## year2022_team_WAS                   -0.0232      -0.1752       
## year2022_team_BAL                   -0.2318      -1.5433      .
## year2022_team_BUF                    0.0678       0.5123       
## year2022_team_DAL                   -0.0027      -0.0157       
## year2022_team_DET                   -0.1156      -0.9051       
## year2022_team_GB                    -0.1321      -0.9508       
## year2022_team_JAX                   -0.1973      -1.7079      *
## year2022_team_KC                    -0.1574      -0.9282       
## year2022_team_LA                     0.1378       1.0179       
## year2022_team_LV                     0.0971       0.6523       
## year2022_team_NO                    -0.0760      -0.4750       
## year2022_team_PHI                    0.0344       0.2612       
## year2022_team_PIT                    0.1280       0.9708       
## year2022_team_DEN                    0.0350       0.2877       
## year2022_team_MIN                   -0.1247      -0.8056       
## year2022_team_NE                     0.0437       0.3152       
## year2022_team_NYJ                   -0.1562      -1.1944       
## year2022_team_NYG                   -0.0656      -0.4552       
## year2022_team_SF                    -0.1894      -1.1437       
## year2023_team_BAL                   -0.0746      -0.5485       
## year2023_team_CHI                   -0.1636      -1.1555       
## year2023_team_CLE                   -0.1440      -0.9694       
## year2023_team_GB                    -0.0243      -0.1852       
## year2023_team_IND                    0.0429       0.3205       
## year2023_team_KC                    -0.0226      -0.1593       
## year2023_team_LAC                    0.0492       0.3294       
## year2023_team_LV                    -0.0135      -0.1056       
## year2023_team_MIA                   -0.0223      -0.1567       
## year2023_team_MIN                    0.1573       1.2967       
## year2023_team_NO                    -0.1186      -0.8366       
## year2023_team_NYG                    0.0573       0.4106       
## year2023_team_SEA                   -0.3145      -2.5524     **
## year2023_team_SF                     0.0306       0.1991       
## year2023_team_WAS                    0.1438       1.1384       
## year2023_team_ATL                   -0.1411      -0.9509       
## year2023_team_BUF                   -0.1040      -0.6853       
## year2023_team_CAR                    0.0603       0.4680       
## year2023_team_DAL                    0.0777       0.5285       
## year2023_team_DEN                   -0.0444      -0.3440       
## year2023_team_HOU                   -0.0162      -0.1110       
## year2023_team_LA                    -0.0126      -0.0843       
## year2023_team_NE                    -0.0012      -0.0090       
## year2023_team_PHI                   -0.0813      -0.6143       
## year2023_team_PIT                   -0.0190      -0.1174       
## year2023_team_TEN                   -0.0389      -0.2529       
## year2023_team_ARI                   -0.2062      -1.4516      .
## year2023_team_CIN                   -0.1644      -1.0741       
## year2023_team_DET                    0.0070       0.0553       
## year2023_team_TB                     0.0845       0.6040       
## year2023_team_JAX                   -0.0976      -0.6365       
## year2023_team_NYJ                    0.1587       1.1460       
## is_first_half                       -0.0134      -0.7561       
## time_in_half                         0.0155       1.5839      .
## home_attendance                     -0.0276      -0.3738       
## GIMR                                 0.0521       2.1791     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1103503 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.71
## prev_singleback_rate                                   5.58
## cover1_rate                                            6.08
## cover3_rate                                            6.45
## starter_OL_grades_offense_12w                          6.66
## home_attendance                                       13.79
## 
## 
##  ================================================================================ 
## MODEL COMPARISON - Adjusted R-squared values
## ================================================================================ 
## 
## Player Model with GIMR: 0.1110219 
## Starter Model with GIMR: 0.1103503 
## 
## 
## ==================================================================================================== 
## ANALYZING DATASET 7/8: Defense Tackles
## ==================================================================================================== 
## 
## Reading data: processed_predict_ccafd_def_tackles.csv.csv.gz
## Reading data: processed_predict_ccfd_def_tackles.csv.csv.gz
## 
## Phase 1: Validation Phase
## 
## Running 2 test iterations with best parameters...
## 
## Test Results over 2 iterations:
## Mean AUC: 0.8846365 
## SD AUC: 0.003329271 
## 95% CI: 0.8781111 to 0.8911618 
## 
## 
##  ================================================================================ 
## MODEL: Player Model with GIMR 
## ================================================================================ 
## 
## 
## Player Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.4404       3.5309    ***
## ydstogo                             -0.1099     -12.4840    ***
## posteam_timeouts_remaining           0.0119       1.2964       
## defteam_timeouts_remaining           0.0092       1.0369       
## rush_attempt                         0.1505       7.6575    ***
## week                                 0.0055       0.5484       
## temp                                -0.0111      -1.0568       
## wind                                 0.0114       1.0711       
## vegas_wp                             0.0165       1.4466      .
## spread_line                         -0.0032      -0.2524       
## total_line                           0.0242       1.9071      *
## prep_days                            0.0069       0.8821       
## overall_win_pct                      0.0084       0.6317       
## team_win_pct                         0.0178       1.2397       
## prev_win_pct                        -0.0362      -2.8533    ***
## prev_shotgun_rate                    0.0154       0.7076       
## prev_singleback_rate                 0.0116       0.7095       
## prev_empty_rate                      0.0131       1.0906       
## prev_iform_rate                      0.0048       0.3088       
## prev_shotgun_success                 0.0042       0.3570       
## prev_singleback_success              0.0065       0.5436       
## prev_empty_success                   0.0040       0.3598       
## prev_iform_success                   0.0222       2.2287     **
## prev_stop_rate_run                   0.0016       0.1389       
## prev_stop_rate_pass                 -0.0382      -3.6502    ***
## shotgun_rate                         0.0142       1.0426       
## singleback_rate                      0.0052       0.4357       
## empty_rate                          -0.0015      -0.1357       
## iform_rate                          -0.0187      -1.7808      *
## shotgun_success                     -0.0182      -2.0421     **
## singleback_success                  -0.0079      -0.8570       
## empty_success                       -0.0076      -0.7921       
## iform_success                       -0.0153      -1.5990      .
## def_stop_rate_run                    0.0156       1.6799      *
## def_stop_rate_pass                  -0.0115      -1.2083       
## avg_pass_rushers                    -0.0101      -0.8963       
## avg_box_defenders                   -0.0045      -0.4226       
## cover0_rate                          0.0009       0.0739       
## cover1_rate                         -0.0071      -0.3834       
## cover2_rate                         -0.0011      -0.0786       
## cover3_rate                          0.0308       1.5616      .
## cover4_rate                          0.0139       0.9599       
## cover6_rate                         -0.0032      -0.2499       
## two_man_rate                         0.0137       1.4601      .
## prevent_rate                         0.0212       2.6134    ***
## roof_outdoors                       -0.0111      -0.4601       
## posteam_type_home                   -0.0210      -1.3431       
## QB_grades_pass_12w                   0.0100       1.1953       
## RB_grades_run_12w                    0.0037       0.4965       
## WR1_grades_offense_12w              -0.0189      -2.1731     **
## WR2_grades_offense_12w              -0.0028      -0.2753       
## WR3_grades_offense_12w               0.0213       2.1391     **
## TE1_grades_offense_12w               0.0121       1.4947      .
## DL1_grades_tackles_12w              -0.0087      -1.0503       
## DL2_grades_tackles_12w               0.0130       1.5783      .
## DL3_grades_tackles_12w               0.0010       0.1105       
## DL4_grades_tackles_12w              -0.0107      -1.1842       
## LB1_grades_tackles_12w               0.0131       1.1896       
## LB1_tackles_12w                     -0.0170      -1.4788      .
## LB2_grades_tackles_12w              -0.0243      -2.0829     **
## LB2_tackles_12w                      0.0126       1.0712       
## LB3_grades_tackles_12w              -0.0181      -1.2826       
## LB3_tackles_12w                      0.0123       0.9187       
## LB4_grades_tackles_12w               0.0049       0.3627       
## LB4_tackles_12w                     -0.0026      -0.1917       
## CB1_grades_tackles_12w               0.0028       0.3207       
## CB1_tackles_12w                      0.0118       1.3380       
## CB2_grades_tackles_12w               0.0023       0.2399       
## CB2_tackles_12w                     -0.0027      -0.2880       
## CB3_grades_tackles_12w               0.0100       0.9389       
## CB3_tackles_12w                     -0.0074      -0.6674       
## S1_grades_tackles_12w                0.0047       0.5189       
## S1_tackles_12w                      -0.0021      -0.2423       
## S2_grades_tackles_12w                0.0090       0.8212       
## S2_tackles_12w                      -0.0036      -0.3179       
## S3_grades_tackles_12w                0.0221       1.7359      *
## S3_tackles_12w                      -0.0200      -1.5160      .
## OL_grades_offense_12w               -0.0062      -0.7638       
## yardline_1_10                       -0.0602      -2.2708     **
## yardline_11_20                       0.0107       0.3661       
## yardline_21_30                       0.0042       0.1475       
## yardline_41_50                       0.0487       2.0023     **
## yardline_51_60                       0.0212       0.7293       
## yardline_61_70                       0.0459       1.3981       
## yardline_71_80                       0.0734       1.8224      *
## yardline_81_90                       0.1388       2.3288     **
## yardline_91_100                      0.1092       1.0316       
## year2017_team_ARI                    0.0504       0.2642       
## year2017_team_BUF                   -0.1195      -0.5951       
## year2017_team_CHI                   -0.0148      -0.0833       
## year2017_team_CLE                    0.1640       0.8160       
## year2017_team_DAL                   -0.1058      -0.5994       
## year2017_team_DET                   -0.0865      -0.4881       
## year2017_team_GB                     0.3668       2.1710     **
## year2017_team_HOU                    0.3856       1.7517      *
## year2017_team_MIA                   -0.1854      -1.0133       
## year2017_team_MIN                   -0.0709      -0.3803       
## year2017_team_NE                     0.0173       0.0906       
## year2017_team_SF                     0.4128       2.0632     **
## year2017_team_BAL                    0.0434       0.2265       
## year2017_team_DEN                    0.0227       0.1226       
## year2017_team_LA                     0.0763       0.4004       
## year2017_team_NYG                   -0.0431      -0.2456       
## year2017_team_OAK                   -0.0872      -0.4717       
## year2017_team_SEA                    0.1196       0.6311       
## year2017_team_CAR                    0.1039       0.4683       
## year2017_team_CIN                    0.1682       0.8178       
## year2017_team_IND                    0.1610       0.8791       
## year2017_team_NO                     0.1272       0.5783       
## year2017_team_PHI                    0.0742       0.3960       
## year2017_team_PIT                   -0.1156      -0.6552       
## year2017_team_TEN                    0.0945       0.4384       
## year2017_team_WAS                    0.0335       0.1702       
## year2017_team_KC                     0.2924       1.4996      .
## year2017_team_LAC                   -0.0017      -0.0087       
## year2017_team_NYJ                    0.1784       0.8222       
## year2017_team_TB                     0.0788       0.3267       
## year2017_team_ATL                    0.0069       0.0346       
## year2017_team_JAX                    0.0905       0.4360       
## year2018_team_ARI                    0.0960       0.6528       
## year2018_team_BAL                    0.0876       0.6098       
## year2018_team_CAR                    0.0202       0.1388       
## year2018_team_CLE                   -0.0466      -0.3362       
## year2018_team_DET                    0.0985       0.6878       
## year2018_team_HOU                    0.1809       1.1375       
## year2018_team_IND                   -0.1447      -1.0632       
## year2018_team_KC                     0.1143       0.8344       
## year2018_team_NYG                    0.1133       0.6527       
## year2018_team_OAK                   -0.1302      -0.7733       
## year2018_team_PHI                    0.0632       0.4357       
## year2018_team_SEA                   -0.1037      -0.5866       
## year2018_team_BUF                   -0.1265      -0.7923       
## year2018_team_CHI                   -0.0110      -0.0860       
## year2018_team_CIN                   -0.0603      -0.3702       
## year2018_team_DAL                   -0.0631      -0.4255       
## year2018_team_DEN                   -0.0217      -0.1485       
## year2018_team_GB                    -0.0516      -0.3013       
## year2018_team_LAC                    0.0484       0.3322       
## year2018_team_NE                    -0.0954      -0.6346       
## year2018_team_NO                     0.1000       0.7245       
## year2018_team_PIT                    0.0815       0.4418       
## year2018_team_SF                     0.0451       0.3000       
## year2018_team_MIA                    0.0847       0.5898       
## year2018_team_MIN                    0.0533       0.3463       
## year2018_team_NYJ                    0.1376       0.5999       
## year2018_team_TB                     0.0588       0.3619       
## year2018_team_ATL                    0.0846       0.6278       
## year2018_team_JAX                    0.0470       0.3091       
## year2018_team_LA                    -0.1418      -0.9091       
## year2018_team_TEN                    0.1258       0.7847       
## year2018_team_WAS                   -0.0317      -0.1629       
## year2019_team_ARI                   -0.0910      -0.5913       
## year2019_team_BUF                   -0.1214      -0.9499       
## year2019_team_CHI                    0.0687       0.4695       
## year2019_team_CLE                    0.0747       0.4995       
## year2019_team_DAL                   -0.0667      -0.4057       
## year2019_team_IND                   -0.0739      -0.5534       
## year2019_team_JAX                    0.0673       0.4488       
## year2019_team_KC                     0.0093       0.0701       
## year2019_team_LAC                   -0.0918      -0.6602       
## year2019_team_MIN                   -0.0561      -0.3948       
## year2019_team_NE                    -0.0218      -0.1302       
## year2019_team_NO                    -0.1816      -1.2037       
## year2019_team_PHI                    0.0532       0.3628       
## year2019_team_SEA                    0.0270       0.1397       
## year2019_team_SF                    -0.0589      -0.4394       
## year2019_team_TB                    -0.1249      -0.9096       
## year2019_team_BAL                    0.0164       0.1177       
## year2019_team_CAR                   -0.0802      -0.4987       
## year2019_team_DEN                    0.1397       0.9842       
## year2019_team_DET                   -0.0948      -0.6241       
## year2019_team_HOU                   -0.0178      -0.1225       
## year2019_team_LA                    -0.1053      -0.6709       
## year2019_team_MIA                   -0.3102      -1.9615     **
## year2019_team_NYG                   -0.1542      -0.9718       
## year2019_team_NYJ                   -0.2491      -1.8588      *
## year2019_team_OAK                   -0.0707      -0.4641       
## year2019_team_PIT                   -0.3237      -2.6969    ***
## year2019_team_TEN                   -0.1467      -1.0457       
## year2019_team_CIN                    0.0741       0.5184       
## year2019_team_WAS                   -0.0683      -0.4551       
## year2019_team_ATL                    0.0012       0.0076       
## year2019_team_GB                    -0.0583      -0.3936       
## year2020_team_ATL                    0.0297       0.1927       
## year2020_team_BAL                    0.0508       0.3315       
## year2020_team_BUF                   -0.0160      -0.0875       
## year2020_team_CAR                    0.1055       0.6501       
## year2020_team_CIN                    0.1062       0.7232       
## year2020_team_DEN                   -0.0802      -0.4829       
## year2020_team_DET                   -0.1513      -0.9754       
## year2020_team_JAX                   -0.1129      -0.7075       
## year2020_team_KC                     0.0298       0.1870       
## year2020_team_LA                    -0.1893      -1.1162       
## year2020_team_MIN                    0.1478       1.0524       
## year2020_team_NE                    -0.0207      -0.1333       
## year2020_team_NO                     0.0250       0.1708       
## year2020_team_NYG                    0.0029       0.0189       
## year2020_team_SF                     0.0800       0.4918       
## year2020_team_WAS                    0.0290       0.1965       
## year2020_team_CHI                    0.0625       0.3924       
## year2020_team_DAL                   -0.0241      -0.1615       
## year2020_team_GB                    -0.0001      -0.0008       
## year2020_team_HOU                   -0.0808      -0.5086       
## year2020_team_MIA                   -0.1549      -0.9370       
## year2020_team_NYJ                   -0.0231      -0.1370       
## year2020_team_TB                     0.0488       0.3085       
## year2020_team_TEN                   -0.1022      -0.6269       
## year2020_team_ARI                    0.0744       0.4459       
## year2020_team_CLE                   -0.2486      -1.3986       
## year2020_team_IND                   -0.1728      -1.0345       
## year2020_team_LAC                    0.0331       0.1879       
## year2020_team_PHI                    0.0912       0.6207       
## year2020_team_SEA                   -0.0440      -0.2659       
## year2020_team_LV                     0.0961       0.6376       
## year2020_team_PIT                   -0.1294      -0.8024       
## year2021_team_ATL                   -0.2099      -1.6676      *
## year2021_team_BUF                    0.0420       0.3346       
## year2021_team_CIN                   -0.2392      -1.9719     **
## year2021_team_DAL                   -0.0936      -0.6696       
## year2021_team_DEN                    0.0677       0.5004       
## year2021_team_DET                   -0.0782      -0.5822       
## year2021_team_KC                     0.0163       0.1323       
## year2021_team_LA                    -0.0241      -0.1791       
## year2021_team_LV                     0.0571       0.3912       
## year2021_team_MIN                   -0.0139      -0.1068       
## year2021_team_NE                     0.0570       0.4196       
## year2021_team_NO                    -0.0183      -0.1367       
## year2021_team_NYG                    0.0141       0.1069       
## year2021_team_SF                    -0.0322      -0.2330       
## year2021_team_TEN                   -0.0618      -0.5054       
## year2021_team_ARI                    0.0644       0.5388       
## year2021_team_BAL                    0.1508       0.8464       
## year2021_team_CAR                   -0.0785      -0.6757       
## year2021_team_CHI                   -0.2368      -1.8688      *
## year2021_team_GB                     0.1063       0.8650       
## year2021_team_IND                   -0.0422      -0.3204       
## year2021_team_LAC                    0.0350       0.2411       
## year2021_team_MIA                    0.0190       0.1236       
## year2021_team_NYJ                   -0.0284      -0.1937       
## year2021_team_PHI                   -0.1890      -1.4883      .
## year2021_team_SEA                   -0.1975      -1.3344       
## year2021_team_TB                     0.0344       0.2411       
## year2021_team_WAS                   -0.0859      -0.6884       
## year2021_team_CLE                   -0.0996      -0.8146       
## year2021_team_HOU                   -0.0949      -0.6528       
## year2021_team_JAX                   -0.0528      -0.3631       
## year2021_team_PIT                    0.0515       0.3907       
## year2022_team_ARI                   -0.1670      -1.3123       
## year2022_team_ATL                   -0.2614      -1.9816     **
## year2022_team_CAR                    0.0954       0.6632       
## year2022_team_CHI                   -0.0808      -0.5045       
## year2022_team_CIN                   -0.1501      -0.9896       
## year2022_team_HOU                   -0.0580      -0.4176       
## year2022_team_IND                   -0.1014      -0.7472       
## year2022_team_LAC                   -0.0985      -0.7517       
## year2022_team_MIA                   -0.1726      -1.3877       
## year2022_team_SEA                   -0.0431      -0.3251       
## year2022_team_TB                     0.0253       0.1956       
## year2022_team_TEN                    0.1786       1.5482      .
## year2022_team_WAS                   -0.0219      -0.1692       
## year2022_team_BAL                   -0.1831      -1.2510       
## year2022_team_BUF                    0.0500       0.3920       
## year2022_team_DAL                    0.0060       0.0350       
## year2022_team_DET                   -0.0833      -0.6617       
## year2022_team_GB                    -0.1275      -0.9089       
## year2022_team_JAX                   -0.1426      -1.2571       
## year2022_team_KC                    -0.1316      -0.7864       
## year2022_team_LA                     0.1452       1.0925       
## year2022_team_LV                     0.1541       1.0415       
## year2022_team_NO                    -0.0538      -0.3619       
## year2022_team_PHI                    0.0559       0.4421       
## year2022_team_PIT                    0.1985       1.5662      .
## year2022_team_DEN                    0.0469       0.3847       
## year2022_team_MIN                   -0.1174      -0.7526       
## year2022_team_NE                     0.0610       0.4310       
## year2022_team_NYJ                   -0.1154      -0.8805       
## year2022_team_NYG                   -0.0913      -0.6362       
## year2022_team_SF                    -0.1882      -1.1184       
## year2023_team_BAL                   -0.0256      -0.1957       
## year2023_team_CHI                   -0.1537      -1.1100       
## year2023_team_CLE                   -0.1122      -0.7828       
## year2023_team_GB                     0.0086       0.0651       
## year2023_team_IND                    0.0958       0.7450       
## year2023_team_KC                     0.0325       0.2323       
## year2023_team_LAC                    0.0743       0.5234       
## year2023_team_LV                     0.0157       0.1226       
## year2023_team_MIA                    0.0581       0.4327       
## year2023_team_MIN                    0.1801       1.5223      .
## year2023_team_NO                    -0.0539      -0.3816       
## year2023_team_NYG                    0.0646       0.4815       
## year2023_team_SEA                   -0.2666      -2.2099     **
## year2023_team_SF                     0.0488       0.3106       
## year2023_team_WAS                    0.1993       1.5981      .
## year2023_team_ATL                   -0.0903      -0.6254       
## year2023_team_BUF                   -0.0996      -0.6889       
## year2023_team_CAR                    0.0797       0.6393       
## year2023_team_DAL                    0.0834       0.5933       
## year2023_team_DEN                    0.0416       0.3231       
## year2023_team_HOU                   -0.0276      -0.1821       
## year2023_team_LA                     0.0277       0.1865       
## year2023_team_NE                     0.0510       0.3813       
## year2023_team_PHI                   -0.0263      -0.1986       
## year2023_team_PIT                    0.0073       0.0473       
## year2023_team_TEN                    0.0187       0.1258       
## year2023_team_ARI                   -0.1928      -1.3737       
## year2023_team_CIN                   -0.1602      -1.0415       
## year2023_team_DET                    0.0310       0.2529       
## year2023_team_TB                     0.1049       0.7826       
## year2023_team_JAX                   -0.0474      -0.3074       
## year2023_team_NYJ                    0.1906       1.3956       
## is_first_half                       -0.0114      -0.6305       
## time_in_half                         0.0153       1.5378      .
## home_attendance                     -0.0357      -0.4811       
## GIMR                                 0.0501       2.1457     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1096368 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.23
## prev_singleback_rate                                   5.33
## cover1_rate                                            6.46
## cover3_rate                                            7.43
## home_attendance                                       13.72
## 
## 
##  ================================================================================ 
## MODEL: Starter Model with GIMR 
## ================================================================================ 
## 
## 
## Starter Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.3669       2.9122    ***
## ydstogo                             -0.1097     -12.6472    ***
## posteam_timeouts_remaining           0.0100       1.0856       
## defteam_timeouts_remaining           0.0090       1.0165       
## rush_attempt                         0.1421       7.4906    ***
## week                                 0.0029       0.2869       
## temp                                -0.0082      -0.7729       
## wind                                 0.0076       0.7059       
## vegas_wp                             0.0098       0.8831       
## spread_line                         -0.0106      -0.8551       
## total_line                           0.0320       2.5052     **
## prep_days                            0.0070       0.8896       
## overall_win_pct                      0.0097       0.7367       
## team_win_pct                         0.0213       1.4514      .
## prev_win_pct                        -0.0317      -2.4632     **
## prev_shotgun_rate                    0.0135       0.6164       
## prev_singleback_rate                 0.0092       0.5605       
## prev_empty_rate                      0.0139       1.1425       
## prev_iform_rate                      0.0024       0.1543       
## prev_shotgun_success                 0.0004       0.0306       
## prev_singleback_success              0.0119       0.9923       
## prev_empty_success                   0.0046       0.4170       
## prev_iform_success                   0.0269       2.6764    ***
## prev_stop_rate_run                  -0.0020      -0.1755       
## prev_stop_rate_pass                 -0.0326      -3.2121    ***
## shotgun_rate                         0.0152       1.1043       
## singleback_rate                      0.0048       0.3990       
## empty_rate                          -0.0027      -0.2441       
## iform_rate                          -0.0165      -1.5721      .
## shotgun_success                     -0.0224      -2.4681     **
## singleback_success                  -0.0146      -1.5703      .
## empty_success                       -0.0062      -0.6363       
## iform_success                       -0.0159      -1.6421      .
## def_stop_rate_run                    0.0136       1.4529      .
## def_stop_rate_pass                  -0.0103      -1.0934       
## avg_pass_rushers                    -0.0122      -1.0950       
## avg_box_defenders                   -0.0021      -0.2009       
## cover0_rate                         -0.0042      -0.3686       
## cover1_rate                         -0.0090      -0.5050       
## cover2_rate                         -0.0064      -0.4876       
## cover3_rate                          0.0187       1.0111       
## cover4_rate                          0.0096       0.7115       
## cover6_rate                         -0.0072      -0.5960       
## two_man_rate                         0.0152       1.6333      .
## prevent_rate                         0.0212       2.6589    ***
## roof_outdoors                       -0.0025      -0.1038       
## posteam_type_home                   -0.0225      -1.4253       
## starter_QB_grades_pass_12w           0.0042       0.3015       
## starter_RB_grades_run_12w            0.0032       0.3414       
## starter_WR1_grades_offense_12w       0.0269       2.2227     **
## starter_WR2_grades_offense_12w      -0.0040      -0.3383       
## starter_WR3_grades_offense_12w      -0.0094      -0.9776       
## starter_TE1_grades_offense_12w      -0.0083      -0.7811       
## starter_DL1_grades_tackles_12w       0.0012       0.1463       
## starter_DL2_grades_tackles_12w       0.0108       1.2857       
## starter_DL3_grades_tackles_12w      -0.0056      -0.6639       
## starter_DL4_grades_tackles_12w      -0.0038      -0.4398       
## starter_LB1_grades_tackles_12w       0.0293       2.6358    ***
## starter_LB1_tackles_12w             -0.0141      -1.2288       
## starter_LB2_grades_tackles_12w       0.0008       0.0756       
## starter_LB2_tackles_12w              0.0004       0.0349       
## starter_LB3_grades_tackles_12w       0.0214       1.8929      *
## starter_LB3_tackles_12w             -0.0125      -1.0931       
## starter_LB4_grades_tackles_12w      -0.0197      -1.7180      *
## starter_LB4_tackles_12w              0.0165       1.4707      .
## starter_CB1_grades_tackles_12w      -0.0148      -1.7321      *
## starter_CB1_tackles_12w             -0.0151      -1.7287      *
## starter_CB2_grades_tackles_12w       0.0186       2.1783     **
## starter_CB2_tackles_12w             -0.0195      -2.1765     **
## starter_CB3_grades_tackles_12w      -0.0111      -1.2346       
## starter_CB3_tackles_12w             -0.0072      -0.7978       
## starter_S1_grades_tackles_12w        0.0117       1.2706       
## starter_S1_tackles_12w              -0.0070      -0.7789       
## starter_S2_grades_tackles_12w        0.0024       0.2552       
## starter_S2_tackles_12w               0.0000       0.0028       
## starter_S3_grades_tackles_12w        0.0103       1.0112       
## starter_S3_tackles_12w              -0.0123      -1.1872       
## starter_OL_grades_offense_12w        0.0107       0.6909       
## yardline_1_10                       -0.0582      -2.2452     **
## yardline_11_20                       0.0067       0.2304       
## yardline_21_30                       0.0015       0.0541       
## yardline_41_50                       0.0443       1.8366      *
## yardline_51_60                       0.0165       0.5687       
## yardline_61_70                       0.0451       1.3817       
## yardline_71_80                       0.0749       1.8476      *
## yardline_81_90                       0.1435       2.4342     **
## yardline_91_100                      0.1259       1.2540       
## year2017_team_ARI                    0.0835       0.4439       
## year2017_team_BUF                   -0.1060      -0.5448       
## year2017_team_CHI                    0.0159       0.0916       
## year2017_team_CLE                    0.2034       0.9962       
## year2017_team_DAL                   -0.1051      -0.6033       
## year2017_team_DET                   -0.0774      -0.4555       
## year2017_team_GB                     0.3297       1.9881     **
## year2017_team_HOU                    0.4307       2.0511     **
## year2017_team_MIA                   -0.1561      -0.8790       
## year2017_team_MIN                   -0.0948      -0.5224       
## year2017_team_NE                     0.0250       0.1349       
## year2017_team_SF                     0.3892       1.9592      *
## year2017_team_BAL                    0.0182       0.0944       
## year2017_team_DEN                    0.0043       0.0233       
## year2017_team_LA                     0.0638       0.3469       
## year2017_team_NYG                   -0.0145      -0.0827       
## year2017_team_OAK                    0.0300       0.1594       
## year2017_team_SEA                    0.1085       0.5718       
## year2017_team_CAR                    0.1201       0.5526       
## year2017_team_CIN                    0.1670       0.8137       
## year2017_team_IND                    0.1590       0.8883       
## year2017_team_NO                     0.1004       0.4600       
## year2017_team_PHI                    0.1140       0.6288       
## year2017_team_PIT                   -0.1753      -1.0402       
## year2017_team_TEN                    0.1559       0.7149       
## year2017_team_WAS                    0.0358       0.1872       
## year2017_team_KC                     0.2796       1.4353       
## year2017_team_LAC                    0.0157       0.0830       
## year2017_team_NYJ                    0.1934       0.9004       
## year2017_team_TB                     0.0979       0.4004       
## year2017_team_ATL                   -0.0555      -0.2892       
## year2017_team_JAX                    0.0897       0.4344       
## year2018_team_ARI                    0.1556       1.0560       
## year2018_team_BAL                    0.1332       0.9172       
## year2018_team_CAR                    0.1231       0.8350       
## year2018_team_CLE                   -0.0046      -0.0338       
## year2018_team_DET                    0.0709       0.4995       
## year2018_team_HOU                    0.2084       1.2436       
## year2018_team_IND                   -0.0548      -0.3977       
## year2018_team_KC                     0.0846       0.6238       
## year2018_team_NYG                    0.1482       0.8420       
## year2018_team_OAK                   -0.0030      -0.0173       
## year2018_team_PHI                    0.1510       1.0256       
## year2018_team_SEA                   -0.0494      -0.2993       
## year2018_team_BUF                    0.0148       0.0906       
## year2018_team_CHI                    0.0404       0.3038       
## year2018_team_CIN                   -0.0071      -0.0420       
## year2018_team_DAL                    0.0440       0.2990       
## year2018_team_DEN                    0.0929       0.6220       
## year2018_team_GB                     0.0241       0.1397       
## year2018_team_LAC                    0.0963       0.6743       
## year2018_team_NE                    -0.0611      -0.3860       
## year2018_team_NO                     0.1492       1.0696       
## year2018_team_PIT                    0.1133       0.5896       
## year2018_team_SF                     0.0525       0.3374       
## year2018_team_MIA                    0.0718       0.4938       
## year2018_team_MIN                    0.0649       0.4044       
## year2018_team_NYJ                    0.2080       0.9064       
## year2018_team_TB                     0.1399       0.8230       
## year2018_team_ATL                    0.1336       0.9251       
## year2018_team_JAX                    0.1656       1.0965       
## year2018_team_LA                    -0.1022      -0.6397       
## year2018_team_TEN                    0.2148       1.3013       
## year2018_team_WAS                    0.1244       0.6419       
## year2019_team_ARI                   -0.0272      -0.1754       
## year2019_team_BUF                   -0.1192      -0.9379       
## year2019_team_CHI                    0.1239       0.8324       
## year2019_team_CLE                    0.1117       0.7095       
## year2019_team_DAL                    0.0217       0.1279       
## year2019_team_IND                    0.0105       0.0773       
## year2019_team_JAX                    0.2190       1.3861       
## year2019_team_KC                     0.0389       0.2934       
## year2019_team_LAC                   -0.0400      -0.2794       
## year2019_team_MIN                   -0.0446      -0.3173       
## year2019_team_NE                    -0.0194      -0.1173       
## year2019_team_NO                    -0.1413      -0.9334       
## year2019_team_PHI                    0.0821       0.5554       
## year2019_team_SEA                    0.0735       0.3739       
## year2019_team_SF                    -0.0077      -0.0566       
## year2019_team_TB                    -0.0875      -0.6033       
## year2019_team_BAL                    0.0523       0.3703       
## year2019_team_CAR                    0.0088       0.0541       
## year2019_team_DEN                    0.1769       1.2422       
## year2019_team_DET                   -0.0304      -0.2016       
## year2019_team_HOU                    0.0202       0.1367       
## year2019_team_LA                    -0.0777      -0.4757       
## year2019_team_MIA                   -0.2774      -1.7583      *
## year2019_team_NYG                   -0.0986      -0.6208       
## year2019_team_NYJ                   -0.1316      -1.0050       
## year2019_team_OAK                    0.0688       0.4312       
## year2019_team_PIT                   -0.2465      -1.9808     **
## year2019_team_TEN                   -0.1253      -0.8798       
## year2019_team_CIN                    0.0929       0.6239       
## year2019_team_WAS                   -0.0245      -0.1638       
## year2019_team_ATL                    0.0660       0.4274       
## year2019_team_GB                    -0.0247      -0.1637       
## year2020_team_ATL                    0.1385       0.8816       
## year2020_team_BAL                    0.1516       0.9784       
## year2020_team_BUF                    0.0941       0.5145       
## year2020_team_CAR                    0.2062       1.2877       
## year2020_team_CIN                    0.1057       0.7160       
## year2020_team_DEN                   -0.0115      -0.0663       
## year2020_team_DET                   -0.0760      -0.4952       
## year2020_team_JAX                   -0.0242      -0.1527       
## year2020_team_KC                     0.0797       0.4878       
## year2020_team_LA                    -0.0878      -0.5148       
## year2020_team_MIN                    0.2083       1.4648      .
## year2020_team_NE                     0.0483       0.3067       
## year2020_team_NO                     0.1150       0.7787       
## year2020_team_NYG                    0.1409       0.9289       
## year2020_team_SF                     0.1385       0.8434       
## year2020_team_WAS                    0.1015       0.6758       
## year2020_team_CHI                    0.1054       0.6699       
## year2020_team_DAL                    0.0582       0.3863       
## year2020_team_GB                     0.0764       0.4295       
## year2020_team_HOU                   -0.0900      -0.5532       
## year2020_team_MIA                   -0.0598      -0.3621       
## year2020_team_NYJ                    0.1078       0.6304       
## year2020_team_TB                     0.1579       0.9663       
## year2020_team_TEN                   -0.0242      -0.1505       
## year2020_team_ARI                    0.1589       0.9427       
## year2020_team_CLE                   -0.1858      -1.0632       
## year2020_team_IND                   -0.0811      -0.4851       
## year2020_team_LAC                    0.1199       0.6742       
## year2020_team_PHI                    0.2072       1.4239       
## year2020_team_SEA                    0.0543       0.3213       
## year2020_team_LV                     0.1831       1.1917       
## year2020_team_PIT                   -0.0686      -0.4180       
## year2021_team_ATL                   -0.1583      -1.2249       
## year2021_team_BUF                    0.0687       0.5562       
## year2021_team_CIN                   -0.1605      -1.2555       
## year2021_team_DAL                   -0.0402      -0.2866       
## year2021_team_DEN                    0.1609       1.1742       
## year2021_team_DET                   -0.0254      -0.1843       
## year2021_team_KC                     0.0621       0.4960       
## year2021_team_LA                     0.0471       0.3463       
## year2021_team_LV                     0.1268       0.8991       
## year2021_team_MIN                   -0.0554      -0.4183       
## year2021_team_NE                     0.0793       0.5788       
## year2021_team_NO                     0.0611       0.4506       
## year2021_team_NYG                    0.0888       0.6631       
## year2021_team_SF                     0.0172       0.1198       
## year2021_team_TEN                    0.0262       0.2073       
## year2021_team_ARI                    0.1119       0.9129       
## year2021_team_BAL                    0.1966       1.1096       
## year2021_team_CAR                   -0.0524      -0.4362       
## year2021_team_CHI                   -0.1913      -1.4931      .
## year2021_team_GB                     0.1292       1.0276       
## year2021_team_IND                   -0.0084      -0.0611       
## year2021_team_LAC                    0.0531       0.3610       
## year2021_team_MIA                    0.0861       0.5603       
## year2021_team_NYJ                    0.0095       0.0648       
## year2021_team_PHI                   -0.1400      -1.0746       
## year2021_team_SEA                   -0.1392      -0.9171       
## year2021_team_TB                     0.0753       0.5312       
## year2021_team_WAS                   -0.0013      -0.0103       
## year2021_team_CLE                   -0.0426      -0.3346       
## year2021_team_HOU                   -0.0482      -0.3252       
## year2021_team_JAX                    0.0337       0.2287       
## year2021_team_PIT                    0.0585       0.4348       
## year2022_team_ARI                   -0.1043      -0.8031       
## year2022_team_ATL                   -0.2166      -1.6717      *
## year2022_team_CAR                    0.1571       1.0860       
## year2022_team_CHI                   -0.0397      -0.2498       
## year2022_team_CIN                   -0.0733      -0.4996       
## year2022_team_HOU                    0.0322       0.2278       
## year2022_team_IND                   -0.0599      -0.4394       
## year2022_team_LAC                   -0.0865      -0.6550       
## year2022_team_MIA                   -0.1396      -1.1226       
## year2022_team_SEA                    0.0008       0.0063       
## year2022_team_TB                     0.0427       0.3308       
## year2022_team_TEN                    0.2515       2.1303     **
## year2022_team_WAS                    0.0917       0.7101       
## year2022_team_BAL                   -0.1782      -1.2151       
## year2022_team_BUF                    0.0967       0.7221       
## year2022_team_DAL                    0.0528       0.3161       
## year2022_team_DET                   -0.0256      -0.1988       
## year2022_team_GB                    -0.0990      -0.7164       
## year2022_team_JAX                   -0.1031      -0.8961       
## year2022_team_KC                    -0.0568      -0.3460       
## year2022_team_LA                     0.2036       1.4910      .
## year2022_team_LV                     0.2118       1.4229       
## year2022_team_NO                    -0.0020      -0.0122       
## year2022_team_PHI                    0.0962       0.7507       
## year2022_team_PIT                    0.1837       1.4186       
## year2022_team_DEN                    0.1446       1.1889       
## year2022_team_MIN                   -0.0482      -0.3097       
## year2022_team_NE                     0.0967       0.6851       
## year2022_team_NYJ                   -0.0705      -0.5400       
## year2022_team_NYG                   -0.0071      -0.0491       
## year2022_team_SF                    -0.1672      -1.0487       
## year2023_team_BAL                    0.0168       0.1284       
## year2023_team_CHI                   -0.0939      -0.6963       
## year2023_team_CLE                   -0.1134      -0.7507       
## year2023_team_GB                     0.0337       0.2548       
## year2023_team_IND                    0.1729       1.2987       
## year2023_team_KC                     0.0458       0.3254       
## year2023_team_LAC                    0.1039       0.7302       
## year2023_team_LV                     0.0781       0.5781       
## year2023_team_MIA                    0.0373       0.2803       
## year2023_team_MIN                    0.2654       2.1931     **
## year2023_team_NO                    -0.0286      -0.1990       
## year2023_team_NYG                    0.0893       0.6506       
## year2023_team_SEA                   -0.2129      -1.7270      *
## year2023_team_SF                     0.1282       0.8498       
## year2023_team_WAS                    0.2342       1.8678      *
## year2023_team_ATL                   -0.0845      -0.5764       
## year2023_team_BUF                   -0.0328      -0.2163       
## year2023_team_CAR                    0.1744       1.3579       
## year2023_team_DAL                    0.1466       1.0337       
## year2023_team_DEN                    0.0488       0.3735       
## year2023_team_HOU                    0.0483       0.3298       
## year2023_team_LA                     0.0703       0.4622       
## year2023_team_NE                     0.1273       0.9489       
## year2023_team_PHI                   -0.0076      -0.0580       
## year2023_team_PIT                    0.0777       0.4853       
## year2023_team_TEN                    0.0567       0.3758       
## year2023_team_ARI                   -0.0420      -0.2840       
## year2023_team_CIN                   -0.0821      -0.5311       
## year2023_team_DET                    0.0643       0.5044       
## year2023_team_TB                     0.2071       1.4858      .
## year2023_team_JAX                   -0.0061      -0.0409       
## year2023_team_NYJ                    0.2289       1.6361      .
## is_first_half                       -0.0102      -0.5739       
## time_in_half                         0.0163       1.6588      *
## home_attendance                     -0.0031      -0.0420       
## GIMR                                 0.0465       2.0345     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1128029 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.61
## prev_singleback_rate                                   5.46
## cover1_rate                                            6.03
## cover3_rate                                            6.46
## home_attendance                                       13.70
## 
## 
##  ================================================================================ 
## MODEL COMPARISON - Adjusted R-squared values
## ================================================================================ 
## 
## Player Model with GIMR: 0.1096368 
## Starter Model with GIMR: 0.1128029 
## 
## 
## ==================================================================================================== 
## ANALYZING DATASET 8/8: Defense Pressure
## ==================================================================================================== 
## 
## Reading data: processed_predict_ccafd_def_pressure.csv.csv.gz
## Reading data: processed_predict_ccfd_def_pressure.csv.csv.gz
## 
## Phase 1: Validation Phase
## 
## Running 2 test iterations with best parameters...
## 
## Test Results over 2 iterations:
## Mean AUC: 0.8860601 
## SD AUC: 0.0009662226 
## 95% CI: 0.8841663 to 0.8879538 
## 
## 
##  ================================================================================ 
## MODEL: Player Model with GIMR 
## ================================================================================ 
## 
## 
## Player Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.4513       3.6378    ***
## ydstogo                             -0.1101     -12.6252    ***
## posteam_timeouts_remaining           0.0102       1.1185       
## defteam_timeouts_remaining           0.0084       0.9416       
## rush_attempt                         0.1508       7.6978    ***
## week                                 0.0057       0.5697       
## temp                                -0.0093      -0.8821       
## wind                                 0.0107       1.0076       
## vegas_wp                             0.0134       1.1932       
## spread_line                         -0.0021      -0.1714       
## total_line                           0.0252       1.9934     **
## prep_days                            0.0077       0.9926       
## overall_win_pct                      0.0067       0.5098       
## team_win_pct                         0.0167       1.1623       
## prev_win_pct                        -0.0358      -2.8312    ***
## prev_shotgun_rate                    0.0104       0.4777       
## prev_singleback_rate                 0.0086       0.5265       
## prev_empty_rate                      0.0112       0.9348       
## prev_iform_rate                      0.0033       0.2174       
## prev_shotgun_success                 0.0041       0.3450       
## prev_singleback_success              0.0086       0.7387       
## prev_empty_success                   0.0030       0.2767       
## prev_iform_success                   0.0240       2.3956     **
## prev_stop_rate_run                  -0.0021      -0.1844       
## prev_stop_rate_pass                 -0.0324      -3.1888    ***
## shotgun_rate                         0.0137       1.0061       
## singleback_rate                      0.0044       0.3671       
## empty_rate                          -0.0024      -0.2136       
## iform_rate                          -0.0192      -1.8248      *
## shotgun_success                     -0.0187      -2.0996     **
## singleback_success                  -0.0079      -0.8578       
## empty_success                       -0.0068      -0.7065       
## iform_success                       -0.0136      -1.4153       
## def_stop_rate_run                    0.0158       1.7030      *
## def_stop_rate_pass                  -0.0117      -1.2384       
## avg_pass_rushers                    -0.0090      -0.7984       
## avg_box_defenders                   -0.0069      -0.6497       
## cover0_rate                         -0.0015      -0.1265       
## cover1_rate                         -0.0094      -0.5188       
## cover2_rate                         -0.0038      -0.2866       
## cover3_rate                          0.0240       1.3033       
## cover4_rate                          0.0136       0.9999       
## cover6_rate                         -0.0097      -0.7871       
## two_man_rate                         0.0133       1.4113       
## prevent_rate                         0.0191       2.3882     **
## roof_outdoors                       -0.0151      -0.6263       
## posteam_type_home                   -0.0224      -1.4299       
## QB_grades_pass_12w                   0.0120       1.4336       
## RB_grades_run_12w                    0.0046       0.6059       
## WR1_grades_offense_12w              -0.0183      -2.1163     **
## WR2_grades_offense_12w              -0.0006      -0.0582       
## WR3_grades_offense_12w               0.0222       2.2469     **
## TE1_grades_offense_12w               0.0116       1.4377       
## DL1_hurries_12w                     -0.0162      -1.9297      *
## DL2_hurries_12w                     -0.0020      -0.2432       
## DL3_hurries_12w                     -0.0063      -0.7060       
## DL4_hurries_12w                     -0.0014      -0.1609       
## LB1_hurries_12w                     -0.0116      -1.3257       
## LB2_hurries_12w                     -0.0048      -0.5515       
## LB3_hurries_12w                      0.0047       0.5343       
## LB4_hurries_12w                      0.0053       0.6383       
## CB1_targets_12w                      0.0108       1.2637       
## CB2_targets_12w                     -0.0020      -0.2327       
## CB3_targets_12w                      0.0016       0.1744       
## S1_targets_12w                      -0.0011      -0.1316       
## S2_targets_12w                       0.0044       0.5238       
## S3_targets_12w                      -0.0016      -0.1876       
## OL_grades_offense_12w               -0.0062      -0.7662       
## yardline_1_10                       -0.0614      -2.3192     **
## yardline_11_20                       0.0099       0.3401       
## yardline_21_30                       0.0038       0.1344       
## yardline_41_50                       0.0488       2.0153     **
## yardline_51_60                       0.0171       0.5891       
## yardline_61_70                       0.0428       1.3151       
## yardline_71_80                       0.0681       1.6940      *
## yardline_81_90                       0.1292       2.1466     **
## yardline_91_100                      0.1194       1.1500       
## year2017_team_ARI                    0.0390       0.2085       
## year2017_team_BUF                   -0.1441      -0.7445       
## year2017_team_CHI                   -0.0372      -0.2157       
## year2017_team_CLE                    0.1202       0.6095       
## year2017_team_DAL                   -0.1497      -0.8760       
## year2017_team_DET                   -0.0880      -0.5156       
## year2017_team_GB                     0.3164       1.9328      *
## year2017_team_HOU                    0.3538       1.6476      *
## year2017_team_MIA                   -0.2152      -1.2172       
## year2017_team_MIN                   -0.1139      -0.6393       
## year2017_team_NE                    -0.0180      -0.0968       
## year2017_team_SF                     0.3728       1.8734      *
## year2017_team_BAL                   -0.0026      -0.0137       
## year2017_team_DEN                    0.0066       0.0365       
## year2017_team_LA                     0.0428       0.2296       
## year2017_team_NYG                   -0.0671      -0.3925       
## year2017_team_OAK                   -0.1042      -0.5882       
## year2017_team_SEA                    0.0989       0.5342       
## year2017_team_CAR                    0.0768       0.3588       
## year2017_team_CIN                    0.1473       0.7252       
## year2017_team_IND                    0.1379       0.7749       
## year2017_team_NO                     0.0863       0.4041       
## year2017_team_PHI                    0.0330       0.1842       
## year2017_team_PIT                   -0.1715      -1.0069       
## year2017_team_TEN                    0.0738       0.3405       
## year2017_team_WAS                    0.0155       0.0797       
## year2017_team_KC                     0.2805       1.4559      .
## year2017_team_LAC                   -0.0031      -0.0169       
## year2017_team_NYJ                    0.1602       0.7476       
## year2017_team_TB                     0.0486       0.2043       
## year2017_team_ATL                   -0.0320      -0.1669       
## year2017_team_JAX                    0.0790       0.3902       
## year2018_team_ARI                    0.0872       0.5909       
## year2018_team_BAL                    0.0797       0.5532       
## year2018_team_CAR                    0.0245       0.1688       
## year2018_team_CLE                   -0.0492      -0.3511       
## year2018_team_DET                    0.0833       0.5800       
## year2018_team_HOU                    0.2106       1.2769       
## year2018_team_IND                   -0.1119      -0.8202       
## year2018_team_KC                     0.1272       0.9210       
## year2018_team_NYG                    0.0994       0.5766       
## year2018_team_OAK                   -0.1064      -0.6376       
## year2018_team_PHI                    0.0884       0.6096       
## year2018_team_SEA                   -0.0915      -0.5230       
## year2018_team_BUF                   -0.0856      -0.5346       
## year2018_team_CHI                   -0.0004      -0.0034       
## year2018_team_CIN                   -0.0603      -0.3563       
## year2018_team_DAL                   -0.0373      -0.2566       
## year2018_team_DEN                    0.0117       0.0802       
## year2018_team_GB                    -0.0161      -0.0975       
## year2018_team_LAC                    0.0654       0.4355       
## year2018_team_NE                    -0.0833      -0.5399       
## year2018_team_NO                     0.1133       0.8295       
## year2018_team_PIT                    0.0767       0.4099       
## year2018_team_SF                     0.0305       0.2082       
## year2018_team_MIA                    0.0885       0.6184       
## year2018_team_MIN                    0.0551       0.3500       
## year2018_team_NYJ                    0.1685       0.7323       
## year2018_team_TB                     0.0433       0.2659       
## year2018_team_ATL                    0.0764       0.5590       
## year2018_team_JAX                    0.0540       0.3587       
## year2018_team_LA                    -0.1238      -0.7901       
## year2018_team_TEN                    0.1351       0.8202       
## year2018_team_WAS                   -0.0015      -0.0075       
## year2019_team_ARI                   -0.1019      -0.6760       
## year2019_team_BUF                   -0.1313      -1.0496       
## year2019_team_CHI                    0.0770       0.5394       
## year2019_team_CLE                    0.0968       0.6573       
## year2019_team_DAL                   -0.0409      -0.2463       
## year2019_team_IND                   -0.0697      -0.5270       
## year2019_team_JAX                    0.0661       0.4399       
## year2019_team_KC                     0.0160       0.1219       
## year2019_team_LAC                   -0.0883      -0.6301       
## year2019_team_MIN                   -0.0645      -0.4605       
## year2019_team_NE                    -0.0384      -0.2340       
## year2019_team_NO                    -0.1523      -1.0099       
## year2019_team_PHI                    0.0774       0.5290       
## year2019_team_SEA                    0.0219       0.1112       
## year2019_team_SF                    -0.0374      -0.2792       
## year2019_team_TB                    -0.1614      -1.1736       
## year2019_team_BAL                    0.0133       0.0959       
## year2019_team_CAR                   -0.0778      -0.4795       
## year2019_team_DEN                    0.1527       1.0809       
## year2019_team_DET                   -0.0867      -0.5767       
## year2019_team_HOU                   -0.0185      -0.1276       
## year2019_team_LA                    -0.0999      -0.6246       
## year2019_team_MIA                   -0.3286      -2.0767     **
## year2019_team_NYG                   -0.1555      -0.9895       
## year2019_team_NYJ                   -0.2171      -1.6611      *
## year2019_team_OAK                   -0.0671      -0.4458       
## year2019_team_PIT                   -0.3229      -2.7339    ***
## year2019_team_TEN                   -0.1750      -1.2663       
## year2019_team_CIN                    0.0664       0.4728       
## year2019_team_WAS                   -0.0527      -0.3508       
## year2019_team_ATL                   -0.0119      -0.0768       
## year2019_team_GB                    -0.0322      -0.2177       
## year2020_team_ATL                    0.0345       0.2265       
## year2020_team_BAL                    0.0389       0.2556       
## year2020_team_BUF                    0.0020       0.0111       
## year2020_team_CAR                    0.1232       0.7547       
## year2020_team_CIN                    0.1086       0.7319       
## year2020_team_DEN                   -0.0920      -0.5533       
## year2020_team_DET                   -0.1427      -0.9289       
## year2020_team_JAX                   -0.1273      -0.7997       
## year2020_team_KC                     0.0491       0.3057       
## year2020_team_LA                    -0.2009      -1.1817       
## year2020_team_MIN                    0.1501       1.0776       
## year2020_team_NE                    -0.0347      -0.2220       
## year2020_team_NO                     0.0459       0.3150       
## year2020_team_NYG                   -0.0014      -0.0094       
## year2020_team_SF                     0.0644       0.3927       
## year2020_team_WAS                    0.0242       0.1624       
## year2020_team_CHI                    0.0469       0.2968       
## year2020_team_DAL                   -0.0384      -0.2594       
## year2020_team_GB                     0.0280       0.1618       
## year2020_team_HOU                   -0.0985      -0.6242       
## year2020_team_MIA                   -0.1432      -0.8785       
## year2020_team_NYJ                    0.0001       0.0004       
## year2020_team_TB                     0.0570       0.3634       
## year2020_team_TEN                   -0.1040      -0.6359       
## year2020_team_ARI                    0.0689       0.4148       
## year2020_team_CLE                   -0.2485      -1.4058       
## year2020_team_IND                   -0.1792      -1.0722       
## year2020_team_LAC                    0.0322       0.1849       
## year2020_team_PHI                    0.0875       0.6071       
## year2020_team_SEA                   -0.0554      -0.3389       
## year2020_team_LV                     0.0894       0.5964       
## year2020_team_PIT                   -0.1169      -0.7153       
## year2021_team_ATL                   -0.2242      -1.7914      *
## year2021_team_BUF                    0.0365       0.2952       
## year2021_team_CIN                   -0.2426      -1.9983     **
## year2021_team_DAL                   -0.0853      -0.6120       
## year2021_team_DEN                    0.0654       0.4814       
## year2021_team_DET                   -0.0832      -0.6194       
## year2021_team_KC                     0.0271       0.2206       
## year2021_team_LA                     0.0120       0.0900       
## year2021_team_LV                     0.0521       0.3579       
## year2021_team_MIN                   -0.0345      -0.2668       
## year2021_team_NE                     0.0498       0.3623       
## year2021_team_NO                     0.0106       0.0788       
## year2021_team_NYG                   -0.0068      -0.0517       
## year2021_team_SF                    -0.0170      -0.1232       
## year2021_team_TEN                   -0.0510      -0.4147       
## year2021_team_ARI                    0.0607       0.5086       
## year2021_team_BAL                    0.1203       0.6807       
## year2021_team_CAR                   -0.0905      -0.7751       
## year2021_team_CHI                   -0.2280      -1.8128      *
## year2021_team_GB                     0.0943       0.7692       
## year2021_team_IND                   -0.0422      -0.3197       
## year2021_team_LAC                    0.0499       0.3418       
## year2021_team_MIA                    0.0201       0.1328       
## year2021_team_NYJ                   -0.0451      -0.3178       
## year2021_team_PHI                   -0.1901      -1.4910      .
## year2021_team_SEA                   -0.1950      -1.3157       
## year2021_team_TB                     0.0549       0.3934       
## year2021_team_WAS                   -0.0855      -0.6945       
## year2021_team_CLE                   -0.0908      -0.7322       
## year2021_team_HOU                   -0.1015      -0.7039       
## year2021_team_JAX                   -0.0389      -0.2693       
## year2021_team_PIT                    0.0361       0.2769       
## year2022_team_ARI                   -0.1555      -1.1983       
## year2022_team_ATL                   -0.2647      -2.0439     **
## year2022_team_CAR                    0.1032       0.6868       
## year2022_team_CHI                   -0.0971      -0.6096       
## year2022_team_CIN                   -0.1215      -0.8153       
## year2022_team_HOU                   -0.0306      -0.2223       
## year2022_team_IND                   -0.1114      -0.8301       
## year2022_team_LAC                   -0.0878      -0.6700       
## year2022_team_MIA                   -0.1645      -1.3506       
## year2022_team_SEA                   -0.0389      -0.2987       
## year2022_team_TB                     0.0114       0.0892       
## year2022_team_TEN                    0.1665       1.4462      .
## year2022_team_WAS                    0.0086       0.0661       
## year2022_team_BAL                   -0.2137      -1.4917      .
## year2022_team_BUF                    0.0489       0.3796       
## year2022_team_DAL                    0.0294       0.1693       
## year2022_team_DET                   -0.0987      -0.7875       
## year2022_team_GB                    -0.1266      -0.9260       
## year2022_team_JAX                   -0.1601      -1.4217       
## year2022_team_KC                    -0.1357      -0.8196       
## year2022_team_LA                     0.1609       1.2090       
## year2022_team_LV                     0.1697       1.1461       
## year2022_team_NO                    -0.0498      -0.3242       
## year2022_team_PHI                    0.0820       0.6438       
## year2022_team_PIT                    0.1691       1.3537       
## year2022_team_DEN                    0.0404       0.3412       
## year2022_team_MIN                   -0.1357      -0.8697       
## year2022_team_NE                     0.0371       0.2629       
## year2022_team_NYJ                   -0.1415      -1.1105       
## year2022_team_NYG                   -0.0642      -0.4451       
## year2022_team_SF                    -0.1732      -1.0219       
## year2023_team_BAL                   -0.0587      -0.4431       
## year2023_team_CHI                   -0.1595      -1.1634       
## year2023_team_CLE                   -0.1311      -0.9086       
## year2023_team_GB                     0.0141       0.1086       
## year2023_team_IND                    0.0823       0.6353       
## year2023_team_KC                     0.0231       0.1660       
## year2023_team_LAC                    0.0824       0.5782       
## year2023_team_LV                     0.0267       0.2073       
## year2023_team_MIA                    0.0450       0.3409       
## year2023_team_MIN                    0.1628       1.3874       
## year2023_team_NO                    -0.0507      -0.3571       
## year2023_team_NYG                    0.0695       0.5203       
## year2023_team_SEA                   -0.2645      -2.2203     **
## year2023_team_SF                     0.0490       0.3168       
## year2023_team_WAS                    0.1953       1.5917      .
## year2023_team_ATL                   -0.1020      -0.7068       
## year2023_team_BUF                   -0.0886      -0.6036       
## year2023_team_CAR                    0.0817       0.6586       
## year2023_team_DAL                    0.1189       0.8149       
## year2023_team_DEN                    0.0061       0.0473       
## year2023_team_HOU                   -0.0079      -0.0528       
## year2023_team_LA                     0.0369       0.2533       
## year2023_team_NE                     0.0328       0.2439       
## year2023_team_PHI                   -0.0207      -0.1568       
## year2023_team_PIT                   -0.0053      -0.0338       
## year2023_team_TEN                    0.0021       0.0144       
## year2023_team_ARI                   -0.1919      -1.3740       
## year2023_team_CIN                   -0.1578      -1.0423       
## year2023_team_DET                    0.0325       0.2652       
## year2023_team_TB                     0.0982       0.7250       
## year2023_team_JAX                   -0.0789      -0.5221       
## year2023_team_NYJ                    0.2000       1.4713      .
## is_first_half                       -0.0114      -0.6333       
## time_in_half                         0.0158       1.6042      .
## home_attendance                     -0.0326      -0.4401       
## GIMR                                 0.0478       1.9574      *
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.109698 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.23
## prev_singleback_rate                                   5.32
## cover1_rate                                            6.12
## cover3_rate                                            6.47
## home_attendance                                       13.67
## 
## 
##  ================================================================================ 
## MODEL: Starter Model with GIMR 
## ================================================================================ 
## 
## 
## Starter Model with GIMR Model Results (Robust Statistics)
## Variable                        Coefficient      t-value    Sig
## ----------------------------------------------------------------- 
## (Intercept)                          0.3896       3.1473    ***
## ydstogo                             -0.1090     -12.6410    ***
## posteam_timeouts_remaining           0.0107       1.1719       
## defteam_timeouts_remaining           0.0095       1.0710       
## rush_attempt                         0.1418       7.4794    ***
## week                                 0.0022       0.2235       
## temp                                -0.0098      -0.9169       
## wind                                 0.0103       0.9720       
## vegas_wp                             0.0110       0.9965       
## spread_line                         -0.0086      -0.6927       
## total_line                           0.0275       2.1596     **
## prep_days                            0.0063       0.8092       
## overall_win_pct                      0.0098       0.7455       
## team_win_pct                         0.0182       1.2693       
## prev_win_pct                        -0.0356      -2.7801    ***
## prev_shotgun_rate                    0.0212       0.9688       
## prev_singleback_rate                 0.0165       0.9939       
## prev_empty_rate                      0.0146       1.2008       
## prev_iform_rate                      0.0040       0.2580       
## prev_shotgun_success                 0.0040       0.3380       
## prev_singleback_success              0.0119       1.0053       
## prev_empty_success                   0.0017       0.1551       
## prev_iform_success                   0.0240       2.3967     **
## prev_stop_rate_run                  -0.0005      -0.0449       
## prev_stop_rate_pass                 -0.0347      -3.4119    ***
## shotgun_rate                         0.0127       0.9211       
## singleback_rate                      0.0036       0.3017       
## empty_rate                          -0.0036      -0.3282       
## iform_rate                          -0.0176      -1.6675      *
## shotgun_success                     -0.0211      -2.3441     **
## singleback_success                  -0.0141      -1.5218      .
## empty_success                       -0.0069      -0.7078       
## iform_success                       -0.0143      -1.4840      .
## def_stop_rate_run                    0.0152       1.6372      .
## def_stop_rate_pass                  -0.0144      -1.5209      .
## avg_pass_rushers                    -0.0097      -0.8729       
## avg_box_defenders                   -0.0027      -0.2545       
## cover0_rate                         -0.0023      -0.2064       
## cover1_rate                         -0.0069      -0.3868       
## cover2_rate                         -0.0007      -0.0516       
## cover3_rate                          0.0230       1.2573       
## cover4_rate                          0.0132       0.9884       
## cover6_rate                         -0.0015      -0.1222       
## two_man_rate                         0.0167       1.7758      *
## prevent_rate                         0.0208       2.5705     **
## roof_outdoors                       -0.0088      -0.3635       
## posteam_type_home                   -0.0249      -1.5867      .
## starter_QB_grades_pass_12w           0.0033       0.2369       
## starter_RB_grades_run_12w            0.0056       0.6048       
## starter_WR1_grades_offense_12w       0.0308       2.5980    ***
## starter_WR2_grades_offense_12w      -0.0029      -0.2434       
## starter_WR3_grades_offense_12w      -0.0095      -0.9850       
## starter_TE1_grades_offense_12w      -0.0037      -0.3451       
## starter_DL1_hurries_12w             -0.0060      -0.7086       
## starter_DL2_hurries_12w             -0.0097      -1.1201       
## starter_DL3_hurries_12w             -0.0032      -0.3747       
## starter_DL4_hurries_12w             -0.0127      -1.4066       
## starter_LB1_hurries_12w              0.0066       0.7679       
## starter_LB2_hurries_12w              0.0089       1.0569       
## starter_LB3_hurries_12w              0.0024       0.2961       
## starter_LB4_hurries_12w             -0.0086      -1.0091       
## starter_CB1_targets_12w             -0.0083      -0.9339       
## starter_CB2_targets_12w             -0.0091      -1.0312       
## starter_CB3_targets_12w             -0.0103      -1.2183       
## starter_S1_targets_12w              -0.0034      -0.3896       
## starter_S2_targets_12w              -0.0024      -0.2879       
## starter_S3_targets_12w              -0.0037      -0.4390       
## starter_OL_grades_offense_12w        0.0124       0.7974       
## yardline_1_10                       -0.0607      -2.3423     **
## yardline_11_20                       0.0045       0.1544       
## yardline_21_30                       0.0038       0.1351       
## yardline_41_50                       0.0471       1.9419      *
## yardline_51_60                       0.0165       0.5702       
## yardline_61_70                       0.0482       1.4811      .
## yardline_71_80                       0.0670       1.6631      *
## yardline_81_90                       0.1366       2.3354     **
## yardline_91_100                      0.1108       1.0629       
## year2017_team_ARI                    0.0855       0.4605       
## year2017_team_BUF                   -0.0796      -0.4163       
## year2017_team_CHI                    0.0389       0.2257       
## year2017_team_CLE                    0.2094       1.0393       
## year2017_team_DAL                   -0.1084      -0.6357       
## year2017_team_DET                   -0.0488      -0.2880       
## year2017_team_GB                     0.3476       2.1258     **
## year2017_team_HOU                    0.3916       1.8734      *
## year2017_team_MIA                   -0.1286      -0.7265       
## year2017_team_MIN                   -0.0723      -0.4060       
## year2017_team_NE                     0.0605       0.3259       
## year2017_team_SF                     0.4512       2.2617     **
## year2017_team_BAL                    0.0504       0.2641       
## year2017_team_DEN                    0.0319       0.1766       
## year2017_team_LA                     0.1011       0.5608       
## year2017_team_NYG                    0.0201       0.1158       
## year2017_team_OAK                    0.0457       0.2454       
## year2017_team_SEA                    0.1531       0.8167       
## year2017_team_CAR                    0.1345       0.6253       
## year2017_team_CIN                    0.1736       0.8576       
## year2017_team_IND                    0.1933       1.0874       
## year2017_team_NO                     0.1312       0.6039       
## year2017_team_PHI                    0.1147       0.6368       
## year2017_team_PIT                   -0.1144      -0.6636       
## year2017_team_TEN                    0.1075       0.4934       
## year2017_team_WAS                    0.0638       0.3358       
## year2017_team_KC                     0.3467       1.8171      *
## year2017_team_LAC                    0.0442       0.2343       
## year2017_team_NYJ                    0.2151       1.0221       
## year2017_team_TB                     0.1407       0.5702       
## year2017_team_ATL                   -0.0098      -0.0502       
## year2017_team_JAX                    0.1345       0.6761       
## year2018_team_ARI                    0.1216       0.8346       
## year2018_team_BAL                    0.1399       0.9722       
## year2018_team_CAR                    0.0988       0.6763       
## year2018_team_CLE                   -0.0284      -0.2052       
## year2018_team_DET                    0.0564       0.3921       
## year2018_team_HOU                    0.2101       1.3071       
## year2018_team_IND                   -0.0666      -0.4769       
## year2018_team_KC                     0.1126       0.8165       
## year2018_team_NYG                    0.1089       0.6163       
## year2018_team_OAK                   -0.0191      -0.1131       
## year2018_team_PHI                    0.1091       0.7573       
## year2018_team_SEA                   -0.0532      -0.3169       
## year2018_team_BUF                   -0.0380      -0.2375       
## year2018_team_CHI                    0.0175       0.1351       
## year2018_team_CIN                   -0.0400      -0.2435       
## year2018_team_DAL                    0.0172       0.1192       
## year2018_team_DEN                    0.0275       0.1850       
## year2018_team_GB                    -0.0053      -0.0319       
## year2018_team_LAC                    0.0982       0.6793       
## year2018_team_NE                    -0.0729      -0.4588       
## year2018_team_NO                     0.1630       1.1803       
## year2018_team_PIT                    0.1330       0.6912       
## year2018_team_SF                     0.0451       0.2924       
## year2018_team_MIA                    0.0839       0.5787       
## year2018_team_MIN                    0.0446       0.2855       
## year2018_team_NYJ                    0.2122       0.9596       
## year2018_team_TB                     0.0992       0.6018       
## year2018_team_ATL                    0.0702       0.4953       
## year2018_team_JAX                    0.1230       0.8245       
## year2018_team_LA                    -0.1340      -0.8504       
## year2018_team_TEN                    0.1573       0.9592       
## year2018_team_WAS                    0.0339       0.1788       
## year2019_team_ARI                   -0.0738      -0.4770       
## year2019_team_BUF                   -0.0998      -0.7903       
## year2019_team_CHI                    0.0998       0.6901       
## year2019_team_CLE                    0.1210       0.7945       
## year2019_team_DAL                   -0.0226      -0.1367       
## year2019_team_IND                   -0.0654      -0.4989       
## year2019_team_JAX                    0.1775       1.1304       
## year2019_team_KC                    -0.0002      -0.0013       
## year2019_team_LAC                   -0.0694      -0.4934       
## year2019_team_MIN                   -0.0927      -0.6553       
## year2019_team_NE                    -0.0052      -0.0312       
## year2019_team_NO                    -0.1782      -1.1737       
## year2019_team_PHI                    0.0899       0.6127       
## year2019_team_SEA                    0.0182       0.0961       
## year2019_team_SF                    -0.0204      -0.1526       
## year2019_team_TB                    -0.1315      -0.9436       
## year2019_team_BAL                    0.0357       0.2550       
## year2019_team_CAR                   -0.0626      -0.3836       
## year2019_team_DEN                    0.1240       0.8713       
## year2019_team_DET                   -0.0495      -0.3317       
## year2019_team_HOU                   -0.0071      -0.0486       
## year2019_team_LA                    -0.1056      -0.6465       
## year2019_team_MIA                   -0.3009      -1.9192      *
## year2019_team_NYG                   -0.1186      -0.7491       
## year2019_team_NYJ                   -0.1778      -1.3839       
## year2019_team_OAK                    0.0237       0.1491       
## year2019_team_PIT                   -0.3078      -2.4915     **
## year2019_team_TEN                   -0.1156      -0.8159       
## year2019_team_CIN                    0.1042       0.7188       
## year2019_team_WAS                   -0.0219      -0.1478       
## year2019_team_ATL                    0.0172       0.1116       
## year2019_team_GB                     0.0043       0.0287       
## year2020_team_ATL                    0.0984       0.6350       
## year2020_team_BAL                    0.1371       0.8975       
## year2020_team_BUF                    0.0600       0.3251       
## year2020_team_CAR                    0.1733       1.0875       
## year2020_team_CIN                    0.1597       1.0861       
## year2020_team_DEN                   -0.0133      -0.0777       
## year2020_team_DET                   -0.0855      -0.5608       
## year2020_team_JAX                   -0.0600      -0.3699       
## year2020_team_KC                     0.0600       0.3683       
## year2020_team_LA                    -0.1424      -0.8362       
## year2020_team_MIN                    0.2087       1.4862      .
## year2020_team_NE                     0.0072       0.0465       
## year2020_team_NO                     0.0755       0.5139       
## year2020_team_NYG                    0.0713       0.4689       
## year2020_team_SF                     0.1206       0.7295       
## year2020_team_WAS                    0.0916       0.6198       
## year2020_team_CHI                    0.0976       0.6263       
## year2020_team_DAL                    0.0394       0.2635       
## year2020_team_GB                     0.0606       0.3421       
## year2020_team_HOU                   -0.0728      -0.4493       
## year2020_team_MIA                   -0.0826      -0.5006       
## year2020_team_NYJ                    0.0628       0.3752       
## year2020_team_TB                     0.0864       0.5375       
## year2020_team_TEN                   -0.0509      -0.3153       
## year2020_team_ARI                    0.1264       0.7395       
## year2020_team_CLE                   -0.2003      -1.1450       
## year2020_team_IND                   -0.1146      -0.6937       
## year2020_team_LAC                    0.0774       0.4426       
## year2020_team_PHI                    0.2132       1.4713      .
## year2020_team_SEA                    0.0021       0.0131       
## year2020_team_LV                     0.1349       0.8935       
## year2020_team_PIT                   -0.0714      -0.4393       
## year2021_team_ATL                   -0.2156      -1.6992      *
## year2021_team_BUF                    0.0531       0.4277       
## year2021_team_CIN                   -0.2084      -1.6769      *
## year2021_team_DAL                   -0.0720      -0.5191       
## year2021_team_DEN                    0.0709       0.5270       
## year2021_team_DET                   -0.0870      -0.6427       
## year2021_team_KC                     0.0233       0.1873       
## year2021_team_LA                     0.0005       0.0036       
## year2021_team_LV                     0.1040       0.7196       
## year2021_team_MIN                   -0.0618      -0.4690       
## year2021_team_NE                     0.0589       0.4353       
## year2021_team_NO                     0.0214       0.1582       
## year2021_team_NYG                    0.0318       0.2416       
## year2021_team_SF                    -0.0096      -0.0690       
## year2021_team_TEN                    0.0049       0.0386       
## year2021_team_ARI                    0.0837       0.6918       
## year2021_team_BAL                    0.1528       0.8681       
## year2021_team_CAR                   -0.0814      -0.6884       
## year2021_team_CHI                   -0.2403      -1.8999      *
## year2021_team_GB                     0.0913       0.7334       
## year2021_team_IND                   -0.0238      -0.1801       
## year2021_team_LAC                    0.0314       0.2152       
## year2021_team_MIA                    0.0549       0.3600       
## year2021_team_NYJ                   -0.0139      -0.0966       
## year2021_team_PHI                   -0.1861      -1.4658      .
## year2021_team_SEA                   -0.1711      -1.1346       
## year2021_team_TB                     0.0332       0.2347       
## year2021_team_WAS                   -0.0396      -0.3142       
## year2021_team_CLE                   -0.0634      -0.5098       
## year2021_team_HOU                   -0.0636      -0.4385       
## year2021_team_JAX                    0.0112       0.0765       
## year2021_team_PIT                    0.0389       0.2883       
## year2022_team_ARI                   -0.1512      -1.1746       
## year2022_team_ATL                   -0.2656      -2.0857     **
## year2022_team_CAR                    0.1283       0.8653       
## year2022_team_CHI                   -0.0550      -0.3417       
## year2022_team_CIN                   -0.0843      -0.5633       
## year2022_team_HOU                    0.0124       0.0899       
## year2022_team_IND                   -0.0646      -0.4818       
## year2022_team_LAC                   -0.0800      -0.6049       
## year2022_team_MIA                   -0.1724      -1.3920       
## year2022_team_SEA                   -0.0012      -0.0093       
## year2022_team_TB                     0.0274       0.2125       
## year2022_team_TEN                    0.2164       1.8643      *
## year2022_team_WAS                    0.0367       0.2853       
## year2022_team_BAL                   -0.2124      -1.4553      .
## year2022_team_BUF                    0.0777       0.5961       
## year2022_team_DAL                    0.0460       0.2700       
## year2022_team_DET                   -0.0471      -0.3702       
## year2022_team_GB                    -0.1118      -0.8098       
## year2022_team_JAX                   -0.1396      -1.2329       
## year2022_team_KC                    -0.0998      -0.5915       
## year2022_team_LA                     0.1972       1.4873      .
## year2022_team_LV                     0.1797       1.2334       
## year2022_team_NO                    -0.0279      -0.1791       
## year2022_team_PHI                    0.0780       0.6192       
## year2022_team_PIT                    0.1964       1.5320      .
## year2022_team_DEN                    0.0829       0.7006       
## year2022_team_MIN                   -0.0975      -0.6253       
## year2022_team_NE                     0.0655       0.4648       
## year2022_team_NYJ                   -0.1033      -0.8146       
## year2022_team_NYG                   -0.0153      -0.1052       
## year2022_team_SF                    -0.1509      -0.9102       
## year2023_team_BAL                   -0.0155      -0.1175       
## year2023_team_CHI                   -0.1147      -0.8386       
## year2023_team_CLE                   -0.1074      -0.7172       
## year2023_team_GB                     0.0412       0.3156       
## year2023_team_IND                    0.1352       1.0513       
## year2023_team_KC                     0.0506       0.3646       
## year2023_team_LAC                    0.0650       0.4606       
## year2023_team_LV                     0.0623       0.4774       
## year2023_team_MIA                    0.0204       0.1532       
## year2023_team_MIN                    0.2086       1.7653      *
## year2023_team_NO                    -0.0320      -0.2215       
## year2023_team_NYG                    0.1127       0.8405       
## year2023_team_SEA                   -0.2365      -1.9641     **
## year2023_team_SF                     0.0568       0.3741       
## year2023_team_WAS                    0.2149       1.7456      *
## year2023_team_ATL                   -0.1100      -0.7684       
## year2023_team_BUF                   -0.0423      -0.2824       
## year2023_team_CAR                    0.1291       1.0297       
## year2023_team_DAL                    0.1188       0.8116       
## year2023_team_DEN                    0.0137       0.1083       
## year2023_team_HOU                    0.0182       0.1220       
## year2023_team_LA                     0.0537       0.3681       
## year2023_team_NE                     0.0833       0.6156       
## year2023_team_PHI                   -0.0261      -0.2007       
## year2023_team_PIT                    0.0243       0.1522       
## year2023_team_TEN                    0.0389       0.2628       
## year2023_team_ARI                   -0.1284      -0.8971       
## year2023_team_CIN                   -0.1011      -0.6601       
## year2023_team_DET                    0.0600       0.4764       
## year2023_team_TB                     0.1360       1.0014       
## year2023_team_JAX                   -0.0275      -0.1807       
## year2023_team_NYJ                    0.2204       1.5785      .
## is_first_half                       -0.0114      -0.6444       
## time_in_half                         0.0156       1.5849      .
## home_attendance                     -0.0009      -0.0125       
## GIMR                                 0.0500       2.0848     **
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Adjusted R-squared: 0.1092911 
## 
## Variables with VIF > 5:
## prev_shotgun_rate                                      9.39
## prev_singleback_rate                                   5.51
## cover1_rate                                            6.00
## cover3_rate                                            6.37
## home_attendance                                       13.68
## 
## 
##  ================================================================================ 
## MODEL COMPARISON - Adjusted R-squared values
## ================================================================================ 
## 
## Player Model with GIMR: 0.109698 
## Starter Model with GIMR: 0.1092911
```

```
## 
## 
##  ========================================================================================================================
```

```
## GIMR SELECTION BIAS RESULTS SUMMARY
```

```
## ========================================================================================================================
```

```
## Dataset                        Player GIMR               Starter GIMR
```

```
## --------------------------------------------------------------------------------
```

```
## Offense Grades                 0.0571 (t=2.19**)         0.0505 (t=1.95*)         
## Offense Yards                  0.0497 (t=1.96**)         0.0476 (t=1.91*)         
## Offense Tds                    0.0557 (t=2.31**)         0.0478 (t=2.01**)        
## Offense First Downs            0.0473 (t=2.00**)         0.0410 (t=1.76*)         
## Defense Stops                  0.0487 (t=1.92*)          0.0493 (t=1.98**)        
## Defense Grades                 0.0547 (t=2.17**)         0.0521 (t=2.09**)        
## Defense Tackles                0.0501 (t=2.07**)         0.0465 (t=1.96*)         
## Defense Pressure               0.0478 (t=1.89*)          0.0500 (t=2.01**)
```

```
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
```

```
## 
## Note: GIMR values are shown as coefficient (t-value). A significant GIMR coefficient indicates
```

```
## the presence of selection bias. All models control for multiple relevant variables as shown
```

```
## in the detailed model outputs above.
```

```
## 
## 
##  ========================================================================================================================
```

```
## QB PASS DEPTH T-VALUES IN OUTCOME MODELS
```

```
## ========================================================================================================================
```

```
## Dataset                        Model Type           QB Variable     Short      Medium     Deep      
## ----------------------------------------------------------------------------------------------- 
## Offense Grades                 Player Model         grades          2.453**    -0.301     -1.559.   
## Offense Grades                 Starter Model        grades          2.017**    -1.258     -0.857    
## Offense Yards                  Player Model         yards           1.530.     0.508      -1.693*   
## Offense Yards                  Starter Model        yards           1.649*     2.445**    -3.341*** 
## Offense Tds                    Player Model         touchdowns      0.417      0.071      -1.510.   
## Offense Tds                    Starter Model        touchdowns      3.051***   -1.313     -1.505.   
## Offense First Downs            Player Model         touchdowns      0.434      0.037      -1.520.   
## Offense First Downs            Starter Model        touchdowns      3.095***   -1.094     -1.494.   
## 
## Significance codes: 0 '***' 0.01 '**' 0.05 '*' 0.1 '.' 0.15
## 
## Note: T-values shown with significance stars. Higher absolute t-values indicate
## stronger statistical significance. Positive values suggest better conversion rates
## for passes at that depth, while negative values suggest worse conversion rates.
```

```
## 
## 
##  ======================================================================================================================== 
## SUMMARY: AVERAGE QB PASS DEPTH T-VALUES BY MODEL TYPE
## ======================================================================================================================== 
## 
## Model Type           Avg Short       Avg Medium      Avg Deep       
## ---------------------------------------------------------------------- 
## Player Model         1.208           0.079           -1.571         
## Starter Model        2.453           -0.305          -1.800         
## ---------------------------------------------------------------------- 
## Overall Average      1.831           -0.113          -1.685         
## 
## Note: Higher average t-values suggest stronger positive effects of quarterback
## performance at that pass depth on conversion success across models.
```

