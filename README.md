# Monolith Application
A express js back-end and front-end application in one repository. The domain subject for this application is a simple CRUD Contacts application with a sqlite3 database to store the contacts in a table.

## Setup
- fork and clone this repository `git clone <repository name>`
- change directory in to the project `cd <repository name>`
- run `npm install`
- run `npm run dev`
- copy the `.env.sample` file to `.env`. `cp .env.sample .env` and change the variables in the `.env` file to suite your needs.

## Technology Stack
### Dependencies
- nodejs (the v8 engine implementation)
- ExpressJS (API Server)
- sqlite3 (Database)
- Sequelize (ORM)
- BodyParser (deal with Json)
- cors (cross site origin requests)
### Dev Dependencies
- nodemon (auto restarting of server on file changes)

## API
### Endpoints
- **/contacts** (POST) **Creates a new contact**
- **/contacts** (GET) **Get all contacts**
- **/contacts/:id** (GET) **Get a single contact by its `id`**
- **/contacts/:id** (PUT) **Update a contact by its `id`**
- **/contacts/:id** (DELETE) **Deletes a contact by its `id`**

## Models
- **Contact**
    - id: INTEGER, AutoIncrement, PrimaryKey
    - name: STRING, Required
    - email: STRING, Require, unique
    - address: STRING, Required

