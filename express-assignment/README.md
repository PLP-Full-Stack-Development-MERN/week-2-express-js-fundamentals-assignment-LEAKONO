# Express.js Fundamentals Assignment

## Project Overview
This project is an Express.js-based RESTful API that implements fundamental concepts of routing, middleware, controllers, and error handling. The API manages user and product resources, allowing basic CRUD operations.

## Features
- RESTful API routes for users and products.
- Custom middleware for logging requests.
- Environment variable management using `dotenv`.
- Global error-handling middleware.
- Organized project structure for maintainability.

## Technologies Used
- Node.js
- Express.js
- MongoDB (Mongoose for ODM)
- Dotenv (for environment variables)
- Postman (for API testing)

## Project Structure
```
express-assignment/
│-- routes/
│    ├── userRoutes.js
│    ├── productRoutes.js
│-- middleware/
│    ├── logger.js
│-- controllers/
│    ├── userController.js
│    ├── productController.js
│-- models/
│    ├── User.js
│    ├── Product.js
│-- index.js
│-- package.json
│-- .env
│-- README.md
```

## Installation

### Prerequisites
- Node.js (installed via NVM)
- MongoDB (running locally or via cloud)

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/PLP-Full-Stack-Development-MERN/week-2-express-js-fundamentals-assignment-LEAKONO.git
   cd express-assignment
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Create a `.env` file and configure environment variables:
   ```env
   PORT=5000
   MONGO_URI=mongodb://localhost:27017/product
   JWT_SECRET=mysecretkey
   ```
4. Start the server:
   ```sh
   node index.js
   ```

## API Endpoints

### Users API
| Method | Endpoint | Description |
|--------|---------|-------------|
| GET    | `/users` | Get all users |
| POST   | `/users` | Create a new user |
| PUT    | `/users/:id` | Update a user by ID |
| DELETE | `/users/:id` | Delete a user by ID |

### Products API
| Method | Endpoint | Description |
|--------|---------|-------------|
| GET    | `/products` | Get all products |
| POST   | `/products` | Create a new product |
| PUT    | `/products/:id` | Update a product by ID |
| DELETE | `/products/:id` | Delete a product by ID |

## Middleware
- **Logger Middleware**: Logs HTTP requests (method, URL, and timestamp).
- **Global Error Handler**: Handles and formats errors gracefully.

## Testing
- Use Postman or cURL to test API endpoints.
- Example request using cURL:
  ```sh
  curl -X GET http://localhost:5000/products
  ```

## Contributing
Feel free to fork the repository and submit pull requests for improvements.

## License
This project is open-source and available under the MIT License.

