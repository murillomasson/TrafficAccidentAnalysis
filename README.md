# TrafficAccidentAnalysis
This project focuses on analyzing traffic accidents that have occurred and been recorded in Porto Alegre over the past four years. The goal is to gain insights into the patterns, causes, and trends of these accidents in order to improve road safety measures.

## Project Overview and Functionality
The Main file performs the following functions:

- Connects to the endpoint of the open data from Porto Alegre.
- Connects to AWS S3.
- Creates a session in PySpark, a dataframe, and connects it to the endpoint data.
- Performs data cleaning.

The Tests file:

- Connects to the sharpfile.
- Reads it into a Pandas dataframe.
- Executes column comparisons to enable proper address cleaning for joining with the traffic accident table.
- Performs some preliminary analysis and tests to enhance understanding of the dataset.

## Prerequisites
Before running the program, make sure to set the environment variables with the values of your AWS S3 account. If you don't want to save the database in AWS, you will need to comment out the relevant code sections in the main function (fifth cell).

Please note that this project was created using Anaconda dependencies, so it may not work in environments outside of Anaconda.

## Installation
To install the required dependencies, run the following command at the root of the project, where the requirements.txt file is located:

```pip install -r requirements.txt```

## Usage
- Load the Jupyter Notebook.
- Execute the main function.
- After running the main function, you can execute the tests to verify the correctness of the analysis.

## Output
The script generates a CSV file after execution, which can be further analyzed using various data visualization tools.

## Data Reliability
The data used in this project is provided by https://dadosabertos.poa.br. The reliability of the data is the responsibility of the source. You can explore other endpoints available on their website.
The data cleaning and analysis performed in this project correspond to the data provided until May 29th. It may be necessary to execute additional functions to extract more up-to-date data in the future.

Feel free to explore the code and customize it according to your needs. Happy analyzing!
