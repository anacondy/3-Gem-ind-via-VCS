# India Governance Map 2025
  https://anacondy.github.io/3-Gem-ind-via-VCS/ --- DEMO

An interactive map of India showing political control and leadership across all states and union territories.

## Features

- **Interactive Map**: Click on any state to view detailed political information
- **Mobile Optimized**: Fully responsive design optimized for 16:9 and 20:9 aspect ratio devices
- **Real-time Updates**: Integrated with Gemini API to fetch the latest political data
- **Comprehensive Data**: Shows ruling party, opposition, coalition details, and seat distribution
- **Clean UI**: Modern glassmorphism design with smooth animations

## Mobile Optimizations

- **Responsive Sidebar**: State details appear in a bottom drawer taking 50% of screen on mobile
- **Fixed Tooltip Issue**: Removed the square box that appeared when hovering over states
- **Better Rendering**: Optimized for mobile with improved contrast and rendering performance
- **Dynamic Viewport**: Supports both portrait and landscape orientations
- **Touch-Friendly**: Optimized tap targets and interactions for touch devices

## Gemini API Integration

This application uses Google's Gemini API to fetch the latest political data for Indian states.

### Setup Instructions

1. **Get an API Key**:
   - Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Sign in with your Google account
   - Create a new API key

2. **Configure the Application**:
   - Open `index.html`
   - Find the line: `const GEMINI_API_KEY = 'YOUR_GEMINI_API_KEY_HERE';`
   - Replace `YOUR_GEMINI_API_KEY_HERE` with your actual API key
   - Example: `const GEMINI_API_KEY = 'AIzaSyABC123...';`

3. **Use the Update Feature**:
   - Click the "🔄 Update Political Data" button in the header
   - The app will fetch the latest data from Gemini API
   - Data is automatically validated and merged with existing information

### API Features

The Gemini API integration provides:

- **Latest Data**: Fetches data from November 2025 or later
- **Comprehensive Information**: 
  - Chief Minister names
  - Ruling party/coalition details
  - Assembly seat distribution
  - Opposition strength
  - Coalition composition
- **Multi-Source Verification**: AI cross-checks data from multiple reliable sources
- **Automatic Updates**: Refreshes the map with new data instantly

### API Prompt Details

The application uses an advanced prompt that:
- Requests data for all 28 states and 8 union territories
- Requires data from November 2025 or later
- Cross-verifies information from official sources (Election Commission, state governments, news agencies)
- Captures coalition details and opposition seat counts
- Returns structured JSON for easy parsing

## Data Displayed

For each state, the map shows:

1. **Alliance Badge**: NDA (Ruling), INDIA Bloc, or Regional/Independent
2. **State Name**: Full name of the state/UT
3. **Chief Minister**: Current CM or Administrator
4. **Ruling Party**: Party name or coalition name
5. **Assembly Strength**: Current seats held / Total seats
6. **Coalition Type**: Single party, Coalition, or Multi-party
7. **Opposition**: Opposition seat count and main parties

## How to Use

1. **Open the Map**: Simply open `index.html` in a modern web browser
2. **Explore States**: 
   - Hover over states to see their names
   - Click on any state to view detailed information
   - Click anywhere on the map background to close the sidebar
3. **Update Data**: Click the refresh button to fetch the latest political data via Gemini API
4. **Mobile**: On mobile devices, the sidebar slides up from the bottom showing state details

## Technical Stack

- **Leaflet.js**: Interactive mapping library
- **CartoDB Dark**: Map tiles for clean dark theme
- **Gemini API**: AI-powered data updates
- **Pure HTML/CSS/JS**: No build process required

## Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile browsers (iOS Safari, Chrome Mobile)
- Requires internet connection for map tiles and API updates

## Color Coding

- **Orange (#FF9933)**: NDA-ruled states
- **Cyan (#00E5FF)**: INDIA Bloc states
- **Yellow (#FFFF00)**: Regional/Other parties

## Privacy & Security

⚠️ **IMPORTANT SECURITY NOTICE**:
- The API key in this implementation is stored in client-side code for demonstration purposes only
- **DO NOT use this approach in production environments**
- For production deployment:
  1. Store API keys in environment variables
  2. Create a backend proxy server to handle API requests
  3. Implement rate limiting and authentication
  4. Never expose API keys in client-side code
- No user data is collected or stored by this application
- Consider implementing a backend service for secure API key management

## License

Open source - feel free to use and modify

## Credits

- GeoJSON data: [geohacker/india](https://github.com/geohacker/india)
- Map tiles: CartoDB
- AI Integration: Google Gemini API
