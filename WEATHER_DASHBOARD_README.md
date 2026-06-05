# Weather Dashboard

A real-time weather dashboard powered by OpenWeatherMap API. Get current weather, hourly forecasts, and 5-day predictions for any city worldwide.

## 🌟 Features

- ✅ **Current Weather** - Real-time temperature, humidity, wind, and pressure
- ⏰ **Hourly Forecast** - 24-hour weather predictions
- 📅 **5-Day Forecast** - Extended weather outlook
- 🌍 **Global Coverage** - Search for any city in the world
- 🔄 **Unit Toggle** - Switch between Celsius/Fahrenheit and Km/h/mph
- 📍 **Smart Search** - Auto-complete suggestions and popular cities
- 🎨 **Beautiful Design** - Modern gradient UI with glass-morphism
- 📱 **Responsive** - Works on all devices (mobile, tablet, desktop)
- ⚡ **Real-time Updates** - Live weather data from OpenWeatherMap

## 🚀 Quick Start

### Prerequisites

- Node.js 18+
- OpenWeatherMap API Key (get it free at https://openweathermap.org/api)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/infotjarax-cloud/nextjs-boilerplate.git
cd nextjs-boilerplate
```

2. Install dependencies:
```bash
npm install
```

3. Create `.env.local` file:
```bash
NEXT_PUBLIC_OPENWEATHER_API_KEY=your_api_key_here
```

4. Run the development server:
```bash
npm run dev
```

5. Open [http://localhost:3000/weather](http://localhost:3000/weather) in your browser

## 📁 Project Structure

```
src/
├── app/
│   ├── weather/
│   │   ├── page.tsx          # Main weather dashboard
│   │   └── layout.tsx        # Weather layout with metadata
│   └── weather-landing.tsx   # Landing page (info)
├── components/
│   ├── SearchCity.tsx        # City search with suggestions
│   ├── WeatherCard.tsx       # Current weather display
│   ├── HourlyForecast.tsx    # Hourly forecast cards
│   ├── DetailedForecast.tsx  # 5-day forecast grid
│   └── LoadingSpinner.tsx    # Loading animation
```

## 🎨 Data Displayed

### Current Weather
- Temperature (with feels-like)
- Weather condition & description
- Humidity percentage
- Atmospheric pressure
- Wind speed & gust
- Visibility distance
- UV Index & cloud cover
- Sunrise & sunset times
- Precipitation (if any)

### Hourly Forecast
- Time for each hour
- Temperature prediction
- Weather condition
- Wind speed
- Precipitation chance

### 5-Day Forecast
- Date & day of week
- High/Low temperatures
- Weather condition
- Humidity
- Wind speed
- Precipitation

## 🔐 API Configuration

### Get Your API Key

1. Visit [OpenWeatherMap](https://openweathermap.org/api)
2. Sign up for a free account
3. Go to your API keys section
4. Copy your API key
5. Add it to `.env.local`

### Available Free Tier

The free tier includes:
- Current weather data
- 5-day weather forecast
- Unlimited API calls per second
- Global coverage

## 🛠️ Technologies Used

- **Next.js 16** - React framework
- **React 19** - UI library
- **TypeScript** - Type safety
- **Tailwind CSS 4** - Styling
- **OpenWeatherMap API** - Weather data

## 🎨 Design Features

- **Gradient backgrounds** - Beautiful modern look
- **Glass-morphism** - Semi-transparent cards with blur effect
- **Responsive layout** - Mobile-first design
- **Smooth animations** - Loading spinners and transitions
- **Color-coded data** - UV index and weather conditions
- **Weather emojis** - Visual indicators for conditions
- **Accessibility** - Semantic HTML and ARIA labels

## 📱 Responsive Breakpoints

- **Mobile** - Full-width single column
- **Tablet** - 2-3 column layout
- **Desktop** - Full 6-column responsive grid

## 🔄 Unit Support

The dashboard supports two unit systems:

### Metric (Celsius)
- Temperature in °C
- Wind speed in km/h
- Distance in km

### Imperial (Fahrenheit)
- Temperature in °F
- Wind speed in mph
- Distance in km (OpenWeatherMap doesn't support miles)

## 🌐 Search Functionality

### Features

- **Type-ahead search** - Get suggestions as you type
- **Popular cities** - Quick access to major cities
- **Global coverage** - Search any city worldwide
- **Autocomplete** - Filtered suggestions from popular cities
- **Error handling** - User-friendly messages for invalid cities

## 🚀 Deployment

### Deploy to Vercel (Recommended)

```bash
npm install -g vercel
vercel
```

1. Vercel will detect Next.js
2. Set `NEXT_PUBLIC_OPENWEATHER_API_KEY` in environment variables
3. Deploy!

### Deploy to Other Platforms

1. Build the app:
```bash
npm run build
```

2. Set environment variables on your hosting platform

3. Deploy the `.next` folder

## 🤝 API Rate Limits

- **Free Tier**: 60 calls per minute
- **Pro Tier**: 1,000 calls per minute

For production apps, consider upgrading to a paid plan.

## 📊 Weather API Response

The dashboard uses the OpenWeatherMap 5-day forecast API which provides:

- Current weather conditions
- Hourly forecasts (3-hour intervals)
- 5-day forecast data
- Additional metrics (UV index, cloud cover, etc.)

## 🔧 Customization

### Change Default City

Edit `/src/app/weather/page.tsx`:
```typescript
const [city, setCity] = useState('New York'); // Change this
```

### Add More Popular Cities

Edit `/src/components/SearchCity.tsx`:
```typescript
const popularCities = [
  'Your City',
  'Another City',
  // ...
];
```

### Customize Colors

Use Tailwind CSS classes in component files to change the color scheme.

## 🐛 Troubleshooting

### "City not found" error
- Check spelling of city name
- Try a larger city
- Some small towns may not be in the database

### No API data displayed
- Verify API key is correct
- Check if API key is set in `.env.local`
- Ensure free tier is active on OpenWeatherMap

### Slow loading
- OpenWeatherMap API can take 1-2 seconds
- Check internet connection
- Verify API key rate limits

## 📝 Usage Examples

### Search New York
1. Type "New York" in search box
2. Select from suggestions or hit enter
3. View current weather and forecasts

### Check Weather for Tokyo
1. Click "Tokyo" from popular cities
2. See instant weather update

### Toggle Temperature Units
1. Click "°C → °F" button in header
2. All temperatures update instantly

## 🎓 Learning Resources

- [OpenWeatherMap API Docs](https://openweathermap.org/api)
- [Next.js Documentation](https://nextjs.org/docs)
- [React Documentation](https://react.dev)
- [Tailwind CSS Docs](https://tailwindcss.com/docs)

## 📄 License

This project is open source and available under the MIT License.

## 🎉 Features in Development

- Weather alerts & warnings
- Multiple city comparison
- Weather history & trends
- Favorite cities bookmarks
- Browser geolocation support

---

**Get instant access to weather forecasts for any location worldwide!**

Made with ❤️ for weather enthusiasts
