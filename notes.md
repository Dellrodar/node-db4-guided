# Data Normalization: The process of designing our database schema in a way that prevents redundancies

## Denormalized Data

```javascript
const farm = {
 id: 1,
 name: "Lon Lon Ranch"
 animals: [ Horse, Chicken, Cows ]
 }
```

## Guidelines

- No field values are repeated
- There are no redundant records
- Each record should always have a unique primary key
- All fields in a table should relate to the PK in some way

## Relationship Types

- One to One
  - Table A can link to a single row in Table B and vice versa
- One to Many
  - Table A can link to many rows in Table B, but Table B can only link to a single row in Table A
- Many to Many
  - Table A can link to many rows in Table B and Table B can link to many rows in Table A
  - Intermediary/join tables are usually required
