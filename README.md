Here's the English version of your README file for your public transport ETA system project:

---

# Public Transport ETA System

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

A comprehensive web application providing real-time arrival information for various public transport services (buses, MTR, minibuses) and weather forecasts in Hong Kong.

## Key Features

- 🚌 **Bus ETA**: Supports KMB, Citybus, NWFB, and Long Win buses with route details and stop information
- 🚇 **MTR ETA**: Real-time arrival times for all MTR lines with station-specific data
- 🚐 **Minibus ETA**: Green minibus real-time information with regional search
- ☀️ **Weather Forecast**: 7-day Hong Kong weather forecast and warnings from HKO
- 📱 **Responsive Design**: Mobile-friendly interface for all screen sizes
- ⚡ **Real-time Data**: Fetches latest transport and weather information
- 🔄 **Auto Refresh**: Automatic updates for arrival times (MTR)

## Technical Architecture

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **UI Framework**: Font Awesome icons for consistent UI
- **API Integration**: Connects with multiple official transport APIs
  - KMB/LWB: data.etabus.gov.hk
  - Citybus/NWFB: rt.data.gov.hk
  - MTR: rt.data.gov.hk
  - Minibus: data.etagmb.gov.hk
  - Weather: data.weather.gov.hk
- **Modular Design**: ES6 modules for better code organization
- **Error Handling**: Comprehensive error handling and user feedback

## File Structure

```
public-transport-eta/
├── css/
│   ├── style.css          # Main stylesheet
│   └── gmb-eta.css        # Minibus-specific styles
├── js/
│   ├── api/               # API handlers
│   │   ├── bus-api.js     # Bus API service
│   │   ├── mtr-api.js     # MTR API service
│   │   ├── gmb-api.js     # Minibus API service
│   │   └── weather-api.js # Weather API service
│   ├── bus-app.js         # Bus search page logic
│   ├── bus-results.js     # Bus results page logic
│   ├── mtr-app.js         # MTR search page logic
│   ├── mtr-results.js     # MTR results page logic
│   ├── gmb-eta.js         # Minibus page logic
│   └── weather-ui.js      # Weather page logic
├── index.html             # Main entry page
├── bus-index.html         # Bus search page
├── bus-results.html       # Bus results page
├── mtr-index.html         # MTR search page
├── mtr-results.html       # MTR results page
├── gmb-eta.html           # Minibus page
└── weather-index.html     # Weather page
```

## Installation & Usage

1. **Clone repository**:
   ```bash
   git clone https://github.com/your-username/public-transport-eta.git
   ```

2. **Enter project directory**:
   ```bash
   cd public-transport-eta
   ```

3. **Launch application**:
   - Open `index.html` directly in a browser
   - Or use a local server (like VS Code's Live Server extension)

## API Documentation

### Bus API (`bus-api.js`)
- `getRouteDetails(company, route, direction)`: Get full route information including stops
- `getStopArrivals(company, stopId, route)`: Get arrival times for a specific stop

### MTR API (`mtr-api.js`)
- `getMtrArrivalTimes(lineCode, stationCode)`: Get real-time arrival data for MTR stations
- `getStationsForLine(lineCode)`: Get all stations for a specific MTR line

### Minibus API (`gmb-api.js`)
- `getRouteList(region)`: Get minibus routes by region
- `getRouteStopETA(routeId, routeSeq, stopSeq)`: Get arrival times for minibus stops

### Weather API (`weather-api.js`)
- `getForecast()`: Get 7-day weather forecast
- `getWarnings()`: Get current weather warnings

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the project
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## License

This project is licensed under the [MIT License](LICENSE).

## Screenshots

![Homepage](screenshots/home.png)
![Bus Search](screenshots/bus.png)
![MTR Search](screenshots/mtr.png)
![Minibus Search](screenshots/gmb.png)
![Weather Forecast](screenshots/weather.png)

---

**Note**: Remember to replace placeholder image links and GitHub repository URL when actually using. You may want to add more specific documentation about API usage or deployment instructions if needed.
