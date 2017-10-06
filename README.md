# python lightning talk

## What is this?

This repo / notebook relates to a short talk on Python / Pandas at the University of Melbourne.

This is a Python / Pandas demonstration, not a tutorial. I am primarily trying to show how an excel-type workflow might be done with Python

## Variables and functions

Of course, it's hard to demonstrate anything in Python withoutr using tools and concepts that may be unfamiliar. Let's get two of these out of the way.

Whenever you see a single equals sign in Python, it reflects the creation (or 'assigment') of a `variable`.  

A variable is a label for a location in memory. It can be used to hold a value.

Creating, and manipulation variables lies at the heart writing python code.

Reusing code is also essential to programming. A function is a block of organized, reusable code that is used to perform a single, related action. a Python function is always followed by round brackets:

```python
someFunction(someVariable)
```

In this demonstration we'll only use functions provide to us by the core Python language, and it's libraries. But defining your own functions is easy.


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

https://tutorial.djangogirls.org/en/python_introduction/

http://swcarpentry.github.io/python-novice-inflammation/

https://github.com/jrjohansson/scientific-python-lectures

https://python.swaroopch.com/

https://dansand.gitbooks.io/resguides-research-with-jupyter/content/?q=

https://www.youtube.com/channel/UCscdxGKSj4hOaVFYvslW1-g/playlists

## Notes

#### Pandas vs. R

http://pandas.pydata.org/pandas-docs/stable/comparison_with_r.html#comparison-with-r-r-libraries

#### Migrating from excel

```
df = pd.read_excel("excel-comp-data.xlsx")
```
http://pbpython.com/excel-pandas-comp.html
