# IT22178190-SE4010-Labsheet05

Microservices lab project with:
- API Gateway (`8080`)
- Item Service
- Order Service
- Payment Service

## Run the project

```bash
docker compose up -d --build
```

Base URL (through gateway):

```text
http://localhost:8080
```

## Required API Endpoints (9)

All endpoints below are accessed through the API Gateway on port `8080`.

| Method | Endpoint | Service | Description |
|---|---|---|---|
| GET | `/items` | Item | Returns list of all items |
| POST | `/items` | Item | Create a new item |
| GET | `/items/{id}` | Item | Get item by ID |
| GET | `/orders` | Order | Returns all orders |
| POST | `/orders` | Order | Place a new order |
| GET | `/orders/{id}` | Order | Get order by ID |
| GET | `/payments` | Payment | Returns all payments |
| POST | `/payments/process` | Payment | Process a payment |
| GET | `/payments/{id}` | Payment | Get payment status |

