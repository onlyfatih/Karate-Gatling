# RESTful Booker API Test and Performance Project

This project aims to test RESTful APIs obtained from the Restful Booker site using the Karate framework. Additionally, it includes performance testing using Gatling integration.

<p align="center">
  <img src="https://gatling.io/wp-content/uploads/2021/06/gatling-og.jpg" width="300" />
</p>

## Project Overview

This project combines the usage of Karate framework for API testing and Gatling for performance testing against the Restful Booker APIs.

## Project Structure

The project structure is organized as follows:

    caller: Contains Karate scenarios making API requests.
    features: Holds Karate scenarios, each representing a specific API request.
    performance: Includes Gatling scenarios for performance testing.

## How to Run?
## API Tests

To run the API tests, follow these steps:

1. Open a terminal in the project directory.
2. Run the following command to execute Karate tests:
   ```
   mvn test
   ```

## Performance Tests

To run performance tests with Gatling, follow these steps:

1- Open a terminal in the project directory.
2- Run the following command to execute Gatling tests:
   ```
   mvn clean test-compile gatling:test
   ```

## Important Files and Functions

    createBookingCaller.feature: Contains the scenario for creating a new booking.
    getBooking.feature: Includes the scenario for querying an existing booking.
    deleteBooking.feature: Holds the scenario for deleting a booking.
    UserSimulation.scala: Contains the Gatling scenario defining the performance tests.

## Environment Configuration and Variables

Environment settings and variables are configured using the fn() function through the Karate framework. This function handles defining the environment where the scenarios run and setting up necessary variables.

## Contributions

This project is open to contributions. Feel free to contribute your enhancements or report issues by opening a pull request or issue.
