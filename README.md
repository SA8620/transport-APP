# Public Transport ETA System

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

A web application providing real-time arrival information for various public transport services and weather forecasts in Hong Kong.

## Key Features

- 🚌 **Bus ETA**: Supports KMB, Citybus, NWFB, and Long Win buses
- 🚇 **MTR ETA**: Real-time arrival times for all MTR lines
- 🚐 **Minibus ETA**: Green minibus real-time information
- ☀️ **Weather Forecast**: 7-day Hong Kong weather forecast and warnings
- 📱 **Responsive Design**: Adapts to various screen sizes
- ⚡ **Real-time Data**: Fetches latest transport and weather information

## Technical Architecture

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **UI Framework**: Font Awesome icons
- **API Integration**: Connects with multiple public transport APIs
- **Modular Design**: Developed with modular JavaScript

## File Structure

```
public-transport-eta/
├── css/
│   ├── style.css          # Main stylesheet
│   └── gmb-eta.css        # Minibus-specific styles
├── js/
│   ├── bus-app.js         # Bus search logic
│   ├── bus-results.js     # Bus results page logic
│   ├── mtr-app.js         # MTR search logic
│   ├── mtr-results.js     # MTR results page logic
│   ├── gmb-api.js         # Minibus API handler
│   ├── gmb-eta.js         # Minibus search logic
│   ├── weather-api.js     # Weather API handler
│   └── weather-ui.js      # Weather UI logic
├── index.html             # Main entry page
├── bus-index.html         # Bus search page
├── bus-results.html       # Bus results page
├── mtr-index.html         # MTR search page
├── mtr-results.html       # MTR results page
├── gmb-eta.html           # Minibus search page
└── weather-index.html     # Weather forecast page
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

## Contributing

Pull requests and issue reports are welcome. Main contribution steps:

1. Fork the project
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## License

This project is licensed under the [MIT License](LICENSE).

## Preview Screenshots

![Homepage](screenshots/home.png)
![Bus Search](screenshots/bus.png)
![MTR Search](screenshots/mtr.png)
![Minibus Search](screenshots/gmb.png)
![Weather Forecast](screenshots/weather.png)
---

**Note**: Replace placeholder image links and GitHub repository URL when actually using. You may add more project-specific details such as API documentation links, deployment instructions, etc.
