
# System Overview

This system represents a **basic e-commerce platform** designed to manage customer orders, products, payments, and categories. It includes functionalities for customers to register, place orders, and make payments, while also managing product inventory and categories.

## Key Features
- **Customer Management**: Register, log in, and update profiles.
- **Order Processing**: Add items to orders, calculate totals, and update order status.
- **Payment Handling**: Process payments for completed orders.
- **Product Inventory Management**: Track product stock levels and apply discounts.
- **Category Management**: Organize products by categories.

---

# Key Entities

### 1. **Customer**
Represents customers interacting with the system.
- **Attributes**:
  - `customerID`: Unique identifier for each customer.
  - `name`: Name of the customer.
  - `email`: Contact email.
  - `phoneNumber`: Customer's contact number.
  - `address`: Customer's delivery address.
  - `password`: Encrypted password for account security.
- **Methods**:
  - `register()`: Registers a new customer.
  - `login()`: Allows the customer to log in.
  - `updateProfile()`: Updates the customer’s profile information.

---

### 2. **Order**
Handles the processing of customer orders.
- **Attributes**:
  - `orderID`: Unique identifier for each order.
  - `customer`: Associated customer placing the order.
  - `date`: Date the order was created.
  - `status`: Current status of the order (e.g., pending, completed).
  - `orderItems`: List of items included in the order.
  - `totalAmount`: Total cost of the order.
- **Methods**:
  - `addOrderItem()`: Adds a product to the order.
  - `calculateTotal()`: Calculates the total amount of the order.
  - `updateStatus()`: Updates the order’s status.

---

### 3. **OrderItem**
Represents individual items in an order.
- **Attributes**:
  - `product`: The product being ordered.
  - `quantity`: Quantity of the product ordered.
  - `subTotal`: Subtotal cost for the product (price * quantity).
- **Methods**:
  - `calculateSubTotal()`: Calculates the subtotal for this item.

---

### 4. **Product**
Represents products available for sale.
- **Attributes**:
  - `productID`: Unique identifier for each product.
  - `name`: Name of the product.
  - `description`: Detailed description of the product.
  - `price`: Price of the product.
  - `stockQuantity`: Quantity of the product available in stock.
  - `category`: Category to which the product belongs.
- **Methods**:
  - `updateStock()`: Updates the product’s stock quantity.
  - `applyDiscount()`: Applies discounts to the product price.

---

### 5. **Category**
Organizes products into groups for easier navigation.
- **Attributes**:
  - `categoryID`: Unique identifier for each category.
  - `name`: Name of the category.

---

### 6. **Payment**
Handles payment processing for orders.
- **Attributes**:
  - `paymentID`: Unique identifier for each payment.
  - `order`: Associated order for which the payment is made.
  - `amount`: Total payment amount.
  - `date`: Payment date.
  - `paymentMethod`: Method of payment (e.g., card, cash).
- **Methods**:
  - `processPayment()`: Processes the payment for the order.

---

# Installation and Usage
1. **Prerequisites**:
   - Ensure a backend system supports the implementation of these entities (e.g., a relational database).
   - Use programming languages or frameworks capable of implementing object-oriented structures (e.g., Java, Python, or C#).

2. **Steps**:
   - Clone or download the system files.
   - Set up the database structure following the class diagram.
   - Implement the described methods to handle user and system interactions.
   - Test the system to ensure all functionalities work as expected.

---

---

## Contributors  

1. 22UG1-0281 | Sahan Wijesinghe
2. 22UG1-0323 | Kasun Chamika
3. 
---

