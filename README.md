# Just Tech News

A tech news sharing platform where users can post links, comment, and upvote. Built with Express, Sequelize, and MySQL.

## Tech Stack

- Node.js + Express
- Sequelize (MySQL ORM)
- bcrypt for password hashing
- dotenv for environment variables

## Setup

1. Clone the repo and install dependencies:
   ```bash
   npm install

  ##  Create a .env file in the root:
   

    DB_NAME=just_tech_news_db
    DB_USER=your_mysql_user
    DB_PW=your_mysql_password

  ##  Create the database:
    

    mysql -u root -p < db/schema.sql

 ##   Start the server:
    

    npm start

    Server runs on http://localhost:3001

## API Endpoints :

Method	Route	Description
GET	/api/users	Get all users
POST	/api/users	Create a new user
POST	/api/users/login	Login (returns user data)
PUT	/api/users/:id	Update user
DELETE	/api/users/:id	Delete user
GET	/api/posts	Get all posts (with vote/comments count)
POST	/api/posts	Create a post
PUT	/api/posts/upvote	Upvote a post
GET	/api/comments	Get all comments
POST	/api/comments	Add a comment

## Features :

    Secure password hashing (bcrypt)

    User sessions via login endpoint

    Post voting system

    Nested comments with user info

    Database sync defaults to force: false (preserves data)

## Deployment :

Supports JAWSDB MySQL for Heroku or other cloud platforms.
