# Food Ordering System

A comprehensive food ordering system designed to facilitate the process of ordering food from various restaurants. This system is built to provide users with an intuitive interface to browse, select, and order food items, while offering restaurant owners the tools to manage their menu items and track orders efficiently.

## Overview

The Food Ordering System allows users to register and log in, browse nearby restaurants, view their menus, add items to a cart, and place orders. Restaurant owners can manage their restaurant information, menu items, and view customer orders. The system includes features for user authentication, session management, and data validation.

## Features

- User registration and authentication
- Browse restaurants by category and rating
- View restaurant menus and item details
- Add items to cart, adjust quantities, and place orders
- Restaurant management (menu items, categories)
- Order management for users and restaurant owners
- Secure API endpoints with role-based access control

## Technologies Used

- **Backend**: Java, Spring Boot, Hibernate
- **Frontend**: React
- **Security**: Spring Security, BCrypt
- **Utilities**: Geolocation (OpenStreetMap), Haversine distance calculation

## Getting Started

### Prerequisites

- Java 11 or higher
- Node.js and npm
- PostgreSQL

### Installation

1. Clone the repository
   ```sh
   git clone https://github.com/BogdanCocis/FoGo.git
   ```
2. Backend setup
   ```sh
   cd your-repo-name/backend
   ./mvnw spring-boot:run
   ```
3. Frontend setup
   ```sh
   cd your-repo-name/frontend
   npm install
   npm start
   ```
