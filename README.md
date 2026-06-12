# Zepto E-Commerce App

A modern e-commerce application built with Flutter, Firebase, and PHP.

## Project Overview

This is a full-stack e-commerce application inspired by Zepto's quick commerce model.

### Tech Stack

- **Frontend**: Flutter (Mobile App)
- **Authentication**: Firebase Authentication
- **Backend**: PHP with REST API
- **Database**: MySQL

## Project Structure

```
zepto-ecommerce-app/
├── flutter_app/              # Flutter mobile application
│   ├── lib/
│   ├── assets/
│   ├── pubspec.yaml
│   └── README.md
├── backend/                  # PHP backend API
│   ├── config/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── database/
│   └── README.md
├── docs/                     # Documentation
│   ├── FLUTTER_SETUP.md
│   ├── BACKEND_SETUP.md
│   └── API_DOCS.md
├── .gitignore
└── README.md
```

## Features (Planned)

### User Management
- User registration & login (Firebase Auth)
- Profile management
- Address management
- Favorites/Wishlist

### Products
- Product catalog
- Search & filters
- Categories
- Product details
- Ratings & reviews

### Shopping
- Shopping cart
- Order management
- Order tracking
- Order history

### Payments
- Payment gateway integration (Razorpay/PayPal)
- Multiple payment methods

### Delivery
- Real-time delivery tracking
- Delivery partner assignment
- Notifications

## Getting Started

### Prerequisites

- Flutter SDK (3.0+)
- PHP 7.4+
- MySQL 5.7+
- Node.js & npm
- Git

### Quick Start

#### Frontend Setup
```bash
cd flutter_app
flutter pub get
flutter run
```

#### Backend Setup
```bash
cd backend
composer install
cp .env.example .env
php -S localhost:8000 -t public
```

## Documentation

- [Flutter Setup Guide](./docs/FLUTTER_SETUP.md)
- [PHP Backend Guide](./docs/BACKEND_SETUP.md)
- [API Documentation](./docs/API_DOCS.md)

## Contributing

1. Create a feature branch (`git checkout -b feature/AmazingFeature`)
2. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
3. Push to the branch (`git push origin feature/AmazingFeature`)
4. Open a Pull Request

## Project Timeline

- **Phase 1**: Basic auth & product listing
- **Phase 2**: Cart & checkout
- **Phase 3**: Payment integration
- **Phase 4**: Order tracking & delivery
- **Phase 5**: Admin panel

## License

This project is licensed under the MIT License

## Author

Developed by shivamp03
