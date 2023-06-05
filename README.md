# Data Cleaning Project: Nashville Housing Data

This project focuses on cleaning and preprocessing the Nashville Housing Data to ensure data integrity and prepare it for further analysis. The dataset contains information about various properties in Nashville, including their unique identifiers, land use, sale details, property addresses, owner information, and other relevant attributes.

## Objective

The main objective of this data cleaning project is to address missing values, correct inconsistencies, and format the data appropriately. By performing these tasks, we aim to create a clean and reliable dataset for further analysis and insights.

## Project Structure

The project contains the following files:

- `data_cleaning.ipynb`: Jupyter Notebook containing the Python code for data cleaning.
- `Nashville Housing Data.csv`: The raw dataset in CSV format.
- `cleaned_housing_data.csv`: The cleaned dataset obtained after data cleaning.

## Data Cleaning Steps

The data cleaning process involves the following steps:

1. Importing libraries: The necessary libraries, including Pandas and NumPy, are imported to facilitate data analysis and manipulation.
2. Loading the dataset: The raw dataset, `Nashville Housing Data.csv`, is loaded into a Pandas DataFrame.
3. Exploring the dataset: Initial exploration is conducted to understand the structure, shape, and content of the dataset.
4. Handling unique values: Each column's unique values are inspected to identify any inconsistencies or incorrect representations.
5. Handling "SoldAsVacant" column: In this step, the "SoldAsVacant" column values are standardized by replacing 'N' with 'No' and 'Y' with 'Yes'.
6. Addressing missing data: Missing values in the dataset are identified and handled appropriately. Specifically, the missing values in the "PropertyAddress" column are filled using forward-fill method based on the corresponding ParcelID.
7. Cleaning duplicated data: Duplicated rows in the dataset, identified by the ParcelID column, are examined and resolved.
8. Data transformations: The data is transformed by separating the PropertyAddress column into StreetAddress and CityAddress columns. Additionally, a new State column is added with values set to 'TN' (Tennessee).
9. Dropping unnecessary columns: The OwnerAddress column, which is redundant with the PropertyAddress column, is dropped from the dataset.
10. Data type conversion: The SaleDate column is converted to the datetime data type for further analysis.

## Results

The data cleaning process successfully addresses missing values, corrects inconsistencies, and formats the dataset. The resulting cleaned dataset, `cleaned_housing_data.csv`, is available for further analysis and insights.

## Conclusion

The data cleaning project ensures the reliability and accuracy of the Nashville Housing Data by handling missing values, correcting inconsistencies, and formatting the dataset appropriately. The cleaned dataset can be used for various purposes, such as data analysis, modeling, and visualization, to gain meaningful insights into the Nashville housing market.

Feel free to explore the cleaned dataset and utilize it for your specific data analysis needs!

**Note:** The cleaned dataset is provided as a separate file, `cleaned_housing_data.csv`, in the project repository.

If you have any questions or suggestions, please feel free to reach out.

Happy data cleaning and analysis!
