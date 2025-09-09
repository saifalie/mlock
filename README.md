# MLock - Smart Locker Booking System

MLock is a locker booking platform that allows users to find, book, and manage locker stations through a mobile application.

## Features

- Locker booking and management
- Location-based station finding
- Firebase authentication with Google Sign-In
- Razorpay payment integration
- Push notifications
- Admin dashboard
- Real-time locker status updates

## Tech Stack

### Mobile App (Flutter)
- Flutter 3.7+
- BLoC state management
- Firebase Auth
- Google Maps
- Razorpay payments
- Secure storage

### Backend (Node.js)
- Express.js with TypeScript
- MongoDB with Mongoose
- Firebase Admin SDK
- Socket.IO
- MQTT
- AdminJS dashboard

## Installation

### Backend Setup

1. Clone and install dependencies:

```bash
git clone <repository-url>
cd backend
npm install
```

2. Create `.env` file:

```env
PORT=3000
MONGODB_URI=mongodb://localhost:27017/mlock
JWT_SECRET=your_jwt_secret
FIREBASE_PROJECT_ID=your_firebase_project_id
RAZORPAY_KEY_ID=your_razorpay_key
RAZORPAY_SECRET=your_razorpay_secret
```

3. Start server:

```bash
npm run dev
```

### Mobile App Setup

1. Install Flutter dependencies:

```bash
cd fontend
flutter pub get
```

2. Create `.env` file:

```env
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
API_BASE_URL=http://localhost:7000/api
GOOGLE_MAPS_API_KEY=your_google_maps_key
```

3. Add Firebase configuration files and run:

```bash
flutter run
```

## API Endpoints

- `POST /api/auth/login` - User login
- `POST /api/auth/register` - User registration
- `GET /api/lockers/stations` - Get locker stations
- `POST /api/lockers/book` - Book a locker
- `POST /api/payments/create-order` - Create payment order

## Project Structure

```
mlock/
├── mlock-server/          # Node.js backend
│   ├── src/
│   └── package.json
└── mlock_flutter/         # Flutter app
    ├── lib/
    └── pubspec.yaml
```

## Deployment

### Backend

```bash
npm run build
npm run start
```

### Mobile App

```bash
flutter build apk --release
```

## Author

Saif Ali Shaikh
