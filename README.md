# postgres-world-db

Example Database for [PostgreSQL](https://www.postgresql.org/) : World DB

Database script downloaded at : http://pgfoundry.org/frs/?group_id=1000150&release_id=366#world-world-1.0-title-content

See also PostgreSQL [Sample Databases](https://wiki.postgresql.org/wiki/Sample_Databases).

# Database details

**Important note** : from version 2.0, tables and columns names use _camel case_.
 This version is incompatible with version 1.x.

## Default parameters

- database : world-db
- user : world
- password : world123

## Schema

- public

## Tables
This database contains 3 tables :

- city
- country
- country_language

## Relationships

- country_language -> country (country_language_country_code_fkey)
- country -> city (country_capital_fkey)

# Docker

You can launch this docker image like this :

`docker run -d -pxxxx:5432 ghusta/postgres-world-db:2.1-alpine`

# Alternatives

You can find alternative DBMS or databases examples [at this page](ALTERNATIVES.md).
