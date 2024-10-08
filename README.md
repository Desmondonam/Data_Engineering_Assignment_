# Data_Engineering_Assignment_

## Data Engineering Assignment: Loading Data from Different File Formats and Databases

### Objective:
This assignment aims to test students' ability to work with various data formats and databases. Students will be required to load data from different file formats (CSV, JSON, Excel) and from a database (MySQL). They should demonstrate how to read, process, and analyze the data using Python.

#### Requirements:
Data Formats: Students will work with the following data formats:

- CSV (data.csv)
- JSON (data.json)
- Excel (data.xlsx)
- Database: A MySQL database will be provided containing the same data as the files for consistency.

Python Libraries:

- pandas
- mysql-connector-python or SQLAlchemy
- json
#### Assignment Steps:
##### Part 1: Setup the Environment
Install the necessary Python libraries using the following command:

`pip install pandas mysql-connector-python openpyxl`

### Download the data:

- data.csv
- data.json
- data.xlsx
The data for all formats is the same and contains the following columns:

    - id: Unique identifier for each entry.
    - name: Name of a product.
    - category: Category to which the product belongs.
    - price: Price of the product.
    - quantity: Quantity available in stock.
MySQL Database Setup: The MySQL database is named store_db, with a table named products that contains the same data as the files. The table structure is as follows:

`CREATE TABLE products (`
 `   id INT PRIMARY KEY,`
  `  name VARCHAR(255),`
  `  category VARCHAR(255),`
  `  price DECIMAL(10, 2),`
  `  quantity INT`
`);`

Sample data to insert into the products table:

`INSERT INTO products (id, name, category, price, quantity) VALUES`
`(1, 'Laptop', 'Electronics', 1000.00, 50),`
`(2, 'Keyboard', 'Electronics', 50.00, 200),`
`(3, 'Desk Chair', 'Furniture', 150.00, 80),`
`(4, 'Pen', 'Stationery', 2.00, 500);`



## Part 2: Loading and Processing the Data
- Load the CSV Data:

Use Python's pandas library to load data from data.csv.

- Load the JSON Data:

Use Python's json and pandas libraries to load data from data.json.
- Load the Excel Data:

Use pandas to load data from data.xlsx.

- Load Data from MySQL:

Use mysql-connector-python to connect to a MySQL database and retrieve the data.

## Part 3: Analysis Task
Summarize Data: For each dataset (CSV, JSON, Excel, MySQL), provide the following:

- Total number of products.
- Average price of products.
- Total quantity of products.