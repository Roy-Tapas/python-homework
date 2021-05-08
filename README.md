# python-homework repository
Python homework for Module-2

This repository contains the solved homework for "PyBank" - Python script for analyzing the financial records of a fictitious company 

## Solution components
**1. Module fin_module.py** <br>
For better mudularity, readibility, reusabaility and maintainability, core computation of business logic is separated from main and kept in this module in the form of a function as described following.

**2. calculate_fin_metrics()** <br>
This function resides in the above mentioned module that houses the business logic of all core calculation for desired metrics
This function takes a dictionary "budget_data" as argument with "date" as key and "pnl amount" as value in the dict and 
return the required metrics in a python list

**3. main.ipynb**
This is the main script that reads the budget_data.csv, loop through the records and forms a dictionary with date and pnl amount. 
Then main calls calculate_fin_metrics() inside fin_module by passing the dictionary as formed from budget_data.csv
Main then catches the return values of calculate_fin_metrics() in a list and print individual list elements to report the metrics in the desired format.
Main also writed these metrics in a txt file.

**4. bidget_data.csv file**
This is the input file to main.ipynb script. 
This has monthly pnl with one record for each month
Each record has two columns - (1) date and  (2) pnl amount

## How to run the script
Clone the entire "python-homework" repository into a local folder by issuing the following command from gitbash
$git clone https:\\

open Jupyter lab by issuing the following command from gitbash:
$Jupyter lab

Then open main() in jupyter notebook and run each cells one after another

## Important points to note
Retail the folder structure as clones from github. Else path set inside the main is not going to work. 
Hierarchy inside repository should look like following:

python-homework
     |
     |-------> PyBank
        |
        |---------------> fin_module.py
        |---------------> main.ipynb
        |---------------> output.txt
     |------> PyRamen
     |------> Resources
        |---------------> budget_data.csv
        |---------------> menu_data.csv
        |---------------> sales_data.csv
     |------> README.md

Scripts for PyRamen is under user acceptance testing. Stay tuned. 



