# 🌤️ Weather App

A modern, responsive weather forecasting application built with React.js and OpenWeatherMap API. Get real-time weather updates, location-based forecasts, and a comprehensive 5-day weather outlook.

## ✨ Features

- **Real-time Weather Updates**: Get current weather conditions for any location
- **Location-based Forecasts**: Automatically detect your location or search for any city
- **5-Day Weather Outlook**: Comprehensive daily weather predictions
- **Responsive Design**: Beautiful UI that works on all devices
- **Geolocation Support**: Automatically get weather for your current location
- **Search Functionality**: Search for cities, countries, or coordinates
- **Detailed Weather Metrics**: Temperature, humidity, wind speed, pressure, and visibility
- **Weather Icons**: Intuitive emoji-based weather representations
- **Performance Optimized**: Efficient API requests and caching

## 🚀 Getting Started

### Prerequisites

- Node.js (version 14 or higher)
- npm or yarn package manager
- OpenWeatherMap API key

### Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd weather-app
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Get OpenWeatherMap API Key**
   - Visit [OpenWeatherMap](https://openweathermap.org/)
   - Sign up for a free account
   - Get your API key from the dashboard
   - Replace `YOUR_API_KEY_HERE` in `src/services/weatherService.js`

4. **Start the development server**
   ```bash
   npm start
   # or
   yarn start
   ```

5. **Open your browser**
   - Navigate to `http://localhost:3000`
   - The app will automatically open in your default browser

## 🔧 Configuration

### API Key Setup

1. Open `src/services/weatherService.js`
2. Replace `YOUR_API_KEY_HERE` with your actual OpenWeatherMap API key:
   ```javascript
   const API_KEY = 'your_actual_api_key_here';
   ```

### Environment Variables (Optional)

For production, you can use environment variables:

1. Create a `.env` file in the root directory
2. Add your API key:
   ```
   REACT_APP_OPENWEATHER_API_KEY=your_api_key_here
   ```
3. Update the service file to use:
   ```javascript
   const API_KEY = process.env.REACT_APP_OPENWEATHER_API_KEY;
   ```

## 📱 Usage

### Current Location
- The app automatically detects your location on first load
- Grant location permissions when prompted

### Search for Weather
- Use the search bar to find weather for any city
- Enter city name, country, or coordinates
- Press Enter or click Search

### Weather Information
- **Current Weather**: Temperature, feels like, humidity, wind, pressure, visibility
- **5-Day Forecast**: Daily predictions with averages
- **Weather Icons**: Visual representation of conditions

## 🏗️ Project Structure

```
src/
├── components/          # React components
│   ├── WeatherSearch.js    # Search interface
│   ├── CurrentWeather.js   # Current weather display
│   └── Forecast.js         # 5-day forecast
├── services/            # API services
│   └── weatherService.js   # OpenWeatherMap API calls
├── utils/               # Utility functions
│   └── weatherIcons.js     # Weather icon mapping
├── App.js              # Main application component
├── App.css             # Application styles
├── index.js            # Application entry point
└── index.css           # Global styles
```

## 🎨 Technologies Used

- **Frontend**: React.js 18
- **Styling**: CSS3 with modern features (Grid, Flexbox, CSS Variables)
- **Icons**: React Icons (Weather Icons)
- **API**: OpenWeatherMap REST API
- **Build Tool**: Create React App
- **Package Manager**: npm/yarn

## 🌐 API Endpoints Used

- **Current Weather**: `/weather` - Get current weather data
- **5-Day Forecast**: `/forecast` - Get 5-day weather forecast
- **Geocoding**: `/geo/1.0/direct` - City search and coordinates

## 📱 Responsive Design

The app is fully responsive and works on:
- Desktop computers
- Tablets
- Mobile phones
- All modern browsers

## 🚀 Deployment

### Build for Production
```bash
npm run build
# or
yarn build
```

### Deploy to Netlify/Vercel
1. Build the project
2. Upload the `build` folder
3. Configure environment variables if needed

### Deploy to GitHub Pages
```bash
npm run deploy
# or
yarn deploy
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [OpenWeatherMap](https://openweathermap.org/) for providing the weather API
- [React Icons](https://react-icons.github.io/react-icons/) for beautiful weather icons
- [Create React App](https://create-react-app.dev/) for the project setup

## 📞 Support

If you encounter any issues or have questions:
- Check the [OpenWeatherMap API documentation](https://openweathermap.org/api)
- Review the console for error messages
- Ensure your API key is correctly configured
- Verify your internet connection

## 🔮 Future Enhancements

- [ ] Dark/Light theme toggle
- [ ] Weather alerts and notifications
- [ ] Historical weather data
- [ ] Weather maps integration
- [ ] Multiple language support
- [ ] Offline functionality
- [ ] Weather widgets
- [ ] Social sharing features

---

**Happy Weather Forecasting! ☀️🌧️❄️**
