# Stock Management System
The Stock Management System is a web application built using Spring Boot, Java, Maven, and H2 database. It allows users to manage stocks, perform various operations, and execute custom queries to retrieve specific data.

## Prerequisites
Before running the application, ensure that you have the following installed:

* Java Development Kit (JDK) 8 or higher
* Apache Maven
## Getting Started
1. Clone the repository
2. The application will start on http://localhost:8080.

## Endpoints and Operations
The Stock Management System exposes the following endpoints for performing various operations:

* Retrieve Stocks by Type: GET /stocks/type/{stockType}
* Retrieve stocks of a specific type. Replace {stockType} with the desired stock type.

* Retrieve Stocks Above Price and Lower Date: GET /stocks/abovePrice/price/{price}/lowerDate/date/{date}
* Retrieve stocks above a certain price and lower than a specific date. Replace {price} with the desired price and {date} with the desired date.

* Retrieve Stocks by Market Cap Percentage: GET /stocks/cap/{capPercentage}
* Retrieve stocks based on a specified market cap percentage. Replace {capPercentage} with the desired market cap percentage.

* Create a Stock: POST /stocks/
* Create a new stock by sending a JSON payload containing the stock details.

* Update Stock Market Cap by ID: PUT /stocks/marketCap/{marketCap}/id/{id}
* Update the market cap of a stock by providing the stock ID and the new market cap value.

* Update Stock Type by ID: PUT /stocks/stock/type/id
* Update the type of a stock by providing the stock ID and the new stock type.

* Update Stock by ID: PUT /stocks/stock/{id}
* Update the details of a stock by providing the stock ID and a JSON payload containing the updated stock information.

* Delete Stocks by Owner Count: DELETE /stocks/ownerCount/{count}
* Delete stocks based on the owner count. Replace {count} with the desired owner count.

## Custom Queries and Finders
The Stock Management System includes custom queries and finders to retrieve specific data from the database. These custom queries can be found in the source code of the application. Feel free to explore the codebase to see how these queries are implemented.

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.