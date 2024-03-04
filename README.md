# Dive Deeper

<img src="static/images/otter2.gif" width="100" height="120">

## Web Application Exercise

A little exercise to build a web application following an agile development process. See the [instructions](instructions.md) for more detail.

## Product vision statement

A web app card game that fosters deeper connections with others through question prompts.

## User stories

* As a player, I can log in.
* As a player, I can sign up.
* As a not-logged-in player, I can play with sample decks.
* As a logged-in player, I can play with sample decks and my personal decks.
* As a logged-in player, I can create a new deck.
* As a logged-in player, I can edit an existing deck.
* As a logged-in player, I can delete an existing deck.
* As a logged-in player, I can search for an existing deck.
* As a logged-in player, I can log out.

[Issues Page](https://github.com/software-students-spring2024/2-web-app-exercise-gas2/issues)

## Task boards

[Sprint 1 Task Board](https://github.com/orgs/software-students-spring2024/projects/4) <br>
[Sprint 2 Task Board](https://github.com/orgs/software-students-spring2024/projects/22/)

## Design

[Wireframe](https://www.figma.com/file/MtmBlXWq7G9Axki5tmboSd/Project-2?type=design&node-id=0%3A1&mode=design&t=mF8G6yOHcrtvsROr-1)

## Set Up

1. Download the source code from the repository
    ```
    git clone https://github.com/software-students-spring2024/2-web-app-exercise-gas2.git
    ```

2. Install pipenv using pip or pip3
    ```
    pip install pipenv
    ```
    or 
    ```
    pip3 install pipenv
    ```

3. Activate the virtual environment
    ```
    pipenv shell
    ```

4. Install the dependencies
    ```
    pipenv install
    ```

5. Create a file called `.env`. Populate it with the following:
    ```
    MONGO_DBNAME=gas
    MONGO_URI=mongodb+srv://<username>:<password>@gas.xhjamgl.mongodb.net/?retryWrites=true&w=majority&appName=gas
    SECRET_KEY=<key>
    ```
    To run it locally using Dive Deeper's database via MongoDB Atlas, you need to replace  `<username>`, `<password>`, and `<key>` with the right information. Please contact the authors for this information.

    Note: using your own database

    Alternatively, you can create your own database. Replace the `MONGO_URI` string with the connection string generated by MongoDB. Replace `MONGO_DBNAME` with the name of your database, and replace `<username>` and `<password>` with the credentials used to generate the database. Also replace `<key>` with a secret key of your choosing. Furthermore, make sure to create a collection named `users` and another collection named `decks`.

6. Finally run the app
    ```
    flask run
    ```