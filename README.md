
## Database

```bash
brew install postgresql
brew services start postgresql
psql postgres
```

```sql
CREATE ROLE me WITH LOGIN PASSWORD 'password';
ALTER ROLE me CREATEDB;
CREATE DATABASE api;
GRANT ALL PRIVILEGES ON DATABASE api TO me;
```

```bash
psql -d api -U me
```

```sql
CREATE TABLE users (
  ID SERIAL PRIMARY KEY,
  name VARCHAR(30),
  email VARCHAR(30)
);

INSERT INTO users (name, email)
  VALUES ('Jerry', 'jerry@example.com'), ('George', 'george@example.com');
```

## Installation

```bash

npm install
node index.js
```






# node_postgre_backend
# node_postgre_backend
