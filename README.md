# Mombar-NYC-Checkout-Project

- [Mombar-NYC-Checkout-Project](#mombar-nyc-checkout-project)
  * [Description](#description)
  * [Requirements](#requirements)
  * [Installation](#installation)
  * [Usage](#usage)
    + [Updating the Menu](#updating-the-menu)

## Description
A menu and checkout project for the NYC restaurant Mombar. This project was created for the popular restaurant Mombar located at 25-22 Steinway street Astoria New York. It contains the full menu and images for each item, with a functional login and checkout system.

## Requirements
- A web browser (Chrome, Edge, or another Chromium-based browser is recommended).

## Installation
To run the project locally, follow these steps:
1. Download the code from [GitHub](https://github.com/your-username/Mombar-NYC-Checkout-Project).
2. Unzip the folder named "Completed Project".
3. Open the `registration.html` page inside the "Completed Project" folder using your preferred web browser (Chrome, Edge, or another Chromium-based browser is recommended).
Note: You do not need to use the `registration.html` page as it should redirect you to the login page regardless of what page you access when you are not logged in.

## Usage
This project allows users to view the menu of the NYC restaurant Mombar, add items to their cart, and checkout. It was designed as a proof of concept for a web development class 385 as the final project. It includes the entire menu with images and a description for each item. The items are automatically populated from a user-created list inside of `/js/catalog.js`. To update the menu, edit the file `Catalog.js` and add a new item, description, and image. For example, if you add a steak item to the catalog with the image "Steak.png" and the description "A nice tasty steak", it will automatically appear on the `menu.html` page and look like all the other menu options without you having to change the `menu.html` file at all. When you click on the image or name of the steak on `menu.html`, you will be redirected to the `solopage.html` page, which will automatically be populated with the information and image of the item you clicked on. The JavaScript will automatically populate the new menu item inside of the menu list, giving it the proper CSS and its own item box with add-to-cart functionality and checkout functionality inside of 'menu.html'. The project can also dynamically create a dedicated page for any item inside of `catalog.js`. This benefits the user because they do not have to make an individual page for each item, as the `solopage.html` creates the page dynamically.

### Updating the Menu

To update the menu, you will need to modify the `catalog.js` file. Here is a step-by-step guide:

1. Open the `catalog.js` file in your preferred text editor.

2. Inside the `catalog.js` file, you will see a list of products, each product is represented as an object with properties like `id`, `name`, `code`, `image`, `description`, and `price`. Here is an example:

    ```javascript
    {
        id:1,
        name:"Mombar - Appetizer", 
        code:"mombara", 
        image:"mombara.jpg",
        description:"Experience a delightful blend of traditional flavors with our Mombar appetizer. Hand-stuffed sausages filled with rice, succulent beef, tender lamb, aromatic herbs, and a selection of finely ground spices. Sautéed to perfection with garlic, chickpeas, and tomatoes for an unforgettable taste experience.",
        price:13.00
    },
    ```
3. To add a new item to the menu, simply create a new object at the end of the list. Make sure to increment the `id` for the new item and provide a unique `code`:

    ```javascript
    {
        id:21, 
        name:"New Dish", 
        code:"newdish", 
        image:"newdish.jpg", 
        description:"This is a new dish description.",
        price:20.00
    }
    ```
4. Save the `catalog.js` file once you have added the new item.

The JavaScript code in the project will automatically populate the new menu item inside of the menu list, giving it the proper CSS and its own item box with add-to-cart functionality and checkout functionality inside of 'menu.html'. The project can also dynamically create a dedicated page for any item inside of `catalog.js`. This benefits the user because they do not have to make an individual page for each item, as the `solopage.html` creates the page dynamically.
