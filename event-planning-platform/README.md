# EventHub - Event Planning Platform

A comprehensive full-stack web application for event planning that connects customers with venues and service providers.

## Features

### 👥 User Roles
- **Customers**: Browse venues, book services, manage bookings
- **Venue Owners**: Upload venues, manage bookings, view analytics
- **Service Providers**: List services, manage availability, accept bookings
- **Admin**: Approve registrations, manage users, handle disputes

### 🎯 Key Features
- Location-based venue and service search
- Real-time availability checking
- Integrated booking system
- Ratings and reviews system
- Payment processing with Stripe
- Multiple event types support
- Service filters (location, date, price, ratings)
- Dashboard for all user roles

## Tech Stack

### Frontend
- React.js 18
- React Router v6
- Axios for API calls
- Google Maps integration
- Stripe integration

### Backend
- Node.js + Express.js
- MongoDB
- JWT Authentication
- Cloudinary for image storage
- Stripe Payment API

## Project Structure

```
event-planning-platform/
├── frontend/
│   ├── public/
│   │   └── index.html
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.js
│   │   │   └── Navbar.css
│   │   ├── pages/
│   │   │   ├── Home.js
│   │   │   ├── Login.js
│   │   │   ├── Register.js
│   │   │   ├── VenueSearch.js
│   │   │   ├── VenueDetail.js
│   │   │   ├── Services.js
│   │   │   ├── CustomerDashboard.js
│   │   │   ├── VenueOwnerDashboard.js
│   │   │   └── ServiceProviderDashboard.js
│   │   ├── App.js
│   │   ├── App.css
│   │   ├── index.js
│   │   └── index.css
│   └── package.json
│
├── backend/
│   ├── models/
│   │   ├── User.js
│   │   ├── Venue.js
│   │   ├── Service.js
│   │   └── Booking.js
│   ├── routes/
│   │   ├── authRoutes.js
│   │   ├── venueRoutes.js
│   │   ├── serviceRoutes.js
│   │   └── bookingRoutes.js
│   ├── server.js
│   ├── .env.example
│   └── package.json
│
└── README.md
```

## Setup Instructions

### Backend Setup

1. Navigate to backend directory:
   ```
   cd backend
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Create `.env` file from `.env.example`:
   ```
   cp .env.example .env
   ```

4. Configure environment variables in `.env`

5. Start MongoDB service

6. Run the server:
   ```
   npm run dev
   ```

### Frontend Setup

1. Navigate to frontend directory:
   ```
   cd frontend
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Start the React app:
   ```
   npm start
   ```

The app will run on `http://localhost:3000`

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login

### Venues
- `GET /api/venues/search?location=<location>` - Search venues by location
- `GET /api/venues/:id` - Get venue details
- `POST /api/venues/` - Create new venue
- `PUT /api/venues/:id` - Update venue

### Services
- `GET /api/services/type/:type` - Get services by type
- `GET /api/services/:id` - Get service details
- `POST /api/services/` - Create new service

### Bookings
- `POST /api/bookings/` - Create booking
- `POST /api/bookings/payment` - Process payment
- `GET /api/bookings/user/:userId` - Get user bookings

## Environment Variables

```
MONGODB_URI=mongodb://localhost:27017/event-planning
JWT_SECRET=your_jwt_secret_key_here
PORT=5000
STRIPE_SECRET_KEY=sk_test_your_stripe_key
STRIPE_PUBLISHABLE_KEY=pk_test_your_stripe_key
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
GOOGLE_MAPS_API_KEY=your_google_maps_key
```

## Future Enhancements

- Video gallery integration
- Real-time chat between customers and providers
- Advanced analytics dashboard
- Mobile app (React Native)
- Email/SMS notifications
- Wishlist functionality
- Recommendation engine
- Virtual venue tours

## License

MIT
