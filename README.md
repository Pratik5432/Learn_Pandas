# Pandas
* It is a fast, powerful, flexible and easy to use open source python library used for data analysis and manipulation.

## Pandas Series
* It is like a column in a table.
* It is a 1-D array holding data of any type.

* Series will return an index and the tuple.
* For custom index use parameter: pd.Series(col_name, index=[])
* pd.Series(col_name, index=[], name='any_name')           # For additional information
* While importing from a dataset with only 1 col: pd.Series('file_path', squeeze=True)
* While importing from a dataset with 2 col: pd.Series('file_path', index_col='col_name', squeeze=True)
* Series does not support negative indexing. (when the index is number)
 
#### Series Creation
* Lists: pd.Series(my_list)
* A column in a table: pd.Series(col_name)

#### Series Attributes
* series_marks.size
* series_marks.dtype
* series_marks.name
* series_marks.is_unique
* series_marks.index
* series_marks.values

#### Series Methods
* series_marks.head()
* series_marks.tail()
* series_marks.sample()
* series_marks.value_counts()
* series_marks.sort_values()          # ascending=False, inplace=True (Be careful will using inplace parameter)
* series_marks.sort_index()

* series_marks.count()
* series_marks.size()
* series_marks.min()
* series_marks.max()
* series_marks.sum()
* series_marks.product()
* series_marks.mean()
* series_marks.median()
* series_marks.mode()
* series_marks.std()
* series_marks.var()
* series_marks.describe()

* series_marks.astype()
* series_marks.between(51, 99)    # between 51 and 99
* series_marks.drop_duplicates()
* series_marks.duplicated()
* series_marks.isnull()
* series_marks.dropna()
* series_marks.fillna()
* series_marks.isin()
* series_marks.apply()
* series_marks.copy()
* series_marks.unique()
* series_marks.nunique()

#### Series with Python functionality
* len(series_marks)
* type(series_marks)
* dir(series_marks)
* sorted(series_marks)
* min(series_marks)
* max(series_marks)

* list(series_marks)                # type conversion
* dict(series_marks)
------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Pandas Dataframe

#### Dataframe Attributes
* marks.shape
* marks.dtypes
* marks.columns
* marks.index
* marks.values

#### Dataframe Methods
* marks.info()
* marks.describe()
* marks.head()
* marks.tail()
* marks.sample()
* marks.isnull()
* marks.rename(columns{'col1':'new_col'})
* marks.value_counts()
* marks.sort_values()          # ascending=False, inplace=True (Be careful will using inplace parameter)
* marks.sort_index()
* marks.duplicated()
* marks[''].astype()
* marks.isdigit()
* marks.rank()                # ascending=False
* marks.set_index('')         # Only works in datadrame, not on series
* marks.reset_index()
* marks.dropna()              # parameter: how='all','any'; subset=['col1', 'col2']
* marks.fillna()
* marks.drop_duplicates()
* marks.apply()

#### Selecting columns from a dataset in dataframe
* Single column: marks['']
* Multiple columns: marks[ ['', '', ''] ]

#### Searching rows from a dataset in dataframe
* iloc: searches using index positions. eg: marks.iloc[]
* loc: searches using index labels. eg: marks.loc[]
