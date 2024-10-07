
# Home_Rental_App

The Home Rental Web Application is a platform designed to facilitate the listing, searching, and renting of properties. This web app provides a seamless experience for homeowners to list their properties and for potential renters to search for homes, based on location, price, and other amenities. It features property listings, user authentication, and state management using Redux.


## Features

- Property Listings: Homeowners can list their properties, including details like price, location, and description.

- Search & Filter: Renters can search and filter properties by various parameters (e.g., price range, location, property type).

- User Authentication: Secure login and registration for users.

- Responsive Design: The platform is designed to work on both mobile and desktop devices.

- State Management: Global state handling with Redux to manage user login, property listings, and other application state.

## Tech Stack

**Client:** React, Redux, SCSS 

**Server:** Node, Express, MongoDB


## API Design

StudyNotion's API follows the REST architectural style, implemented using Node.js and Express.js. It uses JSON for data exchange and standard HTTP request methods. Sample API endpoints include:
# API Routes

## Authentication Routes

- **POST** `/api/auth/register`  
  Register a new user with profile image upload.

- **POST** `/api/auth/login`  
  Log in a user and return a JWT token.

---

## Booking Routes

- **POST** `/api/bookings/create`  
  Create a new booking with customer and listing details.

- **GET** `/api/bookings/:userId/trips`  
  Get all trips for a specific user (as a customer).

- **PATCH** `/api/bookings/:userId/:listingId`  
  Add or remove a listing from the user's wishlist.

- **GET** `/api/bookings/:userId/properties`  
  Get all properties listed by a specific user (as a host).

- **GET** `/api/bookings/:userId/reservations`  
  Get all reservations made for a specific user's properties.

---

## Listing Routes

- **POST** `/api/listings/create`  
  Create a new property listing with multiple photos upload.

- **GET** `/api/listings`  
  Get all listings or filter by category.

- **GET** `/api/listings/search/:search`  
  Search listings by category or title.

- **GET** `/api/listings/:listingId`  
  Get a specific listing by ID.

---
## Run Locally

Clone the project

```bash
  git clone https://github.com/Geetansh431/Home-Rental-Web
```
Go to the backend directory

```bash
  cd server
```

Install dependencies

```bash
  npm install
```

create **.env file** 

Start the server

```bash
  npm run start
```

Go to the frontend directory using Other Terminal

```bash
  cd ../
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run start
```


# .env.example

- MongoDB Connection String: YOUR_MONGO_URL

- JWT_SECRET='YOUR_JWT_SECRET'
## Demo

Live Link Coming Soon
## Contributing to Home_Rental_App 🤝

We welcome and appreciate contributions from the community to enhance and improve Home_Rental_App. Whether you're a developer, designer, tester, or someone with valuable feedback, your input is valuable to us.

## Thank You!❤️

Thank you for considering contributing to the Home_Rental_App. Your efforts help make this project better for everyone. If you have any questions or need assistance, feel free to reach out through the issue tracker or discussions. Happy coding🤩!
