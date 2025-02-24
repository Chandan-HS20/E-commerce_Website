# E-commerce Website Application

This is a backend-only implementation of an E-commerce web application built using Spring Boot. It supports product management, user authentication, order management, and integrates with Stripe for payment processing (Stripe integration to be completed). The frontend will be developed using React in the future.

## Features
1. **User Registration & Login**: Users can register and log in using JWT-based authentication.  
2. **Product Catalog**: Display of products with options for browsing and searching.  
3. **Shopping Cart**: Users can add products to the shopping cart and view the cart contents.  
4. **Order Management**: Users can place orders and view order details.  
5. **Stripe Payment Integration**: Payment functionality is planned to be integrated with Stripe (coming soon).  
6. **Admin Panel**: Admins can manage products, orders, and categories.

## Technologies Used
- **Backend**: Spring Boot, Spring Security, JWT, Maven  
- **Frontend (Future)**: React  
- **Database**: PostgreSQL  
- **Payment Integration (Coming Soon)**: Stripe (for processing payments)  
- **Build Tool**: Maven for the backend

## Prerequisites
- Java 11+ (for backend)  
- PostgreSQL (for the database)  
- Maven (for building the backend)

## Installation Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Chandan-HS20/SpEcom.git
   cd SpEcom
Set up the Backend: Navigate to the sp-ecom folder:

bash
cd sp-ecom
Install dependencies using Maven:

bash
mvn clean install
Set up your PostgreSQL database and configure the connection settings in the src/main/resources/application.properties file:

properties
spring.datasource.url=jdbc:postgresql://localhost:5432/your_database_name
spring.datasource.username=your_username
spring.datasource.password=your_password
Run the backend application:

bash
mvn spring-boot:run
The backend application should now be running on http://localhost:8080.

Stripe Payment Integration (Coming Soon)
The backend is set up to handle payments through Stripe, but the frontend integration is yet to be developed. Once the frontend is ready, the backend will process payments via Stripe.

## Usage

- **Register**: Create an account using the Sign-Up API.  
- **Login**: Log in using the credentials you created.  
- **Browse Products**: View products via the API endpoints.  
- **Add to Cart**: Add items to your shopping cart through the Cart API.  
- **Place Orders**: Complete orders via the Order API.  
- **Payment (Coming Soon)**: Payment processing will be added once the frontend is ready.

## API Documentation

### Authentication:
- `POST /api/auth/signup`: Register a new user.  
- `POST /api/auth/signin`: Log in with JWT authentication.

### Products:
- `GET /api/products`: List all products.  
- `POST /api/products`: Add a new product (Admin only).  
- `GET /api/products/{id}`: View a specific product by ID.

### Cart:
- `POST /api/cart`: Add a product to the cart.  
- `GET /api/cart`: View the cart contents.  
- `DELETE /api/cart/{itemId}`: Remove an item from the cart.

### Orders:
- `POST /api/orders`: Place a new order.  
- `GET /api/orders`: View all orders for the logged-in user.

## Contributing
If you'd like to contribute to this project, feel free to fork the repository, create a branch for your feature, and submit a pull request with your changes.

### Steps for Contributing:
1. Fork the repository.  
2. Create a new branch for your feature (`git checkout -b feature-name`).  
3. Make your changes and commit them (`git commit -m "Add new feature"`).  
4. Push to the branch (`git push origin feature-name`).  
5. Open a pull request to merge your changes into the main branch.

## Acknowledgements
- Thanks to Spring Boot for providing the backend framework.  
- Thanks to PostgreSQL for the relational database management system.  
- Thanks to JWT for securing user authentication.  
- Thanks to Stripe for the upcoming payment integration.  
- Thanks to Faisal Memon (EmbarkX).

## Additional Notes:
### Frontend Development (React):
Once the frontend is developed using React, it will communicate with the backend APIs to handle user interaction, display products, manage the cart, and complete the checkout process.

### Stripe Integration:
Stripe will be integrated once the frontend is ready. This will allow users to securely make payments for their orders.

