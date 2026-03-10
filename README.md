# Zerodha Clone

A full-stack web application that replicates the functionality of Zerodha, India's largest discount broker for stock trading.

## Features

- **Dashboard**: Comprehensive trading dashboard with real-time data
  - Holdings: View your current stock holdings with P&L
  - Positions: Track open positions
  - Orders: Manage buy/sell orders
  - Watchlist: Monitor favorite stocks
  - Funds: Check account balance and funds
  - Charts: Visual representation of data with doughnut and vertical graphs

- **Landing Page**: Marketing website with information about products, pricing, support, and account opening

- **Authentication**: User authentication system

## Tech Stack

### Backend
- **Node.js** with **Express.js** for server-side logic
- **MongoDB** with **Mongoose** for data storage
- **Passport.js** for authentication
- **CORS** and **Body-parser** for handling requests

### Dashboard (Trading Interface)
- **React** for frontend framework
- **Material-UI** for UI components
- **Chart.js** and **React-Chartjs-2** for data visualization
- **Axios** for API calls
- **React Router** for navigation

### Frontend (Landing Page)
- **React** for frontend framework
- **React Router** for navigation
- **Axios** for API calls

## Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd zerodha-clone
   ```

2. **Set up the Backend:**
   ```bash
   cd backend
   npm install
   ```
   - Create a `.env` file in the backend directory with:
     ```
     MONGO_URL=your_mongodb_connection_string
     PORT=3002
     ```
   - Start the backend server:
     ```bash
     npm start
     ```

3. **Set up the Dashboard:**
   ```bash
   cd ../dashboard
   npm install
   npm start
   ```
   The dashboard will run on `http://localhost:3000`

4. **Set up the Frontend (Landing Page):**
   ```bash
   cd ../frontend
   npm install
   npm start
   ```
   The landing page will run on `http://localhost:3001`

## Usage

1. Visit the landing page to learn about the platform
2. Sign up for an account
3. Access the dashboard to start trading
4. View holdings, positions, and place orders
5. Monitor your portfolio with charts and analytics

## API Endpoints

The backend provides RESTful APIs for:
- `/holdings` - Manage stock holdings
- `/positions` - Handle trading positions
- `/orders` - Process buy/sell orders

## Project Structure

```
zerodha-clone/
├── backend/          # Node.js/Express server
│   ├── model/        # Database models
│   ├── schemas/      # Mongoose schemas
│   └── index.js      # Main server file
├── dashboard/        # React trading dashboard
│   ├── src/
│   │   ├── components/  # React components
│   │   └── data/        # Static data
│   └── public/
├── frontend/         # React landing page
│   ├── src/
│   │   └── landing_page/  # Landing page components
│   └── public/
└── README.md
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is for educational purposes only and is not affiliated with Zerodha.

## Author

Vishal Pandhare
