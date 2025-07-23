### Day 01:
- Value_Counts() : How many times each unique value appears
- For Average : .mean()
- To find null values : isnull() 
- After finding Null values use bfill()/ffill() to fill the value.
- .shape tells you the dimensions of your DataFrame (or array).It returns a tuple.

### Day 02 :
  - groupby is used to make a group of two components.
  - .sort_values is used to ascending/descending the data.
  - for save the dataframe we used .to_csv/.to_excel("new name.csv/.excel", index=false).
  - index= False : prevents Pandas from writing row numbers into the CSV
  - for replace we use (data[ ].replace(np.nan, " replace value ")).

### Day 03:
- idxmax/idxmin give the highest/lowest count.
- normalize=True: gets percentage instead of count.
- .unstack(): makes the result into a table with rows as gender and columns as survival status.
- legend only shows for single rows/raw data ,for multiple legend we use patches.
- data.loc[...] retrieves the full row for that index.

### Day 04 :
- autopct="%1.1f%%" shows percentage on slices.
- dropna() it drop missing values.
- alpha ranges from 0.0 to 1.0 ,0.0 → completely transparent ,1.0 → completely opaque.
- .notna() is a method in Pandas that returns True for non-missing values (i.e., values that are not NaN), and False for missing values (NaN).
### Day 05 :
- (r',\s*(\w+\.)'):This is a regular expression (regex) used with str.extract() to pull out the title (like Mr., Mrs., Dr.) from the Name column in the  dataset.
- hue enable proper palette usage
- na avoid error if there is NaN value ,na = False
- \b means boundary so it did not count word like theodore.(r'\bthe\b').

### Day 06 :
- pd.cut() splits continuous values into discrete bins.
- bins=4 it split it into 4 equal width-interval
- (r"^(\w+),") : it capture the lastname 
- plt.ylim(0, 100) : It sets the y-axis limits of your plot from 0 to 100, which makes sense when you’re plotting percentages (survival rate).

### Day 07 :
- (sum/count)*100	Converts the survival rate to percent.
- Use agg(['count', 'sum']) when you want to:
- 1 Analyze survival rate
- 2 Keep group-wise structure
- 3 Perform further calculations
- Use value_counts() only when you want detailed breakdowns, but not for rate calculations directly.
- pd.qcut():You want to divide data by distribution, like quartiles or deciles.
- sum: total no. of survivors.
- count : total no. of people in group.

### Day 08 : 
- Number of Bins = Number of Edges − 1
- 5 intervals = 5 labels

### Day 09 :
- Fare brackets mean dividing the continuous range of ticket prices (Fare) into discrete intervals (groups) to make analysis easier.

### Day 10 :
- expand=False returns a Series instead of a DataFrame.
- .str.strip(): This removes any leading or trailing whitespace from the extracted title.
- A pivot_table is a powerful tool to summarize and aggregate data.

### Day 12 :
- .size().unstack() → creates a DataFrame with Survived=0 and Survived=1 as columns
-  max ensures all fares are included.
- .apply(...) → applies a function to each row in the Fare column.
- lambda x: x > avg_fare → anonymous function:
-   1) x is the fare for each passenger.
-   2) It checks: is this fare > average fare?
-   3) Returns True if yes, False if not.
 
### Day 15 :
- .map i encode the Sex column into 0 & 1
- i make a new dataset from old data then split it into x,y
- i apply train_test_split to distribute the data
- then apply logistic regression model
- its testing & training accuracy is something 78% & 79% respectively and it predict accurately almost.
- lastly i make confusion matrix.