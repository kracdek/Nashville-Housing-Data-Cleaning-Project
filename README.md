# Nashville Housing Data Cleaning Project

## Introduction
This is a portfolio project for data cleaning using MySQL for a dataset - Nashville Housing. It required an intensive data cleaning process. The client expected the data to be such cleaned that in future any analysis could be performed on it easily and effectively. For this purpose I used my extensive data cleaning checklist. 


## Tools
This project uses following languages/tools
* Microsoft Excel : To understand the dataset we are dealing with.
* MySQL : For Cleaning Data


## Project 
The aim of the project is to ensure that at the end of this ETL and Data wrangling process, the data extremely neat and 'ready to be analyzed' or 'stored for future use' data

## Data

Home value data for the booming Nashville market with 56,000+ rows altogether. The dataset can be found below:

   - [Nashville Housing Data](https://www.kaggle.com/tmthyjames/nashville-housing-data)
   


## Functions used for Data Cleaning - 
- CONVERT()
- ISNULL()
- CASE WHEN
- SUBSTRING()
- CHARINDEX()
- PARSENAME()
- REPLACE()
- Used CTEs - Row_Number()



## Data Cleaning 
The following is used for the data cleaning for this data set

- Standardized date format using `CONVERT` and updated the table. 
- By using a `SELF JOIN`, populated the *PropertyAddress* fields where the value is `NULL`.
- Broken out *PropertyAddress* and *OwnerAddress* fields into individual columns using `SUBSTRING` and `PARSENAME` functions.
- Changing Y and N to Yes and No in the *SoldAsVacant* field using `CASE` statement. 
- Removed Duplicates using `ROW_NUMBER`, `PARTITION BY`, and `CTE`. 
- Deleted a few unused fields using the `DROP` command.
  

Checkout my [Data Cleaning SQL code here](https://github.com/kracdek/Nashville-Housing-Data-Cleaning-Project/blob/main/NashvilleHousing%20Data%20Cleaning.sql)


## Remarks
Having clean data will ultimately increase overall productivity and allow for the highest quality information in our decision-making.
