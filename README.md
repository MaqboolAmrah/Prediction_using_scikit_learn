# Prediction_using_scikit_learn
Python
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
import random
import seaborn as sns; sns.set_theme()
from sklearn import datasets,linear_model
from sklearn.model_selection import train_test_split
!pip install pandas
amrah = pd.read_csv("C:\\Users\\MC\\Documents\\Academia.csv")
amrah.head()
amrah.tail()
print(type(amrah))
sns.set()
sns.set(color_codes=True)
sns.barplot(amrah['Degree Title'], amrah['%'])
sns.distplot(amrah['%'])
sns.displot(amrah['CGPA'])
sns.barplot(amrah['Degree Title'], amrah['%'], amrah['Ob Marks'],amrah ['Max Marks'] )
sns.jointplot(amrah['Grade'], amrah['University Name'], amrah['Ob Marks'])
sns.pairplot(amrah[['Grade', '%', 'Ob Marks']])
