Assignment: Testing the Cryptocurrency API

## Objective
The objective of this test assignment is to evaluate the functionality and correctness of the REST API that you have developed in the "Building a Cryptocurrency API" assignment.

## Requirements
You are required to perform a series of tests on the all the three layers (Controller, Service and Repository) of the API to ensure it meets the specified requirements.

1. **Testing Cryptocurrency Data Retrieval**
   - Send a GET request to the `/api/cryptocurrencies` endpoint.
   - Verify that the response contains a list of cryptocurrencies from the Twelve Data API.
   - Check if the response status code is 200 (OK).

2. **Testing Wishlist Operations**
   - Add a new cryptocurrency to the Wishlist by sending a POST request to the `/api/wishlist` endpoint with valid data.
   - Retrieve the added cryptocurrency from the Wishlist by sending a GET request to the `/api/wishlist/{id}` endpoint, replacing `{id}` with the ID of the added cryptocurrency.
   - Verify that the retrieved cryptocurrency matches the data you added.
   - Update the cryptocurrency in the Wishlist by sending a PUT request to the `/api/wishlist/{id}` endpoint, replacing `{id}` with the ID of the added cryptocurrency.
   - Retrieve the updated cryptocurrency and confirm that it reflects the changes made during the update.
   - Delete the cryptocurrency from the Wishlist by sending a DELETE request to the `/api/wishlist{id}` endpoint, replacing `{id}` with the ID of the added cryptocurrency.
   - Verify that the cryptocurrency has been removed from the Wishlist.

3. **Testing Validation and Error Handling**
   - Attempt to add a duplicate cryptocurrency to the Wishlist and verify that it returns an appropriate error response.
   - Send invalid requests to endpoints (e.g., missing required fields, incorrect data format) and ensure that the API handles these cases with meaningful error responses.

