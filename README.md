# Food Ordering System
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
- MySQL

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

## Usage

### User Registration and Login

1. **Home Page**: When a user first enters the application, they are greeted with the home page.
   - The home page contains a prompt to "Login/Sign Up".
<div align="center"> 
  <img width="750" alt="home-page" src="https://github.com/user-attachments/assets/92c63487-d8f1-4052-b23b-413295d04dbb" />
</div>
<br><br> 

2. **Registration**: If the user doesn't have an account, they can click on the "Login/Sign Up" button and choose to register.
   - The registration form requires the user to provide their name, email, password, and phone number.
<div align="center"> 
  <img width="750" alt="register" src="https://github.com/user-attachments/assets/b401aae0-8ffc-4e27-9923-1eba6f47b6f6"/>
</div>
<br><br> 

3. **Login**: Registered users can log in using their email and password.   
 <div align="center"> 
  <img width="750" alt="log-in" src="https://github.com/user-attachments/assets/8cf8faad-0c8e-417a-b2f5-a3672d9737e7"/>
</div>
<br><br> 
- Upon successful login, the user is redirected to the main application interface.

### Browsing and Selecting Restaurants

1. **Location Input**: On the main page, users can enter their location to find nearby restaurants.
   - The system uses geolocation services to convert the address into coordinates and find restaurants within a specified radius.
<div align="center"> 
  <img width="750" alt="map" src="https://github.com/user-attachments/assets/ef34947f-98fd-45ae-8016-96411c5be356"/>
</div>
<br><br> 

2. **Top-Rated Restaurants**: Users are presented with a list of top-rated restaurants based on their location.
   - The list includes restaurant names, descriptions, ratings, and categories.
   - Users can filter the list of restaurants by selecting one or more categories.
<div align="center"> 
  <img width="750" alt="top-rated" src="https://github.com/user-attachments/assets/f0463d25-5250-42c4-8725-0e8365cbb6d8"/>
</div>
<br><br> 

### Viewing Menus and Ordering Food

1. **Restaurant Menu**: Clicking on a restaurant name takes the user to the restaurant's menu page.
   - The menu page displays a list of available dishes, including names, descriptions, prices, and availability.
<div align="center">
    <img width="750" style="display: block; margin: 0; padding: 0;" alt="menu1" 
         src="https://github.com/user-attachments/assets/6dcd71e9-db8b-499d-8059-78d5c8c7693c"/>
    <img width="750" style="display: block; margin: -0; padding: -0;" alt="menu2" 
         src="https://github.com/user-attachments/assets/57d4f48a-a364-4326-8327-f5e38bacf345"/>
</div>
<br><br> 

3. **Adding Items to Cart and Cart Management**: Users can select the quantity of each dish they want to order and add it to their cart.
   - They can adjust the quantity of items, remove items, or proceed to checkout.
<div align="center"> 
  <img width="750" alt="cart" src="https://github.com/user-attachments/assets/29017ab3-b271-41ba-a55f-6ba9ce6feac2"/>
</div>
<br><br>

### Placing an Order

1. **Checkout**: In the cart page, users enter their delivery address and review their order.
   - The total price is calculated based on the items in the cart.

2. **Payment Processing**: Users click the "Pay" button to initiate the payment process.
   - A processing popup is displayed while the payment is being processed.
   - Upon successful payment, a "Thank You" popup is displayed, and the order is confirmed.

## Database Schema

The database schema for the Food Ordering System is visually represented below:

<div align="center"> 
   <img width="1276" alt="db_fogo" src="https://github.com/user-attachments/assets/c034706b-2f48-49b8-96a3-c62e652cc7d0" />
</div>
<br><br>
