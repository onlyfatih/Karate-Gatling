# API & Performance Testing with Karate + Gatling

A combined API functional and performance testing project built against the public **Restful Booker** API.

The repository demonstrates how reusable Karate API scenarios can be exercised both as functional tests and as part of **Gatling load simulations**.

## Tech Stack

- Karate
- Gatling
- Scala
- Maven
- JUnit 5

## Project Goals

- Validate REST API behavior with Karate
- Reuse API flows inside performance simulations
- Execute load scenarios with Gatling
- Keep functional and performance test assets close to each other
- Generate repeatable Maven-based test runs

## Structure

```text
src/test/java
├── caller         # Reusable API flows
├── features       # Functional Karate scenarios
└── performance    # Gatling simulations
```

Representative flows include booking creation, retrieval and deletion, while the performance layer drives those API interactions under generated load.

## Run Functional API Tests

```bash
mvn test
```

## Run Performance Tests

```bash
mvn clean test-compile gatling:test
```

## Performance Engineering Perspective

Performance testing is not only about generating requests. The useful output comes from analyzing how a service behaves as load increases: throughput, response-time distribution, error rate and the point at which the system begins to saturate.

This project serves as a compact example of integrating an API test DSL with a dedicated load-generation tool.

## What This Project Demonstrates

- API functional testing with Karate
- Gatling-based performance testing
- Scenario reuse between functional and load tests
- Maven-driven execution
- Separation of functional scenarios and performance simulations

---

**Focus:** API Testing • Performance Testing • Gatling • Karate • Load Simulation
