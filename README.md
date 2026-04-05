# Zerodha Clone - Trading Platform

A full-stack trading platform inspired by Zerodha, featuring a marketing landing page and a comprehensive trading dashboard with real-time portfolio management.

## Features

### Landing Page
- **Modern UI/UX** with responsive design
- **Hero Section** with compelling call-to-action
- **Awards & Recognition** showcase
- **Real-time Statistics** display
- **Pricing Plans** comparison
- **Educational Resources** section
- **User Authentication** (Signup/Login)
- **Support & Help** pages

### Trading Dashboard
- **Portfolio Overview** with total value and P&L
- **Holdings Management** - View all stock holdings
- **Positions Tracking** - Monitor open/closed positions
- **Order Placement** - Buy/sell stocks with real-time pricing
- **Interactive Charts** using Chart.js
- **Material-UI Components** for professional interface
- **Responsive Design** for desktop and mobile

### Backend API
- **RESTful API** built with Express.js
- **MongoDB Integration** with Mongoose ODM
- **Authentication** using Passport.js
- **CORS Support** for cross-origin requests
- **Environment Configuration** with dotenv

## Architecture

```
Zerodha/
├── backend/                 # Node.js API Server
│   ├── index.js            # Main server file
│   ├── model/              # Mongoose models
│   │   ├── HoldingsModel.js
│   │   ├── PositionsModel.js
│   │   └── OrdersModel.js
│   ├── schemas/            # MongoDB schemas
│   └── package.json
├── frontend/               # React Landing Page
│   ├── src/
│   │   ├── landing_page/  # Landing page components
│   │   └── index.js
│   └── package.json
└── dashboard/             # React Trading Dashboard
    ├── src/
    │   ├── components/    # Dashboard components
    │   └── index.js
    └── package.json
```

## Tech Stack

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM for MongoDB
- **Passport.js** - Authentication middleware
- **CORS** - Cross-origin resource sharing
- **dotenv** - Environment variables

### Frontend (Landing Page)
- **React 18** - UI library
- **React Router** - Client-side routing
- **CSS3** - Styling

### Dashboard
- **React 18** - UI library
- **Material-UI (MUI)** - Component library
- **Chart.js** - Data visualization
- **React Chart.js 2** - React wrapper for Chart.js
- **Axios** - HTTP client
- **React Router** - Client-side routing

## Prerequisites

- Node.js (v14 or higher)
- MongoDB (local or cloud instance)
- npm or yarn package manager

## Getting Started

### 1. Clone the repository
```bash
git clone <repository-url>
cd Zerodha
```

### 2. Install Dependencies

#### Backend
```bash
cd backend
npm install
```

#### Frontend (Landing Page)
```bash
cd ../frontend
npm install
```

#### Dashboard
```bash
cd ../dashboard
npm install
```

### 3. Environment Setup

Create a `.env` file in the `backend` directory:
```env
PORT=3002
MONGO_URL=mongodb://localhost:27017/zerodha
```

### 4. Database Setup

Ensure MongoDB is running and create a database named `zerodha`. The application will automatically create the necessary collections.

### 5. Start the Applications

#### Start Backend Server
```bash
cd backend
npm start
```
The API server will run on `http://localhost:3002`

#### Start Frontend (Landing Page)
```bash
cd frontend
npm start
```
The landing page will run on `http://localhost:3000`

#### Start Dashboard
```bash
cd dashboard
npm start
```
The dashboard will run on `http://localhost:3001`

## API Endpoints

### Holdings
- `GET /allHoldings` - Get all user holdings
- `GET /addHoldings` - (Development) Add sample holdings

### Positions
- `GET /allPositions` - Get all user positions
- `GET /addPositions` - (Development) Add sample positions

### Orders
- `POST /newOrder` - Create a new order

## Usage

1. **Visit the Landing Page** at `http://localhost:3000`
   - Explore features and pricing
   - Sign up for an account

2. **Access the Dashboard** at `http://localhost:3001`
   - View your portfolio overview
   - Track holdings and positions
   - Place buy/sell orders
   - Monitor performance with charts

## Development

### Adding New Features
1. Backend: Add new routes in `backend/index.js`
2. Frontend: Create components in respective `src` directories
3. Dashboard: Add new components in `dashboard/src/components`

### Database Models
- **Holdings**: User's long-term stock holdings
- **Positions**: Active trading positions
- **Orders**: Buy/sell order history

