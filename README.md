# SQL Base Project

This Java application is a simple **Product Management System** built with **Swing** for the graphical user interface and **MySQL** for the database backend. The application allows users to perform **CRUD operations** (Create, Read, Update, Delete) on products, with functionalities such as viewing, adding, updating, and searching for products in the database.

### Key Components:
1. **GUI (Swing)**: 
   - The user interface consists of text fields for product information such as ID, Name, Quantity, and a dropdown for the Category.
   - A search bar allows users to find products by ID.
   - A table (`JTable`) displays product data retrieved from the database.

2. **MySQL Database Interaction**:
   - **Connection**: The application connects to a local MySQL database (`mydb`) using JDBC. It retrieves and displays product data from the `product` table.
   - The application interacts with the database through `PreparedStatement` objects to execute SQL queries securely.

3. **Core Functionalities**:
   - **Viewing Products**: The `tableValues()` method fetches all products from the `product` table and displays them in the `JTable`.
   - **Adding a Product**: Users can add a new product by entering the required details and clicking the "ADD" button. This inserts a new product into the database using the following query:
   - **Searching for a Product**: The application provides a search bar where users can enter a product ID to filter the table based on that ID:
   - **Updating a Product**: Users can update the product information by selecting a product from the table, modifying the details, and clicking the "Update" button:
   - **Deleting a Product**: When a product is selected from the table, the user can delete it by confirming a dialog prompt:

### Usage:
- **Add a Product**: Fill in the product details and click "ADD" to insert the product into the database.
- **Search for a Product**: Enter a product ID in the search bar to retrieve and display the corresponding product.
- **Update a Product**: Modify the displayed product details and click "Update" to save changes to the database.
- **Delete a Product**: Select a product from the table, confirm the deletion, and it will be removed from the database.

This system provides a straightforward solution for managing product inventories using a graphical interface connected to a MySQL database.
