# 🌍 WorldWise App

**A Single Page Application that tracks your footsteps using a world map into every city you can think of. Never forget your wonderful experiences, and show your friends how you have wandered the world.**

## 📖 Description

WorldWise is an interactive travel tracking application. It allows you to visually log your adventures on a world map, add details about each city you visit, and keep a personal journal of your experiences. The app is built with modern web technologies for a fast, responsive, and engaging user experience.

## 🛠️ Tech Stack & Tools

This project leverages a modern and efficient frontend stack:

- **React**: A JavaScript library for building a dynamic and component-based user interface.
- **Vite**: A next-generation, fast build tool and development server that provides an excellent developer experience with features like Hot Module Replacement (HMR).
- **Leaflet**: A leading open-source JavaScript library for interactive maps. It's lightweight, mobile-friendly, and powers the core map functionality.
- **React-Leaflet**: A set of React components that provides an elegant way to use Leaflet maps within a React application.
- **CSS Modules / Styled Components**: Used for component-scoped styling to create a maintainable and modular look and feel.


## ✨ Key Features

### 1. Interactive World Map
- A central, interactive map built with Leaflet where you can view all your visited cities as markers
- Zoom and pan functionality to explore different regions

### 2. Add a New City via the Map
- Click on any city location on the map to open an "Add New City" form

### 3. City Details & Notes Management
- For each visited city, add detailed notes about your experience

### 4. Visit Date Logging
- Record the exact date you visited each city

### 5. City List & Management
- Sidebar displays all logged cities in a clean, organized list
- Select any city to view its details on the map
- Delete functionality to remove cities from your travel log
- Integration with the map for visual feedback

### 6. Geolocation Features
- Use your current location to quickly add cities you're visiting
- Reverse geocoding to convert coordinates to city names
- Automatic country detection and flag display

### 7. Data Persistence
- Cities data is stored and managed using React Context
- State persists during the session
- Ready for backend integration for permanent storage

## 📁 Project Structure
```
WorldWise-App/
├── data/
│   └── cities.json
│
├── public/
│
├── src/
│   ├── components/
│   │   ├── AppNav/
│   │   ├── BackButton/
│   │   ├── Button/
│   │   ├── City/
│   │   ├── CityItem/
│   │   ├── CityList/
│   │   ├── CountryItem/
│   │   ├── CountryList/
│   │   ├── Form/
│   │   ├── Logo/
│   │   ├── Map/
│   │   ├── Message/
│   │   ├── PageNav/
│   │   ├── Sidebar/
│   │   ├── Spinner/
│   │   ├── SpinnerFullPage/
│   │   └── User/
│   │
│   ├── contexts/
│   │   ├── CitiesContext.jsx
│   │   └── FakeAuthContext.jsx
│   │
│   ├── hooks/
│   │   ├── useGeolocation.js
│   │   └── useUrlPosition.js
│   │
│   ├── pages/
│   │   ├── AppLayout/
│   │   ├── HomePage/
│   │   ├── Login/
│   │   ├── PageNotFound/
│   │   ├── Pricing/
│   │   ├── Product/
│   │   └── ProtectedRoute/
│   │
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
│
├── .gitignore
├── eslint.config.js
├── index.html
├── package-lock.json
├── package.json
├── README.md
└── vite.config.js
```
## 🚀 Getting Started (Development)

Follow these steps to run the project locally:
### 1. Clone the repository
```bash
git clone https://github.com/ayabedair/WorldWise-App.git
cd WorldWise-App
```
### 2. Install dependencies

```bash
npm install
```
### 3. Start the development server

```bash
npm run dev
```
The app will now be running on http://localhost:5173 (or a similar port).

### 4. Start the (fake) API server
```bash
npm run server
```
The server will now be running on http://localhost:8000/cities (or edit package.json file).
