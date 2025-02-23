# Portfolio API

## Project Overview

This is a RESTful API for managing user portfolios, including features like user authentication, portfolio CRUD operations, and JWT-based authentication.

---

## Installation & Setup

### Prerequisites

- Node.js (v16+ recommended)
- MongoDB (local or cloud-based)
- npm (Node Package Manager)

### Clone the Repository

```sh
git clone https://github.com/yourusername/portfolio-api.git
cd portfolio-api
```

### Install Dependencies

```sh
npm install
```

### Environment Variables

Create a `.env` file in the root directory and add the following variables:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

---

## Running the Project

Start the server using **nodemon**:

```sh
nodemon index.js
```

If you don't have nodemon installed globally, install it first:

```sh
npm install -g nodemon
```

Or run it using `npm`:

```sh
npm start
```

The server will start on `http://localhost:5000/`.

---

## API Documentation

For detailed API documentation and testing endpoints, visit the Postman documentation: 📌 **Postman Documentation:** [Click Here](your_postman_documentation_link)

---

## Available Routes

### **User Authentication**

- **POST** `/api/register` → Register a new user
- **POST** `/api/login` → Login and receive a JWT token

### **Portfolio Management**

- **GET** `/api/portfolio` → Get all portfolios
- **GET** `/api/portfolio/:id` → Get a single portfolio by ID
- **POST** `/api/portfolio` → Create a new portfolio (Authentication required)
- **PUT** `/api/portfolio/:id` → Update a portfolio (Authentication required)
- **DELETE** `/api/portfolio/:id` → Delete a portfolio (Authentication required)

---

## Technologies Used

- **Backend:** Node.js, Express.js
- **Database:** MongoDB, Mongoose
- **Authentication:** JWT (JSON Web Token)
- **API Testing:** Postman

---

## Contributing

Feel free to fork this repository and submit pull requests with improvements or bug fixes!

---

## License

This project is licensed under the MIT License.

