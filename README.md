## Akka Cassandra Demo

### Available Routes

#### Adding a new bank account

```shell
curl -v -X POST http://localhost:8080/bank-accounts\
   -H 'Content-Type: application/json'\
   -d '{"user":"rcardin", "currency":"EUR", "balance": 1000.0}'
```

#### Updating the balance of a bank account

```shell
curl -v -X PUT http://localhost:8080/bank-accounts/5e36bcd7-dd7d-43d6-90f0-de08cd9f551d\
   -H 'Content-Type: application/json'\
   -d '{"currency":"EUR", "amount": 500.0}'
```

#### Retrieving the details of a bank account

```shell
curl -v http://localhost:8080/bank-accounts/ce1f4ac3-f1be-4523-b323-25e81d90322f
```