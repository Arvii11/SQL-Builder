# SQL Builder

This project converts a CSV file into SQL database schema and corresponding insert statements, with plans to include image data support.

## Project Overview

The project utilizes Python and pandas to achieve the following:
- Reads a CSV file (`booth.csv` by default) and detects column data types (`INT`, `TEXT`, `DATETIME`, `DATE`).
- Generates a SQL `CREATE TABLE` statement based on the CSV columns and inferred types.
- Creates SQL `INSERT` statements for each row in the CSV.

## Requirements

To run this project, ensure you have:
- Python (version 3.x recommended)
- pandas library

## Usage

1. **Setup:**
   - Place your CSV file (`booth.csv`) in the project directory.

2. **Execution:**
   - Run the script `main.py`.
   - Example:
     ```bash
     python main.py
     ```

3. **Output:**
   - The script outputs:
     - A `CREATE TABLE` SQL query.
     - Multiple `INSERT INTO` SQL queries.

## Future Planning

- **Image Support:** Future versions will include functionality to handle image data.

## Customization

- **Column Types Detection:** Modify regex patterns in the `column_types` function to support different data formats.
