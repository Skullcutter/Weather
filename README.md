## Introduction

Classy Weather is a **demo learning project** created to explore and practice key React concepts such as class components, state management, lifecycle methods, event handling, and conditional rendering.

The app allows users to enter a location, fetches its coordinates using a geocoding API, and then retrieves the daily weather forecast for that location. Weather details such as temperature and conditions are displayed with corresponding icons, making the interface both informative and visually engaging.

This project serves as a practical exercise for understanding how to work with external APIs, manage asynchronous operations in React, and build clean, modular components.

## How It Works

1. User enters a **location name**.

2. The app calls the **Open-Meteo Geocoding API** to find coordinates and timezone.

3. Using the returned coordinates, it fetches a **daily weather forecast**.

4. The forecast is displayed as a list of days with icons, temperature ranges, and "Today" label for the current day.

## 🌟 Features

- **Real-time Weather Data** — Fetches live weather forecasts for any searched location using the [Open-Meteo API](https://open-meteo.com/).

- **Geocoding Integration** — Automatically retrieves latitude, longitude, and timezone from the location input.

- **Daily Forecast View** — Displays a list of upcoming days with max/min temperatures.

- **Weather Icons** — Uses emoji-style icons mapped to WMO weather codes for quick visual recognition.

- **Today Highlight** — Marks the current day's forecast clearly.

- **Local Storage Support** — Saves the last searched location for persistence across reloads (in `App.js` version).

## 🛠️ Tech Stack

- **React** (Class Components + Lifecycle Methods)
- **CSS** for styling
- **Open-Meteo API** for geocoding and weather data
- **JavaScript (ES6+)** features including `fetch`, async/await, destructuring, and array methods.

## 📁 Project Structure

```
/src
  ├─ App.js        # Main app logic with search, API calls, and state handling
  ├─ App-v1.js     # Earlier version with manual 'Get Weather' button
  ├─ Counter.js    # Small counter component (date offset demo)
  ├─ index.js      # Entry point rendering <App />
  ├─ index.css     # Styling for the app
  ├─ starter.js    # Base starter code (API fetch logic without UI)
```

## 🚀 Installation & Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```
2. **Install dependencies**:
   ```bash
   npm install
   ```
3. **Run the app**:
   ```bash
   npm start
   ```
4. Open `http://localhost:3000` in your browser.

## 👨‍💻 Learning

- Using **class components** and managing state with `this.setState()`.

- React **lifecycle methods** (`componentDidMount`, `componentDidUpdate`, `componentWillUnmount`).

- **Fetching data from APIs** and handling async/await in React.

- Passing props between components (`Weather` → `Day`).

- Mapping **API data** to UI elements and rendering lists with `key` props.

- Basic **local storage integration** for persisting user input.

## 🤝 Contributions

Contributions are welcome!

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit changes and push:
   ```bash
   git push origin feature/your-feature-name
   ```
4. Open a Pull Request describing your changes.
