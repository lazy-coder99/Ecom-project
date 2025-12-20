# Ironade E-commerce Project

This repository contains the source code for Ironade, a front-end e-commerce website for an iron products store. The project is built using HTML, CSS, and vanilla JavaScript, leveraging modern JavaScript features like ES6 modules. The application provides a complete shopping experience, from browsing products to managing a shopping cart.

## Features

*   **Product Catalog:** Products are dynamically loaded from a local `products.json` file and displayed on the homepage and products page.
*   **Shopping Cart:**
    *   **Add to Cart:** Users can add products to their shopping cart.
    *   **Cart Management:** A dedicated cart page allows users to view, update quantities (increment/decrement), and remove items.
    *   **Persistent Cart:** The shopping cart state is saved in the browser's `localStorage`, so items remain even after refreshing the page.
    *   **Dynamic Cart Icon:** The cart icon in the navigation bar updates in real-time to show the number of unique items in the cart.
*   **Dynamic UI Updates:**
    *   The cart total, sub-total, and tax are automatically calculated and updated on the cart page.
    *   User feedback is provided through toast notifications for actions like adding or removing items from the cart.
*   **Responsive Design:** The website is designed to be responsive and functional across various screen sizes, from mobile devices to desktops.
*   **Modular Codebase:** The JavaScript code is organized into modules, each responsible for a specific feature (e.g., cart operations, product display, utility functions).

## Tech Stack

*   **Frontend:** HTML5, CSS3, Vanilla JavaScript (ES6 Modules)
*   **Build Tool:** [Vite](https://vitejs.dev/) is used for a fast development server and optimized production builds.

## Project Structure

The project is organized into several key files and directories:

```
/
├── API/
│   └── products.json         # Mock database for product data
├── public/                     # Static assets like images
├── index.html                  # Main landing page
├── products.html               # All products listing page
├── addToCart.html              # Shopping cart page
├── about.html                  # About Us page
├── contact.html                # Contact Us page
├── style.css                   # All styles for the application
├── main.js                     # Main JavaScript entry point
├── addToCart.js                # Logic for adding items to the cart
├── removeProdFromCart.js       # Logic for removing items from the cart
├── showAddToCartCards.js       # Renders items on the cart page
├── homeProductCards.js         # Renders product cards on the homepage/products page
├── updateCartValue.js          # Updates the cart count in the navbar
├── updateCartProductTotal.js   # Calculates and displays the cart total
├── getCartProducts.js          # Retrieves cart data from localStorage
├── package.json                # Project dependencies and scripts
└── ... (other JS modules)
```

## Getting Started

To run this project locally, follow these steps:

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/lazy-coder99/Ecom-project.git
    ```

2.  **Navigate to the project directory:**
    ```sh
    cd Ecom-project
    ```

3.  **Install dependencies:**
    This project uses `vite`, which is listed as a dev dependency.
    ```sh
    npm install
    ```

4.  **Run the development server:**
    This command will start the Vite development server, and you can view the website at `http://localhost:5173` (or another port if 5173 is in use).
    ```sh
    npm run dev
    ```

5.  **Build for production:**
    To create a production-ready build of the application:
    ```sh
    npm run build
    ```
    The optimized files will be generated in the `dist/` directory.
