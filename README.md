In LAB 2, we analyzed the World Energy dataset (WorldEnergy.csv) by developing a custom tool, LAB 2 CODING, to conduct Exploratory Data Analysis (EDA) and generate insightful visualizations
We focused our analysis on Sweden, as its data proved to be exceptionally reliable, requiring only minor cleaning. To better understand the country’s energy landscape, we specifically selected columns that demonstrated a strong potential relationship with Sweden's energy trends and performance.
1st step is we do the data filtering : which is filtering the column that we choose the related column to keep such as Year, Population, Gdp, Biofuel_Consumption, Coal_Consumption, Fossil_Fuel_Consumption, Gas_Consumption, Hydro_Consumption, Nuclear_Consumption, Oil_Consumption, Primary_Energy_Consumption, Solar_Consumption, Wind_Consumption 
2nd step is create a dataframe to the modified data set name df=data['columns_to_keep']
3rd step is we perform some filtering method to extract only country : Sweden data 
4th step is to rename all the column name into UPPER CASE letter
5th step is to perform counting missing values per column using .isnull().sum method 
6th step from teh table we can see that the GDP value missing is just 2 location. By then we decide to clean the data using interpolate (linear) method since the trend is linear 
7th step is to drop all the rows column for the tear that is missing value or NaN, since the data is missing it values starting from year 1900 to year 1964 and save into data frame name df_cleaned_rows
8th to checks for and counts any identical rows in your filtered Sweden dataset. 
9th to spot for any outlier exist in the data 
10th to clean all the possible outlier from the data set and save it on a new dataframe that is df_cleaned
11th print the df_cleaned data. from the data we can see that it have a zero value but it is acceptable since we treat 0 / zero as a real result/true quantity and its incerement to the numeric is small from zero to values
