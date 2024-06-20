<div align="center">
    <h1>Grocery Store 🛒</h1>
    <a href="https://twitter.com/WeatherfulBot">
        <img alt="Status" src="https://img.shields.io/badge/Status-Complete-brightgreen">
    </a>
    <img alt="C++ Version" src="https://img.shields.io/badge/C++-20%2B-blue">
    <a href="https://opensource.org/licenses/MIT">
        <img alt="License" src="https://img.shields.io/badge/License-MIT-blue.svg">
    </a>
</div>

## Table of Contents

1. [Overview](#-overview)
2. [Features and Demo](#features-and-demo)
3. [License](#-license)

## 🌟 Overview

**Grocery Store** is a C++ project that simulates the functionality a user would experience at a grocery store. This includes adding items to their cart, pricing items, assigning unique UPC codes for each item, product names, and more. The system is designed using object-oriented principles such as polymorphism, abstraction, and encapsulation.

## **Features and Demo**

### Feature 1: Adding Items to Cart

- **Description**: Users can add items to their cart, each with a unique UPC code, product name, brand name, and price.

  - **Code Example**:
    ```cpp
    GroceryList myList;
    myList.insert(GroceryItem("milk", "Brand A", "000000000001", 2.99), GroceryList::Position::TOP);
    myList.insert(GroceryItem("bread", "Brand B", "000000000002", 1.99), GroceryList::Position::BOTTOM);
    ```

### Feature 2: Pricing of Items

- **Description**: Each item in the grocery store has a price, and users can view the total price of the items in their cart.

  - **Code Example**:
    ```cpp
    double totalPrice = myList.calculateTotalPrice();
    std::cout << "Total Price: $" << totalPrice << std::endl;
    ```

### Feature 3: Unique UPC Codes

- **Description**: Each item is assigned a unique UPC code for identification.

  - **Code Example**:
    ```cpp
    GroceryItem item("eggs", "Brand C", "000000000003", 3.49);
    std::cout << "UPC Code: " << item.upcCode() << std::endl;
    ```

### Feature 4: Viewing and Modifying Cart

- **Description**: Users can view the items in their cart, remove items, and modify the cart as needed.

  - **Code Example**:
    ```cpp
    myList.remove(GroceryItem("bread", "Brand B", "000000000002", 1.99));
    std::cout << "Updated Cart: " << myList << std::endl;
    ```

## 📄 License

This project is licensed under the GNU General Public License v3 - see [LICENSE.md](LICENSE.md) for details.
