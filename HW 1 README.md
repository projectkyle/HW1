# Econometrics
Assignments and stuff for Econometrics

#1.	Tanmay Thomas, Kim Fai Chan, Joaquin Sanchez Gomez, Nicholas Esposito, Collin Rafferty

#3. Results from Nicholas. Dice 1 and 2 are drilled so the face with 6 is lighter and theoretically will land facing up. Listed as 1-4 respectively.
1. 6,5,3,4
2. 2,1,5,4
3. 4,6,1,2
4. 2,3,1,2
5. 4,6,6,4
6. 6,1,6,4
7. 5,3,6,6
8. 5,5,1,1
9. 6,5,4,3
10. 6,6,5,1
11. 1,6,5,3
12. 4,1,2,6
13. 1,6,6,4
14. 1,1,4,1
15. 1,6,3,5
16. 5,2,3,5
17. 6,6,6,4
18. 3,2,2,1
19. 3,2,2,1
20. 1,3,3,5

#4.One interesting thing I've noticed from this dataset is that the number of people with an education level of 
nursury school to 4th grade is higher than the amount of people with a 2 year college degree.

summary(acs2017_ny)
      AGE            female         educ_nohs        educ_hs      
 Min.   : 0.00   Min.   :0.0000   Min.   :0.000   Min.   :0.0000  
 1st Qu.:22.00   1st Qu.:0.0000   1st Qu.:0.000   1st Qu.:0.0000  
 Median :42.00   Median :1.0000   Median :0.000   Median :0.0000  
 Mean   :41.57   Mean   :0.5156   Mean   :0.271   Mean   :0.2804  
 3rd Qu.:60.00   3rd Qu.:1.0000   3rd Qu.:1.000   3rd Qu.:1.0000  
 Max.   :95.00   Max.   :1.0000   Max.   :1.000   Max.   :1.0000  
                                                                  
 educ_somecoll    educ_college     educ_advdeg                  SCHOOL      
 Min.   :0.000   Min.   :0.0000   Min.   :0.000   N/A              :  5569  
 1st Qu.:0.000   1st Qu.:0.0000   1st Qu.:0.000   No, not in school:144968  
 Median :0.000   Median :0.0000   Median :0.000   Yes, in school   : 46048  
 Mean   :0.173   Mean   :0.1567   Mean   :0.119   Missing          :     0  
 3rd Qu.:0.000   3rd Qu.:0.0000   3rd Qu.:0.000                             
 Max.   :1.000   Max.   :1.0000   Max.   :1.000                             
                                                                            
                        EDUC      
 Grade 12                 :55119  
 4 years of college       :30802  
 5+ years of college      :23385  
 1 year of college        :19947  
 Nursery school to grade 4:14240  
 2 years of college       :14065  
 (Other)                  :39027  
                                          EDUCD      
 Regular high school diploma                 :35689  
 Bachelor's degree                           :30802  
 1 or more years of college credit, no degree:19947  
 Master's degree                             :17010  
 Associate's degree, type not specified      :14065  
 Some college, but less than 1 year          : 9086  
 (Other)                                     :69986  
                                     DEGFIELD     
 N/A                                     :142398  
 Business                                :  9802  
 Education Administration and Teaching   :  6708  
 Social Sciences                         :  4836  
 Medical and Health Sciences and Services:  3919  
 Fine Arts                               :  3491  
 (Other)                                 : 25431  
                                  DEGFIELDD     
 N/A                                   :142398  
 Psychology                            :  2926  
 Business Management and Administration:  2501  
 Accounting                            :  2284  
 General Education                     :  2238  
 English Language and Literature       :  2202  
 (Other)                               : 42036  
                                 DEGFIELD2     
 N/A                                  :190425  
 Business                             :   972  
 Social Sciences                      :   853  
 Education Administration and Teaching:   611  
 Fine Arts                            :   465  
 Communications                       :   352  
 (Other)                              :  2907  
                                                           DEGFIELD2D    
 N/A                                                            :190425  
 Psychology                                                     :   284  
 Economics                                                      :   260  
 Political Science and Government                               :   243  
 Business Management and Administration                         :   217  
 French, German, Latin and Other Common Foreign Language Studies:   205  
 (Other)                                                        :  4951  
      PUMA            GQ           OWNERSHP       OWNERSHPD        MORTGAGE    
 Min.   : 100   Min.   :1.000   Min.   :0.000   Min.   : 0.00   Min.   :0.000  
 1st Qu.:1500   1st Qu.:1.000   1st Qu.:1.000   1st Qu.:12.00   1st Qu.:0.000  
 Median :3201   Median :1.000   Median :1.000   Median :13.00   Median :1.000  
 Mean   :2713   Mean   :1.148   Mean   :1.266   Mean   :14.95   Mean   :1.453  
 3rd Qu.:3902   3rd Qu.:1.000   3rd Qu.:2.000   3rd Qu.:22.00   3rd Qu.:3.000  
 Max.   :4114   Max.   :5.000   Max.   :2.000   Max.   :22.00   Max.   :4.000  
                                                                               
    OWNCOST           RENT         COSTELEC       COSTGAS        COSTWATR   
 Min.   :    0   Min.   :   0   Min.   :   0   Min.   :   0   Min.   :   0  
 1st Qu.: 1208   1st Qu.:   0   1st Qu.: 960   1st Qu.: 840   1st Qu.: 320  
 Median : 2891   Median :   0   Median :1560   Median :2400   Median :1400  
 Mean   :38582   Mean   : 393   Mean   :2311   Mean   :5032   Mean   :4836  
 3rd Qu.:99999   3rd Qu.: 630   3rd Qu.:2520   3rd Qu.:9993   3rd Qu.:9993  
 Max.   :99999   Max.   :3800   Max.   :9997   Max.   :9997   Max.   :9997  
                                                                            
    COSTFUEL       HHINCOME          FOODSTMP        LINGISOL    
 Min.   :   0   Min.   : -11800   Min.   :1.000   Min.   :0.000  
 1st Qu.:9993   1st Qu.:  41600   1st Qu.:1.000   1st Qu.:1.000  
 Median :9993   Median :  81700   Median :1.000   Median :1.000  
 Mean   :7935   Mean   : 114902   Mean   :1.147   Mean   :1.002  
 3rd Qu.:9993   3rd Qu.: 140900   3rd Qu.:1.000   3rd Qu.:1.000  
 Max.   :9997   Max.   :2030000   Max.   :2.000   Max.   :2.000  
                NA's   :10630                                    
     ROOMS           BUILTYR2         UNITSSTR        FUELHEAT    
 Min.   : 0.000   Min.   : 0.000   Min.   : 0.00   Min.   :0.000  
 1st Qu.: 4.000   1st Qu.: 1.000   1st Qu.: 3.00   1st Qu.:2.000  
 Median : 6.000   Median : 3.000   Median : 3.00   Median :2.000  
 Mean   : 5.887   Mean   : 3.711   Mean   : 4.39   Mean   :2.959  
 3rd Qu.: 8.000   3rd Qu.: 5.000   3rd Qu.: 6.00   3rd Qu.:4.000  
 Max.   :16.000   Max.   :22.000   Max.   :10.00   Max.   :9.000  
                                                                  
      SSMC            FAMSIZE           NCHILD           NCHLT5       
 Min.   :0.00000   Min.   : 1.000   Min.   :0.0000   Min.   :0.00000  
 1st Qu.:0.00000   1st Qu.: 2.000   1st Qu.:0.0000   1st Qu.:0.00000  
 Median :0.00000   Median : 3.000   Median :0.0000   Median :0.00000  
 Mean   :0.01102   Mean   : 3.087   Mean   :0.5009   Mean   :0.08441  
 3rd Qu.:0.00000   3rd Qu.: 4.000   3rd Qu.:1.0000   3rd Qu.:0.00000  
 Max.   :2.00000   Max.   :19.000   Max.   :9.0000   Max.   :5.00000  
                                                                      
     RELATE          RELATED           MARST            RACE          RACED    
 Min.   : 1.000   Min.   : 101.0   Min.   :1.000   Min.   :1.00   Min.   :100  
 1st Qu.: 1.000   1st Qu.: 101.0   1st Qu.:1.000   1st Qu.:1.00   1st Qu.:100  
 Median : 2.000   Median : 201.0   Median :5.000   Median :1.00   Median :100  
 Mean   : 3.307   Mean   : 335.6   Mean   :3.742   Mean   :2.03   Mean   :205  
 3rd Qu.: 3.000   3rd Qu.: 301.0   3rd Qu.:6.000   3rd Qu.:2.00   3rd Qu.:200  
 Max.   :13.000   Max.   :1301.0   Max.   :6.000   Max.   :9.00   Max.   :990  
                                                                               
     HISPAN          HISPAND                  BPL        
 Min.   :0.0000   Min.   :  0.00   New York     :128517  
 1st Qu.:0.0000   1st Qu.:  0.00   West Indies  :  8481  
 Median :0.0000   Median :  0.00   China        :  4964  
 Mean   :0.4153   Mean   : 44.75   SOUTH AMERICA:  4957  
 3rd Qu.:0.0000   3rd Qu.:  0.00   India        :  3476  
 Max.   :4.0000   Max.   :498.00   Pennsylvania :  3303  
                                   (Other)      : 42887  
                 BPLD                            ANCESTR1    
 New York          :128517   Not Reported            :32021  
 China             :  4116   Italian                 :20577  
 Dominican Republic:  3517   Irish, various subheads,:16388  
 Pennsylvania      :  3303   German                  :12781  
 New Jersey        :  3127   African-American        : 9559  
 Puerto Rico       :  2272   United States           : 8209  
 (Other)           : 51733   (Other)                 :97050  
                                   ANCESTR1D             ANCESTR2     
 Not Reported                           :32021   Not Reported:141487  
 Italian (1990-2000, ACS, PRCS)         :20577   German      :  9476  
 Irish                                  :15651   Irish       :  9238  
 German (1990-2000, ACS/PRCS)           :12605   English     :  4895  
 African-American (1990-2000, ACS, PRCS): 9559   Italian     :  4531  
 United States                          : 8209   Polish      :  3113  
 (Other)                                :97963   (Other)     : 23845  
                          ANCESTR2D         CITIZEN          YRSUSA1      
 Not Reported                  :141487   Min.   :0.0000   Min.   : 0.000  
 German (1990-2000, ACS, PRCS) :  9441   1st Qu.:0.0000   1st Qu.: 0.000  
 Irish                         :  8809   Median :0.0000   Median : 0.000  
 English                       :  4895   Mean   :0.4793   Mean   : 5.377  
 Italian (1990-2000, ACS, PRCS):  4531   3rd Qu.:0.0000   3rd Qu.: 0.000  
 Polish                        :  3113   Max.   :3.0000   Max.   :92.000  
 (Other)                       : 24309                                    
    HCOVANY         HCOVPRIV         SEX            EMPSTAT         EMPSTATD    
 Min.   :1.000   Min.   :1.000   Male  : 95222   Min.   :0.000   Min.   : 0.00  
 1st Qu.:2.000   1st Qu.:1.000   Female:101363   1st Qu.:1.000   1st Qu.:10.00  
 Median :2.000   Median :2.000                   Median :1.000   Median :10.00  
 Mean   :1.951   Mean   :1.691                   Mean   :1.514   Mean   :15.16  
 3rd Qu.:2.000   3rd Qu.:2.000                   3rd Qu.:3.000   3rd Qu.:30.00  
 Max.   :2.000   Max.   :2.000                   Max.   :3.000   Max.   :30.00  
                                                                                
    LABFORCE          OCC              IND           CLASSWKR       CLASSWKRD    
 Min.   :0.000   0      : 79987   0      :79987   Min.   :0.000   Min.   : 0.00  
 1st Qu.:1.000   2310   :  3494   7860   : 9025   1st Qu.:0.000   1st Qu.: 0.00  
 Median :2.000   5700   :  3235   8680   : 6354   Median :2.000   Median :22.00  
 Mean   :1.331   430    :  3025   770    : 6279   Mean   :1.116   Mean   :13.03  
 3rd Qu.:2.000   4720   :  2666   8190   : 5873   3rd Qu.:2.000   3rd Qu.:22.00  
 Max.   :2.000   4760   :  2563   7870   : 4041   Max.   :2.000   Max.   :29.00  
                 (Other):101615   (Other):85026                                  
    WKSWORK2        UHRSWORK         INCTOT           FTOTINC       
 Min.   :0.000   Min.   : 0.00   Min.   :  -7300   Min.   : -11800  
 1st Qu.:0.000   1st Qu.: 0.00   1st Qu.:   8000   1st Qu.:  35550  
 Median :1.000   Median :12.00   Median :  25000   Median :  74000  
 Mean   :2.701   Mean   :19.77   Mean   :  45245   Mean   : 107110  
 3rd Qu.:6.000   3rd Qu.:40.00   3rd Qu.:  56500   3rd Qu.: 132438  
 Max.   :6.000   Max.   :99.00   Max.   :1563000   Max.   :2030000  
                                 NA's   :31129     NA's   :10817    
    INCWAGE          POVERTY         MIGRATE1       MIGRATE1D    
 Min.   :     0   Min.   :  0.0   Min.   :0.000   Min.   : 0.00  
 1st Qu.:     0   1st Qu.:159.0   1st Qu.:1.000   1st Qu.:10.00  
 Median : 10000   Median :351.0   Median :1.000   Median :10.00  
 Mean   : 33796   Mean   :318.7   Mean   :1.122   Mean   :11.51  
 3rd Qu.: 47000   3rd Qu.:501.0   3rd Qu.:1.000   3rd Qu.:10.00  
 Max.   :638000   Max.   :501.0   Max.   :4.000   Max.   :40.00  
 NA's   :33427                                                   
    MIGPLAC1         MIGCOUNTY1         MIGPUMA1        VETSTAT      
 Min.   :  0.000   Min.   :  0.000   Min.   :    0   Min.   :0.0000  
 1st Qu.:  0.000   1st Qu.:  0.000   1st Qu.:    0   1st Qu.:1.0000  
 Median :  0.000   Median :  0.000   Median :    0   Median :1.0000  
 Mean   :  6.184   Mean   :  4.117   Mean   :  277   Mean   :0.8621  
 3rd Qu.:  0.000   3rd Qu.:  0.000   3rd Qu.:    0   3rd Qu.:1.0000  
 Max.   :900.000   Max.   :810.000   Max.   :70100   Max.   :2.0000  
                                                                     
    VETSTATD         PWPUMA00        TRANWORK         TRANTIME     
 Min.   : 0.000   Min.   :    0   Min.   : 0.000   Min.   :  0.00  
 1st Qu.:11.000   1st Qu.:    0   1st Qu.: 0.000   1st Qu.:  0.00  
 Median :11.000   Median :    0   Median : 0.000   Median :  0.00  
 Mean   : 9.412   Mean   : 1255   Mean   : 9.725   Mean   : 14.75  
 3rd Qu.:11.000   3rd Qu.: 3100   3rd Qu.:10.000   3rd Qu.: 20.00  
 Max.   :20.000   Max.   :59300   Max.   :70.000   Max.   :138.00  
                                                                   
    DEPARTS           in_NYC          in_Bronx       in_Manhattan    
 Min.   :   0.0   Min.   :0.0000   Min.   :0.0000   Min.   :0.00000  
 1st Qu.:   0.0   1st Qu.:0.0000   1st Qu.:0.0000   1st Qu.:0.00000  
 Median :   0.0   Median :0.0000   Median :0.0000   Median :0.00000  
 Mean   : 373.3   Mean   :0.3615   Mean   :0.0538   Mean   :0.04981  
 3rd Qu.: 732.0   3rd Qu.:1.0000   3rd Qu.:0.0000   3rd Qu.:0.00000  
 Max.   :2345.0   Max.   :1.0000   Max.   :1.0000   Max.   :1.00000  
                                                                     
   in_StatenI       in_Brooklyn      in_Queens      in_Westchester   
 Min.   :0.00000   Min.   :0.000   Min.   :0.0000   Min.   :0.00000  
 1st Qu.:0.00000   1st Qu.:0.000   1st Qu.:0.0000   1st Qu.:0.00000  
 Median :0.00000   Median :0.000   Median :0.0000   Median :0.00000  
 Mean   :0.02084   Mean   :0.126   Mean   :0.1111   Mean   :0.04413  
 3rd Qu.:0.00000   3rd Qu.:0.000   3rd Qu.:0.0000   3rd Qu.:0.00000  
 Max.   :1.00000   Max.   :1.000   Max.   :1.0000   Max.   :1.00000  
                                                                     
   in_Nassau          Hispanic         Hisp_Mex          Hisp_PR      
 Min.   :0.00000   Min.   :0.0000   Min.   :0.00000   Min.   :0.0000  
 1st Qu.:0.00000   1st Qu.:0.0000   1st Qu.:0.00000   1st Qu.:0.0000  
 Median :0.00000   Median :0.0000   Median :0.00000   Median :0.0000  
 Mean   :0.07032   Mean   :0.1387   Mean   :0.01626   Mean   :0.0436  
 3rd Qu.:0.00000   3rd Qu.:0.0000   3rd Qu.:0.00000   3rd Qu.:0.0000  
 Max.   :1.00000   Max.   :1.0000   Max.   :1.00000   Max.   :1.0000  
                                                                      
   Hisp_Cuban         Hisp_DomR           white             AfAm      
 Min.   :0.000000   Min.   :0.00000   Min.   :0.0000   Min.   :0.000  
 1st Qu.:0.000000   1st Qu.:0.00000   1st Qu.:0.0000   1st Qu.:0.000  
 Median :0.000000   Median :0.00000   Median :1.0000   Median :0.000  
 Mean   :0.003403   Mean   :0.02827   Mean   :0.6997   Mean   :0.125  
 3rd Qu.:0.000000   3rd Qu.:0.00000   3rd Qu.:1.0000   3rd Qu.:0.000  
 Max.   :1.000000   Max.   :1.00000   Max.   :1.0000   Max.   :1.000  
                                                                      
    Amindian           Asian            race_oth        unmarried   
 Min.   :0.00000   Min.   :0.00000   Min.   :0.0000   Min.   :0.00  
 1st Qu.:0.00000   1st Qu.:0.00000   1st Qu.:0.0000   1st Qu.:0.00  
 Median :0.00000   Median :0.00000   Median :0.0000   Median :0.00  
 Mean   :0.00378   Mean   :0.08656   Mean   :0.1324   Mean   :0.45  
 3rd Qu.:0.00000   3rd Qu.:0.00000   3rd Qu.:0.0000   3rd Qu.:1.00  
 Max.   :1.00000   Max.   :1.00000   Max.   :1.0000   Max.   :1.00  
                                                                    
    veteran        has_AnyHealthIns has_PvtHealthIns  Commute_car    
 Min.   :0.00000   Min.   :0.0000   Min.   :0.0000   Min.   :0.0000  
 1st Qu.:0.00000   1st Qu.:1.0000   1st Qu.:0.0000   1st Qu.:0.0000  
 Median :0.00000   Median :1.0000   Median :1.0000   Median :0.0000  
 Mean   :0.04443   Mean   :0.9513   Mean   :0.6906   Mean   :0.2997  
 3rd Qu.:0.00000   3rd Qu.:1.0000   3rd Qu.:1.0000   3rd Qu.:1.0000  
 Max.   :1.00000   Max.   :1.0000   Max.   :1.0000   Max.   :1.0000  
                                                                     
  Commute_bus      Commute_subway     Commute_rail     Commute_other    
 Min.   :0.00000   Min.   :0.00000   Min.   :0.00000   Min.   :0.00000  
 1st Qu.:0.00000   1st Qu.:0.00000   1st Qu.:0.00000   1st Qu.:0.00000  
 Median :0.00000   Median :0.00000   Median :0.00000   Median :0.00000  
 Mean   :0.02162   Mean   :0.07468   Mean   :0.01332   Mean   :0.05506  
 3rd Qu.:0.00000   3rd Qu.:0.00000   3rd Qu.:0.00000   3rd Qu.:0.00000  
 Max.   :1.00000   Max.   :1.00000   Max.   :1.00000   Max.   :1.00000  
                                                                        
 below_povertyline below_150poverty below_200poverty   foodstamps    
 Min.   :0.000     Min.   :0.0000   Min.   :0.0000   Min.   :0.0000  
 1st Qu.:0.000     1st Qu.:0.0000   1st Qu.:0.0000   1st Qu.:0.0000  
 Median :0.000     Median :0.0000   Median :0.0000   Median :0.0000  
 Mean   :0.122     Mean   :0.1965   Mean   :0.2676   Mean   :0.1465  
 3rd Qu.:0.000     3rd Qu.:0.0000   3rd Qu.:1.0000   3rd Qu.:0.0000  
 Max.   :1.000     Max.   :1.0000   Max.   :1.0000   Max.   :1.0000
 
 #5. To my understanding, the "hot hands fallacy" is the belief that consecutive successes will continue to lead to success and consecutive failures will
 continue to lead to failure. The hot hand fallacy is common in gambling and investing. For example, if a stock price increases multiple days in a row,
 you may believe it will continue to increase, for no other reason than because it has been consecutively successful. This may lead to overconfidence and
 riskier behavior. S&P 500 supposedly has a 10-11 percent average annual return from 1926-2018.
