# Express.js API with Sequelize PostgreSQL
This repository contains a functional Express.js API that utilizes Sequelize to connect to a PostgreSQL database.

## Setup
1. Clone this repository to your local machine:

git clone <repository-url>
2. Install dependencies:

npm install
3: Create an environment variable file (.env) in the root directory of the project and add the following variables:

DB_NAME=your_database_name
DB_USERNAME=your_postgresql_username
DB_PASSWORD=your_postgresql_password

## Database Setup
1. Enter the following commands to create the development database schema and seed it with test data:
npx sequelize-cli db:create
npx sequelize-cli db:migrate
npx sequelize-cli db:seed:all

## Running the Application
To start the server and sync Sequelize models to the PostgreSQL database, run:

npm start

## API Routes
### GET Routes
Categories: /api/categories
Products: /api/products
Tags: /api/tags

When you open these routes in a tool like Insomnia, you'll receive formatted JSON data for each route.

## POST, PUT, and DELETE Routes
You can test these routes in Insomnia to:

Create new data.
Update existing data.
Delete data from the database.

## Notes
Ensure you have PostgreSQL installed and running on your machine.
Make sure to replace your_database_name, your_postgresql_username, and your_postgresql_password with your actual database credentials in the .env file.
Feel free to explore and modify the code according to your needs!