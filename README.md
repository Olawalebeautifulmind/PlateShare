# PlateShare
PlateShare is an intelligent, real-time platform that connects food providers (restaurants, cafés, grocery stores) with organizations supporting vulnerable communities to efficiently redistribute surplus food and reduce food waste.

## Features

### For Food Providers
- Easy listing of surplus food items
- Real-time tracking of food pickup status
- Impact metrics dashboard
- Automated expiry notifications
- Flexible pickup window scheduling

### For Recipients (Charities/Shelters)
- Real-time food availability notifications
- Geographic-based food search
- Dietary and allergen filtering
- Pickup scheduling and coordination
- Impact tracking and reporting

### General Features
- User authentication and verification
- Role-based access control
- Real-time notifications
- Mobile-responsive design
- Interactive maps
- Rating and feedback system

## Tech Stack

### Frontend
- React with TypeScript
- Material-UI for components
- React Router for navigation
- Axios for API requests
- React Query for state management

### Backend
- Node.js with Express
- TypeScript for type safety
- MongoDB for database
- JWT for authentication
- Mongoose for ODM

## Prerequisites

- Node.js (v14 or higher)
- MongoDB (v4.4 or higher)
- npm or yarn
- Git

## Installation

1. Clone the repository
```bash
git clone https://github.com/Olawalethebeautifulmind/plateshare.git
cd plateshare
```

2. Install Frontend Dependencies
```bash
cd frontend
npm install
```

3. Install Backend Dependencies
```bash
cd ../backend
npm install
```

4. Set up environment variables
```bash
# In backend directory
cp .env.example .env
# Edit .env with your configuration
```

5. Build the project
```bash
# In backend directory
npm run build

# In frontend directory
npm run build
```

## Running the Application

1. Start MongoDB
```bash
# Make sure MongoDB is running on your system
```

2. Start the Backend Server
```bash
cd backend
npm run dev
```

3. Start the Frontend Development Server
```bash
cd frontend
npm start
```

The application will be available at:
- Frontend: http://localhost:3000
- Backend API: http://localhost:5000

## API Documentation

### Authentication Endpoints
- POST /api/users/register - Register a new user
- POST /api/users/login - Login user
- GET /api/users/profile - Get user profile
- PUT /api/users/profile - Update user profile

### Food Listing Endpoints
- POST /api/food-listings - Create a new food listing
- GET /api/food-listings - Get all food listings
- GET /api/food-listings/:id - Get single food listing
- PUT /api/food-listings/:id - Update food listing
- DELETE /api/food-listings/:id - Delete food listing
- POST /api/food-listings/:id/reserve - Reserve food listing
- POST /api/food-listings/:id/complete - Complete food pickup
- GET /api/food-listings/nearby - Get nearby food listings

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- All the food providers and charities working to reduce food waste
- The open-source community for the amazing tools and libraries
- Everyone contributing to food security and sustainability 
