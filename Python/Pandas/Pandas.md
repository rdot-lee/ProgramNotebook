
###### Reading data files
``` python
pd.read_csv("path", index_col = 0)
```

###### To capture the first five rows in DataFrame.
``` python
df.head()
```

###### Check how large the resulting DataFrame
``` python
df.shape
```

###### Set and Reset control how the pandas library is displayed
``` python
pd.set_option("display.max_rows", 10)

pd.reset_option("display.max_columns")
```

###### Take the value of col
```Python
df.col_name

df['col_name']
```

#### row, col 
|  ----   | col0  | col1  |
|  ----    | ----   |  -|
|  row0 | 123  | 789    |
|  row1 | 345  | 000    |

###### Index-based selection
```Python
df.iloc[0] # select the first row of data
df.iloc[row, col] 
```

###### Label-based selection
```Python
df.loc[col, row_Label_Name]
```

###### Conditional selection
```Python
df.loc[df.label.isin(['A', 'B'])]

df.label.isnull() # If there is NULL in the table, output true

df.label.notnull() # If there isn't NULL in the table, output true
```

###### Summary functions
```Python
# comprehensive data
df.describe()
df.label.describe()

# remove identical tuples or arrays
np.unique()
df.label.unique()

# calculate average
df.mean()

# To see a list of unique values and how often they occur in the dataset
df.value_counts()

# Display the index of the row with the largest value in the columns
df.col.idxmax()

```

###### Summary functions
```Python

```

