# python lightning talk

## What is this?

## Wild speculations

## Variables and functions

A variable is a label for a location in memory. It can be used to hold a value. If we imagine the variable as a sticky note with a name written on it, assignment is like putting the sticky note on a particular value:+




## Let's do something


```python

import pandas as pd
from urllib import urlretrieve

#a string containing the data URL
URL = 'http://scrippsco2.ucsd.edu/assets/data/atmospheric/stations/in_situ_co2/weekly/weekly_in_situ_co2_mlo.csv'

#retrieve data and save locally
urlretrieve(URL, 'MaunaLoa.csv')

#this needs to be completed
df = pd.read_csv('MaunaLoa.csv' ...)

df.head(2)

#import and configure plotting
import matplotlib.pyplot as plt
%matplotlib inline

```

## Learning

### Courses

https://dansand.gitbooks.io/resguides-research-with-jupyter/content/?q=

## Notes

#### Pandas vs. R

http://pandas.pydata.org/pandas-docs/stable/comparison_with_r.html#comparison-with-r-r-libraries

#### Migrating from excel

```
df = pd.read_excel("excel-comp-data.xlsx")
```
http://pbpython.com/excel-pandas-comp.html
