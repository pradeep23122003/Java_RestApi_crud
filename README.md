# Java REST API CRUD Example

This project is a simple REST API built using Java and Spring Boot that demonstrates basic CRUD operations. The API manages a collection of `Product` entities with the following fields: `id`, `name`, `description`, and `price`.

## Project Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/yourrepository.git
   cd yourrepository
Build the Project:
Make sure you have Maven installed. Build the project using:

mvn clean install
Run the Application:
Run the application using:

mvn spring-boot:run
API Endpoints
1. Create a New Product
URL: /api/products
Method: POST
Request Body:
json

{
  "name": "Product Name",
  "description": "Product Description",
  "price": 99.99
}
Response:
json

{
  "id": 1,
  "name": "Product Name",
  "description": "Product Description",
  "price": 99.99
}
2. Get All Products
URL: /api/products
Method: GET
Response:
json

[
  {
    "id": 1,
    "name": "Product Name",
    "description": "Product Description",
    "price": 99.99
  },
  {
    "id": 2,
    "name": "Another Product",
    "description": "Another Description",
    "price": 149.99
  }
]
3. Get a Product by ID
URL: /api/products/{id}
Method: GET
Response:
json

{
  "id": 1,
  "name": "Product Name",
  "description": "Product Description",
  "price": 99.99
}
4. Update a Product
URL: /api/products/{id}
Method: PUT
Request Body:
json

{
  "name": "Updated Product Name",
  "description": "Updated Description",
  "price": 119.99
}
Response:
json

{
  "id": 1,
  "name": "Updated Product Name",
  "description": "Updated Description",
  "price": 119.99
}
5. Delete a Product
URL: /api/products/{id}
Method: DELETE
Response:
json

{
  "message": "Product deleted successfully"
  }
src
├── main
│   ├── java
│   │   └── com
│   │       └── example
│   │           └── productapi
│   │               ├── ProductApiApplication.java
│   │               ├── controller
│   │               │   └── ProductController.java
│   │               ├── model
│   │               │   └── Product.java
│   │               └── repository
│   │                   └── ProductRepository.java
│   └── resources
│       └── application.properties
└── test
    └── java
        └── com
            └── example
                └── productapi
                    └── ProductApiApplicationTests.java
