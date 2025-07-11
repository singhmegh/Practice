##Day 01:
- Value_Counts() : How many times each unique value appears
- For Average : .mean()
- To find null values : isnull() 
- After finding Null values use bfill()/ffill() to fill the value.
- .shape tells you the dimensions of your DataFrame (or array).It returns a tuple.

##Day 02 :
  - groupby is used to make a group of two components.
  - .sort_values is used to ascending/descending the data.
  - for save the dataframe we used .to_csv/.to_excel("new name", index=false).
  - index= False : prevents Pandas from writing row numbers into the CSV
  - for replace we use (data[ ].replace(np.nan, " replace value ")).

##Day 03:
    -idxmax/idxmin give the highest/lowest count
    -normalize=True: gets percentage instead of count.
    -.unstack(): makes the result into a table with rows as gender and columns as survival status.
    -legend only shows for single rows/raw data ,for multiple legend we use patches.
    -#data.loc[...] retrieves the full row for that index.

##Day 04 :
    - autopct="%1.1f%%" shows percentage on slices
    -dropna() it drop missing values
    - alpha ranges from 0.0 to 1.0 ,0.0 → completely transparent ,1.0 → completely opaque  
    -.notna() is a method in Pandas that returns True for non-missing values (i.e., values that are not NaN), and False for missing values (NaN).
