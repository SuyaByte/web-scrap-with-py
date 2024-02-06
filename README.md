# web-scrap-with-py
Webscraping a website using python

## Objectives:
1. Use the requests and BeautifulSoup libraries to extract the contents of a web page.
2. Analyze the HTML code of a webpage to find the relevant information.
3. Extract the relevant information and save it in the required form.

## Scenario:
To extract the information of the top 50 movies with the best average rating from the web link [100 Most Highly Ranked Films](https://web.archive.org/web/20230902185655/https://en.everybodywiki.com/100_Most_Highly-Ranked_Films)

## Set Up:
This project is done as a part of IBM Data Engineering Certification Course. It is developed and executed in a Cloud IDE. 

The following libraries are needed for this lab.
1. pandas library for data storage and manipulation. Run the following command in the terminal: python3.11 -m pip install pandas
2. BeautifulSoup library for interpreting the HTML document. Run the following command in the terminal: python3.11 -m pip install bs4
3. requests library to communicate with the web page.
4. sqlite3 for creating the database instance.

## Code:
- The required libraries pandas, requests, BeautifulSoup, and sqlite3 are imported.
- An empty dataframe is created.
- A GET request is sent to the server using the web link. and the response HTML page is stored.
- The text in HTML is parsed using BeautifulSoup.
- The web page is inspected and the html code is analysed to identify the table that has our required information.
- SCraping of the required information is done. Each row is stored into a dictionary which is converted into a temporary dataframe.
- The temporary dataframe is concatenated to the original empty dataframe.
- A counter is maintained to get only 50 records data.
- The data in the dataframe is loaded into a CSV file.
- A connection is established to a dummy database using sqlite3.
- The data in the dataframe is loaded into a table in the database.
- The database connection is closed.

## Acknowledgement
[IBM - Python Project for Data Engineering](https://www.coursera.org/programs/computer-science-comps-alternatives-zphna/learn/python-project-for-data-engineering?authProvider=ttu)

