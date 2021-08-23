# dbee-github-source

This template allows you to use Github as migration source for dbee.

## Adding new schemas

If you want to manage multiple schemas using dbee, you need to create a
folder under `migrations` with the schema name. To specify the connection \
details you must provide the following env variables.

:warning: Note that currently only MySQL is supported as database.

`schema` is the same name as provided in your folder structure (no need to uppercase).

```
DB_USERNAME_{SCHEMA}=root
DB_USERNAME_{SCHEMA}=safeP@ssw0rd!
DB_HOST_{SCHEMA}=localhost
DB_PORT_{SCHEMA}=3306
DB_NAME_{SCHEMA}=myDatabaseName

## Example for production DB

# DB_USERNAME_PRODUCTION=root
# DB_USERNAME_PRODUCTION=safeP@ssw0rd!
# DB_HOST_PRODUCTION=localhost
# DB_PORT_PRODUCTION=3306
# DB_NAME_PRODUCTION=myDatabaseName
```
