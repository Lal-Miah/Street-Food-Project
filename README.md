# StreetFood Connect

A comprehensive web-based platform designed to bridge the gap between street food vendors and raw material suppliers across India. This project addresses the critical challenge of sourcing quality ingredients for street food businesses while providing suppliers with a reliable customer base.

## Project Overview

StreetFood Connect emerged from the recognition that street food vendors in India often struggle with inconsistent supply chains, quality issues, and limited access to reliable suppliers. Conversely, suppliers face challenges in reaching their target market efficiently. This platform serves as a digital marketplace that connects these two essential parts of the food ecosystem.

## Core Functionality

### For Street Food Vendors

**Supplier Discovery and Comparison**
- Browse an extensive database of verified suppliers
- Compare prices, quality ratings, and delivery options
- Filter suppliers by location, material type, and business requirements
- Access detailed supplier profiles with ratings and reviews

**Order Management**
- Place orders with specific quantity requirements
- Track order status in real-time
- Maintain order history for business analysis
- Receive notifications for order updates

**Payment Integration**
- Secure UPI payment processing
- QR code generation for instant payments
- Manual UPI payment options
- Comprehensive payment tracking and receipts

**Business Analytics**
- Monitor spending patterns and trends
- Analyze supplier performance
- Track order frequency and costs
- Generate insights for business optimization

### For Raw Material Suppliers

**Inventory Management**
- Add and update product catalogs
- Set pricing and availability
- Manage stock levels efficiently
- Categorize products for better organization

**Order Processing**
- Receive and review incoming orders
- Accept or reject orders with reasons
- Update order status in real-time
- Communicate with customers directly

**Customer Relationship Management**
- View customer profiles and order history
- Analyze customer behavior and preferences
- Track customer satisfaction through ratings
- Identify top customers and their requirements

**Performance Analytics**
- Monitor sales performance and trends
- Analyze customer acquisition and retention
- Track revenue and order metrics
- Generate business insights for growth

## Technical Architecture

### Frontend Technologies
- **React 18**: Modern component-based architecture
- **Material-UI (MUI)**: Professional design system with dark theme
- **React Router DOM**: Client-side routing for seamless navigation
- **React Query**: Efficient data fetching and caching
- **React Hook Form**: Form validation and management
- **React Hot Toast**: User-friendly notifications

### Backend Infrastructure
- **Firebase Authentication**: Secure user authentication and authorization
- **Firestore Database**: NoSQL database for real-time data management
- **Firebase Hosting**: Fast and reliable application hosting
- **Firebase Security Rules**: Data protection and access control

### Key Features
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Real-time Updates**: Live data synchronization across all users
- **Role-based Access Control**: Separate interfaces for vendors and suppliers
- **Payment Processing**: Integrated UPI payment system
- **Data Analytics**: Comprehensive business intelligence tools

## Database Structure

The application uses a well-structured Firestore database with the following collections:

- **users**: Vendor and supplier profiles with role-based data
- **inventory**: Product catalogs with pricing and availability
- **orders**: Transaction records with status tracking
- **reviews**: Customer feedback and supplier ratings
- **analytics**: Business metrics and performance data

## Installation and Setup

### Prerequisites
- Node.js (version 16 or higher)
- npm or yarn package manager
- Firebase project with Firestore enabled

### Local Development Setup

1. Clone the repository:
```bash
git clone https://github.com/your-username/streetfood-connect.git
cd streetfood-connect
```

2. Install dependencies:
```bash
npm install
```

3. Configure Firebase:
   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com)
   - Enable Authentication, Firestore, and Hosting
   - Update `src/config/firebase.js` with your project credentials

4. Set up Firestore indexes:
   - Navigate to Firestore > Indexes in Firebase Console
   - Create composite indexes for orders collection:
     - `vendorId` + `createdAt` (Ascending)
     - `supplierId` + `createdAt` (Ascending)
   - Create composite indexes for reviews collection:
     - `supplierId` + `createdAt` (Ascending)

5. Start development server:
```bash
npm run dev
```

### Production Deployment

1. Build the application:
```bash
npm run build
```

2. Deploy to Firebase:
```bash
firebase deploy
```

## Usage Guide

### Vendor Registration and Onboarding
1. Register with business details, location, and contact information
2. Complete profile verification process
3. Start browsing suppliers and comparing offerings
4. Place first order and complete payment
5. Access analytics and business insights

### Supplier Registration and Setup
1. Register with business credentials and verification documents
2. Set up inventory catalog with pricing and descriptions
3. Configure delivery options and service areas
4. Start receiving and processing orders
5. Monitor performance through analytics dashboard

## Business Model

StreetFood Connect operates on a commission-based model where suppliers pay a small percentage of successful transactions. This ensures the platform remains sustainable while providing value to both vendors and suppliers.

## Security and Privacy

- All user data is encrypted and stored securely in Firebase
- Authentication uses Firebase's industry-standard security protocols
- Payment information is processed through secure UPI gateways
- Regular security audits and updates are implemented

## Performance Optimization

- Lazy loading for improved initial load times
- Image optimization and compression
- Efficient database queries with proper indexing
- Caching strategies for frequently accessed data
- Progressive Web App features for offline functionality

## Future Enhancements

- Mobile application development for iOS and Android
- Advanced analytics with machine learning insights
- Integration with logistics providers for delivery tracking
- Multi-language support for regional markets
- Advanced payment options including digital wallets
- Supplier verification and certification programs

## Contributing

This project welcomes contributions from developers interested in improving the street food ecosystem. Please read our contributing guidelines and submit pull requests for review.

## Support and Documentation

For technical support or questions about the platform, please refer to the documentation or contact the development team through the project repository.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

Special thanks to the street food vendors and suppliers who provided valuable insights during the development process. Their feedback was instrumental in creating a platform that truly serves the needs of the community.

---

*StreetFood Connect - Connecting the heart of India's street food culture with quality suppliers.*# Street-Food-Project
