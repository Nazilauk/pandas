# Project Name: Data Selection with pandas

## Description:
This project demonstrates how to select data from a dataset using pandas library. It shows different ways of selecting rows and columns and how to sort the data based on a variable. Pandas provides many powerful data manipulation functions, which makes it easy to perform data selection and manipulation tasks.

## Table of Contents:
- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)

## Installation:
1. Download and install Anaconda distribution of Python
2. Open Jupyter Notebook
3. Create a new Notebook
4. Install pandas library using !pip install pandas
5. Load the dataset using pandas read_csv function

## Usage:
1. Selecting rows and columns
	- Use iloc for selecting rows and columns by their index numbers
	- Use loc for selecting rows and columns by their labels
2. Sorting the data
	- Use sort_values function to sort data by a variable
3. Displaying data
	- Use print function to display data in console
	- Use plot function to display data in graphical form
4. Modifying data
	- Use loc and iloc to modify values in a dataframe

### Example:

#### Select the 'Limit' and 'Rating' columns of the first five observ
```pandas
df.iloc[:5, [3, 4]]
```
We use iloc method to select rows and columns by their index numbers. Here, we are selecting first five rows and columns with index numbers 3 and 4, which correspond to 'Limit' and 'Rating'.

#### Select 3 column and 9 rows
```pandas
df.loc[:8, ['Balance','Income','Gender']]
```
We use loc method to select rows and columns by their labels. Here, we are selecting first 9 rows and columns 'Balance', 'Income', and 'Gender'.

#### Select the first five observations with 4 cards
```pandas
df.loc[:4,['Cards']]
```
We use loc method to select rows and columns by their labels. Here, we are selecting first five rows and 'Cards' column.

#### Sort the observations by 'Education'. Show users with a high education value first. 
```pandas
df.sort_values(by ='Education',ascending = False).head()
```
We use sort_values function to sort data by 'Education' column in descending order. head function is used to show first five observations.

#### Select all rows and upto and including the 5th row of the dataframe and all columns 
```pandas
df.loc[ :5, :]
```
We use loc method to select rows and columns by their labels. Here, we are selecting all rows upto and including the 5th row and all columns.

#### Select all rows and all columns in dataframe.
```pandas
df.iloc[:,:]
```
We use iloc method to select all rows and all columns in dataframe.

#### Select all the rows starting from 6th row and all columns stating from 6th column 
```pandas
df.iloc[5:,5:]
```
We use iloc method to select rows and columns by their index numbers. Here, we are selecting all rows starting from 6th row and all columns starting from 6th column.

#### Select all rows in first column of the dataframe
```pandas
df.iloc[:,0]
```
We use iloc method to select all rows in first column.

#### Selects the entire row 10th with their heading names
```pandas
df.iloc[9,:]
```
We use iloc method to select 10th row with all columns. 

### Screenshots:

![Pandas](https://github.com/Nazilauk/pandas/assets/127387087/054d9775-0a94-4dbe-b92b-0d46a78ede16)

### Credits:
This project was created by Nazila Zadeh

