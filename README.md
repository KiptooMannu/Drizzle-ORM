
# Drizzle ORM
## Learning Objectives

- Modelling data using schemas.
- Using the Drizzle ORM to interact with a database.
- Using the Drizzle ORM to create, read, update, and delete data.
- Using the Drizzle ORM to create relationships between models.
- Using the Drizzle ORM to run migrations.


## Configuring Drizzle with PostgreSQL using node-postgres Driver

1. **Create a package.json**:
   - Run `pnpm init` to create a package.json file.
2. **Install Dependencies** :
   - Run below commands to install the required dependencies.   
``` bash
   pnpm add drizzle-orm pg dotenv
```
3. **Install Dev Dependencies** :
   - Run below commands to install the required  dev-dependencies.
``` bash
   pnpm add -D drizzle-kit  @types/node pg tsx typescript @types/pg 
```

4. **Update the package.json file**:
   - Update the `package.json` file to include the following scripts:
``` json
  "scripts": {
    "dev": "tsx watch ./src/index.ts",
    "start": "node ./dist/index.js",
    "build": "tsc",
    "gen":"drizzle-kit generate",
    "migrate" : " tsx src/drizzle/migrate.ts",
    "studio" : "drizzle-kit studio",
    "push": " drizzle-kit generate && tsx src/drizzle/migrate.ts"

  }
```

## Configuring Drizzle with PostgreSQL using Neon Postgres Driver

1. **Create a package.json**:
   - Run `pnpm init` to create a package.json file.
2. **Install Dependencies** :
   - Run below commands to install the required dependencies.   
``` bash
  pnpm add drizzle-orm @neondatabase/serverless
```
3. **Install Dev Dependencies** :
   - Run below commands to install the required  dev-dependencies.
``` bash
   pnpm add -D drizzle-kit  @types/node tsx typescript 
```
