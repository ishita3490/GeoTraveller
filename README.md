

```markdown:README.md
# GeoTraveller - Travel Tracking Application

GeoTraveller is a web application that helps users track and visualize their travel experiences across the world. Users can mark cities they've visited on an interactive map, add notes about their trips, and maintain a digital travel diary.

## Features

- 🗺️ Interactive world map using Leaflet
- 📍 Click-to-add city markers
- 🌍 City and country list views
- 📝 Add notes and dates for each visited location
- 🔐 User authentication system
- 📱 Responsive design
- 🌐 Real-time geolocation support

## Tech Stack

### Frontend
- React 18
- React Router v6
- Leaflet for maps
- CSS Modules for styling
- React DatePicker
- Vite as build tool

### Backend
- Node.js
- Express
- MongoDB with Mongoose
- CORS support
- Environment variables with dotenv

## Getting Started

### Prerequisites
- Node.js
- MongoDB
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone <repository-url>
```

2. Install Frontend dependencies
```bash
cd Frontend
npm install
```

3. Install Backend dependencies
```bash
cd Backend
npm install
```

4. Create `.env` file in Backend directory with:
```env
MONGO_URL=your_mongodb_connection_string
PORT=4000
```

5. Create `.env` file in Frontend directory with:
```env
VITE_BASE_URL=/api
```

### Running the Application

1. Start the Backend server:
```bash
cd Backend
npm start
```

2. Start the Frontend development server:
```bash
cd Frontend
npm run dev
```

## Project Structure

```
├── Frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── contexts/
│   │   ├── hooks/
│   │   ├── pages/
│   │   └── App.jsx
│   └── package.json
│
└── Backend/
    ├── models/
    ├── routes/
    ├── index.js
    └── package.json
```

## Features in Detail

### Map Functionality
- Interactive map with clickable points
- Custom markers for visited cities
- Popup information for each location
- Current location detection

### City Management
- Add new cities with details
- View city information
- Delete visited cities
- Add travel dates and notes

### User Interface
- Clean and intuitive design
- Dark theme
- Responsive layout
- Loading states and error handling

### Authentication
- User login system
- Protected routes
- Session management

### Data Management
- MongoDB database integration
- RESTful API endpoints
- Real-time data updates

## Available Scripts

### Frontend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run lint` - Run ESLint
- `npm run preview` - Preview production build

### Backend
- `npm start` - Start the server
- `npm run build` - Install dependencies

## API Endpoints

- `GET /api/cities` - Get all cities
- `POST /api/cities` - Add a new city
- `DELETE /api/cities/:id` - Delete a city
- `GET /api/cities/:id` - Get city details
