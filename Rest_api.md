# Assignment: Building a Cryptocurrency API with Spring Boot/.NET webapi

## Objective
The goal of this assignment is to build a RESTful API using Spring Boot/.Net webapi that fetches cryptocurrency data from an external API and provides endpoints for adding currencies to a Wishlist, which will be stored in an H2/MSSQL database.

[CLICK HERE FOR API DOCUMENTATION](https://twelvedata.com/docs#getting-started)

## Requirements
1. **Set up a Spring Boot project**
   - Create a new Spring Boot project/.NET web api project

2. **Create a RESTful endpoint for fetching cryptocurrency data**
   - Use the [Twelve Data API](https://api.twelvedata.com/cryptocurrencies) to fetch cryptocurrency data.
   - Implement a REST endpoint, e.g., `/api/cryptocurrencies`, to retrieve a list of cryptocurrencies from the Twelve Data API.

3. **Create a Wishlist feature**
   - Implement a Wishlist feature to allow users to add cryptocurrencies they are interested in.
   - Create a data model for a currency, including attributes you find relevant from api
   - Implement a REST endpoint for adding currencies to the Wishlist, e.g., `/api/wishlist`.
   - Store the added currencies in the H2 database.
   - Ensure that the Wishlist supports CRUD (Create, Read, Update, Delete) operations.

4. **Implement validation and error handling**
   - Ensure proper input validation, such as checking for duplicate currencies in the Wishlist.
   - Implement error handling to return meaningful error responses in case of invalid inputs or other errors.
