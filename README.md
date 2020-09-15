# Awesome Project Build with TypeORM

Steps to run this project:

1. Run `npm i` command
2. Setup database settings inside `ormconfig.json` file

> Set your data (your_user,your_pass,your_database)

```js
{
  "type": "mysql",
  "host": "localhost",
  "port": 3306,
  "username": "your_user",
  "password": "your_pass",
  "database": "your_database",
  "synchronize": true,
  "logging": false,
  "entities": ["src/entity/**/*.ts"],
  "migrations": ["src/migration/**/*.ts"],
  "subscribers": ["src/subscriber/**/*.ts"],
  "cli": {
    "entitiesDir": "src/entity",
    "migrationsDir": "src/migration",
    "subscribersDir": "src/subscriber"
  }
}
```

3. Run `npm start` command
