# Java REST API CRUD Example

This project is a simple REST API built using Java and Spring Boot that demonstrates basic CRUD operations. The API manages a collection of `Product` entities with the following fields: `id`, `name`, `description`, and `price`.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Requirements](#requirements)
- [Setup Instructions](#setup-instructions)
  - [Clone the Repository](#1-clone-the-repository)
  - [Build the Project](#2-build-the-project)
  - [Run the Application](#3-run-the-application)
- [API Endpoints](#api-endpoints)
  - [Create a New Product](#1-create-a-new-product)
  - [Get All Products](#2-get-all-products)
  - [Get a Product by ID](#3-get-a-product-by-id)
  - [Update a Product](#4-update-a-product)
  - [Delete a Product](#5-delete-a-product)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

This project is a basic REST API example using Spring Boot, showcasing how to perform CRUD operations on `Product` entities.

## Project Structure

```plaintext
yourrepository/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/yourusername/yourproject/
│   │   │       ├── ProductApiApplication.java
│   │   │       ├── controller/
│   │   │       │   └── ProductController.java
│   │   │       ├── model/
│   │   │       │   └── Product.java
│   │   │       └── repository/
│   │   │           └── ProductRepository.java
│   ├── resources/
│   │   └── application.properties
│   └── test/
│       └── java/
│           └── com/yourusername/yourproject/
│               └── ProductApiApplicationTests.java
│
├── .gitignore
├── README.md
├── pom.xml
└── mvnw
