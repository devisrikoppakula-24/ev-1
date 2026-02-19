# User Roles & System Overview (490 Words)

## Two Login Systems

**Customer Login:** Customers register with name, email, mobile, and password to plan events. After login, they provide event location and browse venues/services.

**Venue Owner/Service Provider Login:** Venues and service providers manage listings, profiles, and bookings through their dashboards.

---

## Customer Module

**Registration & Location Setup**
Customers register with basic details and specify event location (city/pincode) for tailored recommendations.

**Venue Search**
Location-based results display venue cards featuring:
- Venue name and gallery images
- Ratings, exact location (with Google Maps), pricing
- Seating capacity, available dates, contact info
- Catering options and event gallery

**Detailed Venue Page**
Includes full descriptions, rules, facilities (parking, Wi-Fi), catering details, and event gallery.

**Venue Booking**
Customers select event date and type (marriage, birthday, engagement, corporate). System verifies real-time availability and confirms booking.

**Service Selection**
After booking, customers add complementary services:
- Catering, Culturals/Dance Teams, Event Managers
- Decorations, Priests, Makeup Artists

**Service Provider Details**
Each provider shows profile, ratings, portfolio, pricing packages, date/location availability, and contact options. Filters allow search by location, date, price, and ratings.

**Booking Summary**
Final page displays booked venue, selected services, total cost breakdown, payment integration (Stripe/PayPal), and confirmation notifications.

---

## Venue Owner Dashboard

- Upload venue details: name, location, images, pricing, capacity, availability calendar
- View bookings with customer name, event date, type, and status
- Manage profile and access booking analytics

---

## Service Provider Dashboard

- Create professional profile with service descriptions, work portfolio, pricing packages
- Set availability dates and service locations
- View and accept/reject booking requests
- Track performance metrics and ratings

---

## Admin Module

- Approve registrations for venues and providers
- Manage user accounts and suspensions
- Monitor bookings and transactions
- Handle complaints and disputes
- Manage platform content and featured listings

---

## Technology Stack

**Frontend:** React.js (dynamic UI, search, booking flows)
**Backend:** Node.js + Express.js (APIs and logic)
**Database:** MongoDB (users, venues, services, bookings)
**Authentication:** JWT (secure login)
**Storage:** Cloudinary/Firebase (galleries and portfolios)
**Location:** Google Maps API (location-based search)
**Payment:** Stripe or PayPal API
**Hosting:** AWS, Heroku, or Vercel

---

## Key Features

✓ **Location-Based Search** – Filters by user-specified location
✓ **Integrated Booking** – Seamless venue-to-services flow
✓ **Real-Time Availability** – Prevents scheduling conflicts
✓ **Ratings & Reviews** – Community-driven trust building
✓ **Scalable Design** – Supports multiple event types and providers
✓ **Mobile-Responsive** – Works across all devices

---

This full-stack web application provides an end-to-end event planning solution connecting customers with venues and service providers efficiently.
