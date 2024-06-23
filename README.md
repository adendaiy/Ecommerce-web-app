# Ecommerce web app

This project is a simple web application that manages a list of products, allowing for CRUD (Create, Read, Update, Delete) operations. The products are persisted in a db.json file.

## Features

- *View Products:* Display a list of products with details like name, description, price, and image.
- *Add Product:* Add new products via a form.
- *Edit Product:* Edit details of existing products.
- *Delete Product:* Remove products from the list.
- *Persistence:* Changes are saved to db.json to persist data between sessions.

## Installation

1. *Clone the repository:*
   ```bash
   git clone https://github.com/your-username/product-management-app.git
   cd product-management-app
Set up a local server:

You can use a simple server like http-server or any server of your choice.
If you have Node.js installed, you can install http-server:
bash
Copy code
npm install -g http-server
Start the server in the project directory:
bash
Copy code
http-server
Access the app:

Open your browser and navigate to the local server URL, typically http://localhost:8080.
Usage
Viewing Products
The products will be displayed in a card format for general users.
Admins will see an additional list with options to edit or delete products.
Adding a Product
Fill out the form with the product's name, description, price, image URL, and type.
Click the "Add Product" button to add the product to the list and persist it to db.json.
Editing a Product
Click the "Edit" button next to the product you want to edit.
Update the product details in the prompt dialogs.
The product list will refresh to show the updated details.
Deleting a Product
Click the "Delete" button next to the product you want to remove.
The product will be removed from the list and db.json will be updated.
Code Overview
JavaScript
Initialization and Event Listeners: The script waits for the DOM to load before initializing the products array and setting up event listeners.
Fetching Data: Retrieves initial product data from db.json using the Fetch API.
Rendering Products: Dynamically generates HTML to display products in the UI.
Adding Products: Handles form submissions to add new products to the list and persist them.
Editing Products: Provides functionality to edit product details.
Deleting Products: Allows for the removal of products from the list and updates the persistence layer.
Functions
renderProducts(): Renders the list of products in the UI.
deleteProduct(id): Removes a product by its ID.
editProduct(id): Edits product details based on user input.
persistProducts(products): Persists the current state of the product list to db.json.
Notes
This is a simple project for demonstration purposes. In a production environment, consider using a more robust method for generating unique IDs and handling data persistence.
Ensure you have appropriate error handling for the fetch requests and other potential issues.
License
This project is licensed under the MIT License - see the LICENSE file for details.

css
Copy code

This README.md file provides a comprehensive overview of the project, including its features, installation steps, usage instructions, and a brief explanation of the code structure. Adjust the content as necessary to fit your specific use case or preferences.