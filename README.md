# E-commerce Web Platform 🛒

A full-stack e-commerce application built with a powerful Spring Boot backend and a modern, reactive Vite + React frontend. This platform provides core functionalities for managing an online product catalog.

## ✨ Features

  * **View Products**: Fetches and displays a list of all available products.
  * **Add Products**: A user-friendly form to add new products to the catalog.
  * **Update Products**: Easily edit the details of any existing product.
  * **Delete Products**: Remove products that are no longer needed.
  * **Dynamic Search**: Instantly search for products by name, description, brand, or category.

-----

## 🛠️ Tech Stack

This project is built using the following technologies:

  * **Backend**:

      * **Java 17+**
      * **Spring Boot**: For building the robust REST API.
      * **Spring Data JPA**: For data persistence and repository management.
      * **Hibernate**: As the JPA implementation.
      * **MySQL/PostgreSQL**: As the relational database (can be configured for H2 as well).
      * **Maven**: For dependency management.

  * **Frontend**:

      * **React.js**: For building the user interface.
      * **Vite**: As the blazing-fast build tool and development server.
      * **Axios**: For making API requests to the backend.
      * **CSS**: For styling the application (e.g., Tailwind CSS, Material-UI).

-----

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Make sure you have the following software installed on your machine:

  * Git
  * JDK 17 or later
  * Maven
  * Node.js and npm
  * A running instance of MySQL or PostgreSQL database.

### Installation & Setup

#### 1\. Backend (Spring Boot)

```bash
# Clone the repository
git clone https://github.com/LogeshR2005/Ecommerce-Platform.git

# Navigate to the backend directory
cd <Ecommerce-Platform-SpringBoot-Java>/backend-folder

# Configure the database
# Open `src/main/resources/application.properties`
# Update the following properties to match your database configuration:
# spring.datasource.url=jdbc:mysql://localhost:3306/your_db_name
# spring.datasource.username=your_db_username
# spring.datasource.password=your_db_password

# Build the project and run the application
mvn spring-boot:run
```

The backend server will start on `http://localhost:8080`.

#### 2\. Frontend (Vite + React)

```bash
# Navigate to the frontend directory from the root folder
cd ../frontend-folder

# Install dependencies
npm install

# Start the development server
npm run dev
```

The frontend application will be available at `http://localhost:5173` (or another port specified by Vite).

-----

## 📄 API Endpoints

The backend exposes the following RESTful endpoints:

| HTTP Method | Endpoint                       | Description                                |
|-------------|--------------------------------|--------------------------------------------|
| `GET`       | `/api/products`                | Get a list of all products.                |
| `GET`       | `/api/products/{id}`           | Get a single product by its ID.            |
| `POST`      | `/api/products`                | Add a new product to the database.         |
| `PUT`       | `/api/products/{id}`           | Update an existing product.                |
| `DELETE`    | `/api/products/{id}`           | Delete a product by its ID.                |
| `GET`       | `/api/products/search?keyword=...` | Search for products based on a keyword.    |

-----



## ⚖️ License

This project is licensed under the MIT License - see the `LICENSE` file for details.
