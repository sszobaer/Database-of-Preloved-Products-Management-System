# Preloved Product Management System Database

## Overview

The **Preloved Product Management System** is a database developed in Oracle 10g to manage the core operations of a marketplace where users can buy and sell preloved or second-hand products. The database handles various aspects of the marketplace, including user registration, product listings, order management, and payment processing.

This system aims to streamline the management of second-hand product transactions, ensuring a smooth experience for both buyers and sellers.

## Features

1. **User Management**
   - Allows users to register, log in, and manage their profiles.
   - Differentiates between user roles (buyers and sellers).
   - Secure storage of personal information and login credentials.

2. **Product Listings**
   - Enables sellers to list products with key details such as product name, description, price, condition, and availability.
   - Products can be updated or removed as needed by the sellers.

3. **Order Management**
   - Handles orders placed by buyers, including tracking order status (pending, shipped, delivered).
   - Records shipping details and manages order history.

4. **Transaction Handling**
   - Facilitates secure payment processing for all transactions.
   - Tracks payment status and transaction history for both buyers and sellers.

5. **Review and Rating System**
   - Allows buyers to rate products and provide feedback, improving transparency and product quality over time.
   - Stores review details such as rating, comments, and timestamps.

## Database Structure

The database is designed with the following key tables:

1. **Users Table**
   - Stores user information including user ID, username, password, role (buyer/seller), and contact details.
   
2. **Products Table**
   - Contains product listings with fields for product ID, name, description, price, condition, category, and seller ID (foreign key referencing the `Users` table).

3. **Orders Table**
   - Manages order details with fields for order ID, buyer ID (foreign key), product ID (foreign key), order date, status, and payment information.

4. **Transactions Table**
   - Records payment details for each transaction, including payment ID, order ID, transaction amount, and payment status.

5. **Reviews Table**
   - Tracks product reviews and ratings with fields for review ID, buyer ID, product ID, rating, and comments.

## Installation

1. Install Oracle 10g or later.
2. Clone the repository containing the SQL scripts for table creation and data insertion.
3. Run the provided SQL scripts to set up the database schema.
4. Configure database connection settings based on your local environment.

## Usage

Once the database is set up, you can:

1. **Add New Users**: Register new buyers or sellers in the system.
2. **List Products**: Sellers can add new product listings, including all necessary details.
3. **Manage Orders**: Buyers can place orders and track their status from creation to delivery.
4. **Process Payments**: Payments can be processed and tracked within the system.
5. **Review Products**: Buyers can leave reviews and ratings for purchased products.

## Future Enhancements

- Implement additional payment methods and integrate with external payment gateways.
- Add a messaging system for communication between buyers and sellers.
- Improve reporting and analytics for marketplace trends, popular products, and user activity.

## License

This project is open-source and can be freely modified and distributed under the MIT License.

---

For more details, contributions, or bug reports, please contact the project administrator.
