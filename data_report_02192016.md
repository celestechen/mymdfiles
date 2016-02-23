RWJ Sepsis Data Report Outline
-------------
**Action Items**

| ITEM | RESULTS/OUTPUT |
| ------- | ------ | 
|Xinwei to check for duplicate records in dataset| P1|
|Percentage of patients with a positive blood culture | 82 Patients had at least one positive reading; that is 13.20% of patients who had blood cultures and 3.27% of total sample patients. --see output 1 on P2|
|What is the pattern of a positive blood culture in the total number of blood cultures taken for an individual patient? <BR> --It’s important to understand the time frame between ordering and a positive reading | --pattern frequency report -- see output 2<br> --first positive reading pattern --see output 3 <br> --how many positive readings --see output 5 <br> --summary of time frame between ordering and first positive reading: The average time is 1.42 days between first positive and order date; 1.93 days between first positive and first order date.. --see output 6|
| What is the most common primary diagnosis? What is the most common non-primary diagnosis? <BR> --Frequency report for both| Most common primary diagnosis: Rehabilitation proc NEC <br> most common non-primary diagnosis:  Hypertension NOS|
|Review records/encounters that are missing diagnosis codes, why is there a difference between number of encounters and diagnosis codes?| 78 patients: --created a dataset ```encounter_nodx.sas7bdat``` |
|Why are about 200 people not getting labs taken? Is this correct?| 145 patients: -- created a dataset ```encounter_nolabs.sas7bdat```|
|Frequency report for order name|8702 levels—only provide 20 most common |
|Frequency report for top 20 ordered labs <BR> --Review possible values <BR> --How are labs being reported?| *Note*:Lab result value is not numeric-- need further instruction on how to clean it.|
|What are the possible values for unit_master_care_type?||
|Basic vitals: <BR> --What is the range? <BR> --Total number recorded for an individual patient <BR> -- Screen for outliers <BR>--Mean, min, max, IQR|Note: Vitals are grouped into Basic & ICU-only. Vital_sign_value is not numeric for ICU-only vitals.  |
|Frequency table for order_name||
|Frequency table for order_type_description||
|Pull 10 records and list all potential variables, will be able to see some of the values being reported||
|LOS should be equal to day_length| Yes can confidently confirm this.|
|Frequency table for service code||
|Frequency table for service description|  df |





