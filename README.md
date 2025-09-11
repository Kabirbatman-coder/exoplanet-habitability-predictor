# ExoPlanet Habitability Predictor

A sophisticated React web application for predicting exoplanet habitability using advanced machine learning algorithms and NASA research data. Features a modern UI matching Framer design templates with full ML model integration capabilities.

## 🚀 Features

### Core Functionality
- **Advanced ML Integration**: Ready-to-connect interface for your habitability prediction model
- **Real-time Predictions**: Interactive form with instant results and detailed analysis
- **Exoplanet Database**: Searchable database with filtering and sorting capabilities
- **Personal Collection**: Save and manage your exoplanet research
- **Smart Notifications**: Context-aware user feedback system

### UI/UX Excellence
- **Premium Design**: Matches high-end Framer template aesthetics
- **Dark Space Theme**: Professional astronomy-focused interface
- **Glass Morphism**: Modern backdrop blur effects and transparency
- **Smooth Animations**: Framer Motion powered micro-interactions
- **Responsive Layout**: Perfect on all devices and screen sizes

### Scientific Accuracy
- **NASA Data Integration**: Real exoplanet parameters and classifications
- **Peer-reviewed Research**: Based on Kopparapu et al. (2013) and Schulze-Makuch et al. (2011)
- **Comprehensive Analysis**: Multi-factor habitability scoring system
- **Research-grade Output**: Publication-ready results and recommendations

## 🛠️ Installation & Setup

### Prerequisites
- Node.js (version 16 or higher)
- npm or yarn
-Trained ML model (Python/Flask backend)

### Quick Start

1. **Clone and Install**
   ```bash
   git clone <repository-url>
   cd exoplanet-habitability-predictor
   npm install
   ```

2. **Start Development Server**
   ```bash
   npm start
   ```

3. **Open Application**
   Navigate to [http://localhost:3000](http://localhost:3000)



## 📊 Application Structure

```
src/
├── components/
│   ├── Header.js              # Navigation header
│   ├── Sidebar.js             # Left navigation panel
│   ├── MainContent.js         # Content router
│   ├── HabitabilityAnalysis.js # Landing page
│   ├── ExploreDatabase.js     # Exoplanet database browser
│   ├── CalculateHabitability.js # Redirects to PredictionForm
│   ├── PredictionForm.js      # Main ML prediction interface
│   ├── SavedExoPlanets.js     # User's saved collection
│   ├── NotificationSystem.js  # Toast notifications
│   └── ...
├── services/
│   └── api.js                 # ML model API integration
├── context/
│   └── ExoplanetContext.js    # Global state management
├── App.js                     # Main application
└── index.js                   # Entry point
```

## 🎮 Usage Guide

### Making Predictions

1. **Navigate to Calculate Habitability** section
2. **Enter planetary parameters:**
   - Planet Radius (0.1 - 10.0 Earth radii)
   - Orbital Period (1 - 10,000 days)
   - Stellar Mass (0.1 - 5.0 solar masses)
   - Equilibrium Temperature (50 - 1,000 K)
   - Orbital Eccentricity (0.0 - 0.9)
   - Stellar Radius (0.1 - 5.0 solar radii)

3. **Use presets** for quick testing:
   - Earth (baseline comparison)
   - Kepler-186f (known habitable candidate)
   - Mars (marginal habitability)
   - Venus (non-habitable)

4. **Analyze results:**
   - Habitability score (0-100%)
   - Classification category
   - Factor breakdown
   - Research recommendations

### Exploring the Database

1. **Search** by exoplanet name
2. **Filter** by habitability categories
3. **Sort** by discovery date, distance, or habitability
4. **Save** interesting planets to your collection
5. **Export** data for research

### Managing Your Collection

1. **View saved planets** in your personal collection
2. **Search and sort** your saved data
3. **Export** your research collection
4. **Delete** outdated entries

## 🔧 Configuration

### Export Formats

- **JSON**: Full data structure
- **CSV**: Tabular format for analysis
- **PDF**: Research reports (future enhancement)

## 🚀 Deployment

### Production Build

```bash
npm run build
```

### Deploy to Vercel/Netlify

1. **Connect your repository**
2. **Set environment variables**
3. **Deploy automatically**

### Docker Deployment

```dockerfile
FROM node:16-alpine
WORKDIR /app
COPY package*.json ./
RUN npm ci --only=production
COPY . .
RUN npm run build
EXPOSE 3000
CMD ["npm", "start"]
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests for new functionality
5. Submit a pull request

## 📝 License

 [LICENSE](LICENSE) file for details.

## 🌟 Acknowledgments

- **NASA Exoplanet Archive** for comprehensive datasets
- **Kepler Space Telescope Team** for groundbreaking discoveries
- **ESA Gaia Mission** for stellar characterization
- **Research Community** for peer-reviewed methodologies

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/your-repo/issues)
- **Discussions**: [GitHub Discussions](https://github.com/your-repo/discussions)
- **Email**: 1kabirkhankk@gmail.com
---

**Ready to discover habitable worlds? Start exploring! 🌍✨** 
