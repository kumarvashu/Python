# Badly Structured Sales Data Cleanup

This Python script is designed to clean and restructure badly structured sales data in an Excel file. It uses the Pandas library to perform data manipulation and cleaning tasks. The script follows these main steps:

1. **Data Loading**: It loads the sales data from an Excel file specified by the `excel_file_location` variable.

2. **Data Restructuring**: The script stacks the columns to create a multi-indexed DataFrame for better data organization.

3. **Header Renaming**: The column headers are renamed for clarity using a dictionary. The renaming process helps make the data more understandable.

4. **Column Deletion**: The 'To be deleted' column is removed from the DataFrame as it's no longer needed.

5. **Data Filtering**: Rows containing 'Home Office Total,' 'Consumer Total,' 'Corporate Total,' and 'Grand Total' are removed from the DataFrame, leaving only relevant sales data.

6. **Data Sorting**: The cleaned DataFrame is sorted by the 'Segment' and 'Ship Mode' columns for better presentation and analysis.

7. **Data Export**: Finally, the cleaned and structured data is saved to a new Excel file specified by the `stacked_df.to_excel()` function.

## Prerequisites

Before running the script, ensure that you have the following:

- Python 3.x installed on your system.
- The Pandas library installed (you can install it using `pip install pandas`).
- An Excel file with sales data in the specified format.

## Usage

1. Modify the `excel_file_location` variable to point to your Excel file with sales data.

2. Run the script using a Python environment (e.g., Jupyter Notebook, VSCode, or a Python IDE).

3. The cleaned and structured data will be saved to a new Excel file (`Badly_Structured_Sales_Data_test_2.xlsx` by default) in the same directory as the script.

## Author

[Vashu Kumar]((https://github.com/kumarvashu)

## License

This project is licensed under the MIT License. See the [LICENSE.md](LICENSE.md) file for details.
