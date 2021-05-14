<h1 align = "center"> E-Commerce <br> Back End Application </h1>
<p align = "center">
  <img src="https://img.shields.io/npm/v/npm?color=red&logo=npm"/>
  <img src="https://img.shields.io/node/v/jest"/>
  <img src="https://img.shields.io/github/license/kemaldemirgil/buy-m3?color=cyan&label=License&logo=github&logoColor=cyan"/>
  <img src="https://img.shields.io/github/issues/kemaldemirgil/buy-m3?color=yellow&label=Issues&logo=github&logoColor=yellow">
  <img src="https://img.shields.io/github/last-commit/kemaldemirgil/buy-m3?color=orange&label=Last%20Commit&logo=git&logoColor=orange">
</p>

## About:
This API was created to perform CRUD operations on the simple elements that can occur on a standard `E-Commerce` project. This application has *Products*, *Tags* and *Categories* that interact with each other depending on the request.\
Since the main focus was creating the API for this project, there is no front-end that allows the user to interact with it so, I've used `Postman` during testing and `Insomnia` for the demonstration.\
This API uses `Express.js` to run the server and `Sequelize` to interact with the `MySQL` database.

## Notes:
This was my first time creating a fully interactive back-end using `MySQL`. `Sequelize` makes it so much easier to interact with the database while keeping the code clean. I've noticed that once the API handles with PUT requests, it's best for the user to be inputting specifically the required fields otherwise, things can get messy and the user might come across with errors. Handling the errors and giving back descriptive messages is also very helpful on troubleshooting and for the user experience.\
I used `async` & `await` while coding the **routes**, I also used `try...catch` for the first time. It definitely shortens the code while getting rid of *call-back hell*.

## Installation & Dependencies:
1. Please clone this repo to your PC.
    Download ZIP
    :-------------------------:
    ![](/assets/clone.gif)

  - Alternatively, simply in the terminal;
    ```bash
    git clone https://github.com/kemaldemirgil/buy-m3
    ```
2. Once it's located in your PC, before adding anything yet, please create the database from the `MySQL` shell. The schema is located in `db/schema.sql`.
     Create Database
    :-------------------------:
    ![](/assets/schema.gif)
  - Alternatively, copy the following:
    ```mysql
    -- DROP DATABASE
    DROP DATABASE IF EXISTS ecommerce_db;

    -- CREATE DATABASE
    CREATE DATABASE ecommerce_db;
    ```
3. After creating the database, please create a `.env` file to store your username, password and the database name using the following:
    ```bash
    DB_USER=
    DB_PW=
    DB_NAME=ecommerce_db
    ```
     Seed Database
    :-------------------------:
    ![](/assets/env.gif)
4. After creating the `.env` file, please seed the database by opening the terminal in the parent directory by running;
    ```bash
    npm run seed
    ```
     Seed Database
    :-------------------------:
    ![](/assets/seed.gif)
5. Next, please install the dependencies by running the terminal in the parent directory.\
    \
    ![](/assets/depen.PNG)
    ```bash
    npm i
    ```
     Install Dependencies
    :-------------------------:
    ![](/assets/depen.gif)
6. Finally, to start the application, please run the following on the main file:
    ```bash
    npm start
    ```
    Alternatively, to run it using `nodemon`,
    ```bash
    npm run watch
    ```



## Usage & Demo:

CRUD on Categories
:-------------------------:
![](/assets/category.gif)

CRUD on Tags
:-------------------------:
![](/assets/tag.gif)  

CRUD on Products
:-------------------------:
![](/assets/product.gif)  

## Improvements:

> Please contact me for any contributions or any input about this application, I would love to get some feedback!

<h3 align = "center">Connect with me!</h3>
<p align="center">
  <a href="https://www.linkedin.com/in/kemaldemirgil/" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=plastic&logo=linkedin&logoColor=white"/></a>
  <a href="mailto: kemal.demirgil@hotmail.com" target="_blank"><img src="https://img.shields.io/badge/Gmail-D14836?style=plastic&logo=gmail&logoColor=white"/></a>
</p>

## License:
Copyright © Kemal Demirgil. All rights reserved.
Licensed under the [MIT](https://github.com/kemaldemirgil/buy-m3/blob/main/LICENSE) license.
