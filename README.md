# Payment Service

The **Payment Service** is a microservice responsible for processing payments for orders placed in a restaurant. It handles payment transactions, simulates interactions with external payment providers (e.g., Stripe or PayPal), and maintains a record of all payment activities. This service is built using **Python** with the **Flask** framework for simplicity and flexibility.

---

## Key Features

- **Payment Processing**:
  - Process payments for orders via a RESTful API.
  - Simulate transactions with an external payment provider (e.g., Stripe or a mock payment gateway).

- **Payment History**:
  - Store and retrieve payment records for auditing and reference.

- **Resilience**:
  - Implement a **Circuit Breaker** pattern to handle failures when communicating with external payment providers.

---

## Tech Stack

- **Language**: Python
- **Framework**: [Flask](https://flask.palletsprojects.com/) (Lightweight web framework)
- **Database**: SQLite for storing payment history.
- **Circuit Breaker**: Implemented using `pybreaker` to handle failures gracefully.

---

## Endpoints

### REST API

- `POST /payments`: Process a new payment.
- `GET /payments/:id`: Retrieve the status of a specific payment.

---

## Tools & Libraries

- **Flask**: Lightweight and easy-to-use web framework for building the API.
- **SQLite**: Simple database for storing payment records.
- **pybreaker**: Library for implementing the Circuit Breaker pattern.
- **Requests**: For simulating interactions with external payment providers.

---

![image](https://github.com/user-attachments/assets/4e68edaa-a71a-46c1-bf5f-ca8a482f1106)
