# PizzaMaker

## Overview

PizzaMaker is a web application that allows users to customize and order pizzas seamlessly. The frontend is built using Angular, while the backend leverages .NET, specifically C# and PostgreSQL for data storage. This README provides a concise guide on setting up and using the application.

## Features

- **Create Your Own Pizza:**
  - Customize your pizza by selecting ingredients such as extra cheese, pepperoni, mushrooms, etc.
  - Choose the size of your pizza (small, medium, or large).
- **Menu Options:**

  - Select from a pre-defined menu of delicious pizzas, including:
    - Margherita
    - Quattro Formaggi
    - Bacon Lovers
    - Veggie Delight
    - Hawaiian

- **Checkout:**

  - View the selected pizza and its price before checkout.

- **Delivery Information:**

  - Specify the delivery location for your order.
  - Previous orders are saved for each user.

- **User Authentication:**
  - Register with a unique username, password, and email.
  - Login securely to access the application.

## Project Structure

- **PizzaApp:**

  - The main project file, containing the solution (PizzaApp.sln).

- **PizzaApp.DataAccess:**

  - Manages the database using DBContext, repositories, and migrations.

- **PizzaApp.Domain:**

  - Defines entities such as Order, Pizza, and User.
  - Includes enums for ingredients.

- **PizzaApp.Dtos:**

  - Data transfer objects for Order, Pizza, and User.

- **PizzaApp.Helpers:**

  - Contains reusable code, including DIContainer and Extensions.

- **PizzaApp.Mappers:**

  - Utilizes AutoMapper for mapping configurations.

- **PizzaApp.Services:**

  - Centralized location for application logic, abstractions, implementations, and UserServices.

- **PizzaApp.Shared:**
  - Houses custom exceptions, requests, responses, and settings.

## Getting Started

### Client (Frontend)

1. Open the `client` folder in Visual Studio Code.
2. Open the terminal and run `npm install` to install required packages.
3. Start the project with `npm start`.
4. Open the provided localhost link in your browser by holding Ctrl and clicking.

### Server (Backend)

1. Open the `Server` folder and navigate to `PizzaApp`.
2. Open `PizzaApp.sln` in Visual Studio.
3. In Visual Studio, go to `Tools` > `NuGet Package Manager` > `Package Manager Console`.
4. Select the default project (`PizzaApp.DataAccess`) in the Package Manager Console.
5. Run the command `add-migration [name]` to name the migration.
6. Run the command `update-database` to apply the migration and update the database.

## Usage

1. Register or log in to access the application.
2. Customize your pizza or choose from the menu.
3. Proceed to checkout, review your order, and specify the delivery location.
4. Enjoy your delicious pizza!

## Contributors

- Martin Stamenkovski

## License

This project is licensed under the [MIT License](LICENSE).
