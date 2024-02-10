
# Program Description

This program processes data from three CSV files: File A containing training datasets, File B containing a test dataset, and File C containing datasets for ideal functions. All data consists of x-y pairs of values. The program performs data visualization, calculations, and stores the results in a SQLite database.

## Functionality

- The program selects ideal functions for the training function based on how they minimize the sum of all y-deviations squared (Least-Square).
- The criterion for mapping individual test cases to the four ideal functions is that the existing maximum deviation of the calculated regression does not exceed the largest deviation between the training dataset (File A) and the ideal function (File C) chosen for it by more than a factor of sqrt(2).

## Libraries and Packages

Libraries and packages used include:

- **pandas**: For reading the CSV files and DataFrame data structure.
- **numpy**: For mathematical calculations.
- **matplotlib.pyplot**: For visualization.
- **sqlalchemy**: For creating the database where results are stored.
- **prettytable**: For displaying tables in a visually appealing way.

# Getting Started

To successfully run this program, follow these steps:

1. **File Requirements:**
   - Both 'ideal functions' and 'training datasets' files must have same 'x' values.
   - The 'test dataset' file 'x' values must be part of 'training datasets' file.

2. **Dependency Installation:**
   - Make sure you have all the necessary dependencies installed. You can install them using the following command:
     "pip install pandas numpy matplotlib sqlalchemy prettytable"

4. **Running the Program:**
   - Execute the program and follow the prompts to input the names of your CSV files.

5. **Review the Results:**
   - After execution, review the generated SQLite database for the processed results.

Now you're ready to explore and analyze your data using this program!



