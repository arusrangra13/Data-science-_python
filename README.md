# Data-science-_python
basic of data science
import pandas as pd 

df_employess = pd.DataFrame ({'employee_id':[1,2,3],
                                             'name':['Arus','shiv','raj'],
                                             'department_id':[101,102,103]})

df_department = pd.DataFrame ({'department_id':[101,102,103],
                               'department_name':['HR','SALES','MARKETING']})

merge_df = pd.merge(df_employess,df_department,on='department_id',how='left')
print(merge_df)
