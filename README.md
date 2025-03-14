# XCart-Ecom-API

This is a backend API for a basic Ecommerce application built using **Node.js**, **Express.js**, and **MongoDB**. The API is designed to be fast, scalable, and easy to integrate with frontend applications.

---

## **Features**
✅ User Authentication (JWT-based)  
✅ Product Management (CRUD)  
✅ Cart Management  
✅ Order Placement and Tracking  
✅ Secure and Efficient Data Handling  

---

## **Tech Stack**
- **Node.js** – Backend framework  
- **Express.js** – Web framework  
- **MongoDB** – NoSQL database  
- **JWT** – Authentication  
- **Mongoose** – MongoDB object modeling  

---

## **Setup and Installation**

### **1. Clone the Repository**
```bash
git clone https://github.com/Bijay-Prasad/xcart-ecom-api.git
cd xcart-ecom-api
```
### **2. Install Dependencies**
```bash
npm install
```

### **API Endpoints**
You can test the API using the provided Postman collection.

#### Import Postman Collection
1. Open Postman.
2. Import the file postman-collection.json (provided in the repository).
3. Update the environment variables if needed.

### **Authentication**
Method - Endpoint - Description
- POST - /api/auth/register - Register a new user
- POST - /api/auth/login - Login and receive a JWT

### **Products**
Method - Endpoint - Description
- POST - /api/products - Add a new product
- GET - /api/products - List all products
- GET - /api/products/:id - Get product details
- PUT - /api/products/:id - Update product details
- DELETE - /api/products/:id - Delete a product

### **Cart**
Method - Endpoint - Description
- POST - /api/cart - Add product to cart
- GET - /api/cart - Get cart details
- PUT - /api/cart/:id - Update cart
- DELETE - /api/cart/:id - Remove product from cart

### **Orders**
Method - Endpoint - Description
- POST - /api/orders - Create an order
- GET - /api/orders - Get all orders for the user
- GET - /api/orders/:id - Get order details

### **Environment Variables**
Ensure to add the following environment variables to the .env file:

- `MONGO_URI` – MongoDB connection string
- `JWT_SECRET` – Secret key for JWT
- `PORT` – Port number for the server

### **.gitignore**
The following files and directories are ignored:

```bash[gitignore]
node_modules/  
.env
```