# Data_Scince
#Removing duplicates


import numpy as np
import pandas as pd
from pandas import Series, DataFrame

DF_obj = DataFrame( { 'column1':[1,2,3,3,4,4,4,],
                       'column2':['a','a','b','b','c','c','d'],
                     'column3':['A','A','B','B','C','F','D']})
DF_obj

DF_obj.duplicated()

#DF_obj.drop_duplicates()

DF_obj.drop_duplicates(['column3'])
