# JavaScript Full Stack Capstone Project: GiftLink

## Overview

This is a full-stack JavaScript application for a gift linking platform. The project demonstrates full-stack development skills with Node.js backend, React frontend, and MongoDB database.

## Features

- User authentication (login and registration)
- Gift search functionality
- Gift details page
- User profile management
- Sentiment analysis integration

## Project Structure

- `giftlink-backend/`: Node.js/Express backend with API routes for authentication, gifts, and search
- `giftlink-frontend/`: React frontend application
- `sentiment/`: Sentiment analysis module
- `db.js`, `app.js`, etc.: Additional backend files
- `user-story.md`: Project user stories and requirements

## Installation

### Prerequisites

- Node.js
- MongoDB
- npm or yarn

### Backend Setup

```bash
cd giftlink-backend
npm install
```

### Frontend Setup

```bash
cd giftlink-frontend
npm install
```

## Running the Application

### Start Backend

```bash
cd giftlink-backend
npm start
```

The backend will run on `http://localhost:3001` (or configured port).

### Start Frontend

```bash
cd giftlink-frontend
npm start
```

The frontend will run on `http://localhost:3000`.

## Database

The application uses MongoDB. Ensure MongoDB is installed and running. Database configuration is in `giftlink-backend/models/db.js`.

To populate the database with initial data, run the import script in `giftlink-backend/util/import-mongo/`.

## Technologies Used

- **Backend**: Node.js, Express.js, MongoDB, JWT for authentication
- **Frontend**: React, CSS
- **Other**: Sentiment analysis (possibly using external libraries)

## Contributing

This is a capstone project. For any issues or improvements, please refer to the user stories in `user-story.md`.

## License

This project is for educational purposes.
