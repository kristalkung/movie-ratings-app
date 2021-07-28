# Movie Ratings App

A flask application for viewing movie information and adding ratings to movies.

## Table of Contents

- [Technologies Used](https://github.com/kristalkung/movie-ratings-app#technologies-used)
- [How to Run Movie Ratings App Locally](https://github.com/kristalkung/movie-ratings-app#how-to-run-locally)
- [Features](https://github.com/kristalkung/movie-ratings-app#features)
- [Future Implementations](https://github.com/kristalkung/movie-ratings-app#future-implementations)

## Technologies Used

Python, Flask, SQLAlchemy, PostgreSQL, HTML, Jinja, MovieLens 100K dataset

## How to Run Movie Ratings App Locally

- Clone this repository
- Create a new virtual environment
- In your virtual environment, install the requirements using: ```pip3 install -r requirements.txt```
- Add env to .gitignore
- Seed the database by typing this into the terminal: ```python3.8 seed_database.py```
- Load the website using: ```python3.8 server.py```
- On the browser, search [localhost:5000/](localhost:5000/)

## Features

### Search for movie

On the homepage, click "View all movies". Users will then be taken to a page that will list all
movies listed in the MovieLens 100K dataset. Click on the title of the movie to be taken to a page with additional movie information.

### Users may sign up for an account and log in

New uses may create an account using a unique email. If a new user inputs an email that is already used for an existing account, they will be prompted to use a different email. After signing up, the user will be added to the database and redirected to the login page. On the server side, the login inputs will be checked if the input email exists in the database, and if so, the input password is compared to the password associated with the email. After logging in, a session key for user and user name will be added to the server. From that point on, the user will be able to access their profile and save recalls to their profile.

<!-- ### Users may rate movies -->

## Future Implementations

### Add function to allow users to rate movies on the front end

The data model already includes a ratings table, which connects the users and movies tables.

### Add more to the user profile

This could list out the movie ratings given by a user on their profile.