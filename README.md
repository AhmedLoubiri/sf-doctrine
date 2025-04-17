# Symfony Intro
### This repo contains basic intro to doctrine (creating database, entity and migrations).
after cloning the repo:
```bash
  cd sf-doctrine
  composer install
```
### creating database:
#### 1. Go to the .env file and search for DATABASE_URL
#### 2. Choose the convenient DBMS (for my case MYSQL)
#### 3. Choose the name of the database, and put the wanted credentials
#### 4. run this command:

```bash
  symfony console doctrine:database:create
```
### creating entity:
#### 5. Create An Entity by this command:

```bash
  symfony console make:entity
```
### creating migration:
#### 6. Create migration by this command:

```bash
  symfony console make:migration
```
### Note: verify the version of MYSQL in the DATABASE_URL.

used dependencies:
when creating the project:
```bash
   symfony new $PROJECT_NAME --version="6.4.*" --webapp
```
### --webapp to create a traditional web application.
```bash
  php bin/console doctrine:fixtures:load
```
