# 🌍 Climate Action Intelligence Platform

**ClimateIQ - Your AI Climate Action Partner**

A comprehensive platform that combines IBM watsonx.ai, RAG (Retrieval-Augmented Generation), real-time climate APIs, and an intuitive Streamlit interface to provide personalized climate action recommendations and environmental impact tracking.

## 🚀 Features

### 🤖 AI-Powered Climate Assistant
- **IBM watsonx.ai Integration**: Advanced AI models for climate action recommendations
- **RAG System**: Retrieval-Augmented Generation with climate knowledge base
- **Personalized Responses**: Tailored advice based on user profile and location
- **Fallback Mode**: Intelligent responses even when external services are unavailable

### 📊 Real-Time Climate Data
- **Weather Data**: OpenWeatherMap API integration
- **Carbon Emissions**: Carbon Interface API for footprint calculations
- **NASA POWER**: Solar and energy resource data
- **Climate Trace**: Global emissions tracking
- **UN SDG & World Bank**: Sustainability indicators

### 🎯 Personalized Action Plans
- Location-based recommendations
- Lifestyle-specific suggestions
- Budget-conscious solutions
- Impact estimation and tracking

### 📈 Impact Tracking Dashboard
- Personal carbon footprint monitoring
- Progress visualization with interactive charts
- Emission equivalents (trees, gasoline, coal)
- Community leaderboards

### 🌤️ Local Environmental Data
- Real-time weather conditions
- Air quality monitoring
- Local climate trends
- Environmental alerts

## 🛠️ Technology Stack

- **Frontend**: Streamlit with custom CSS styling
- **AI/ML**: IBM watsonx.ai, LangChain, ChromaDB
- **APIs**: Climate APIs (OpenWeather, Carbon Interface, NASA, etc.)
- **Data Processing**: Pandas, NumPy
- **Visualization**: Plotly, Matplotlib
- **Environment**: Python 3.8+, dotenv

## 📋 Prerequisites

- Python 3.8 or higher
- pip package manager
- Internet connection for API access

## 🔧 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/Nordic116/Climate-Action-Intelligence-Platform.git
cd Climate-Action-Intelligence-Platform
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Setup Data Directories
```bash
python setup_data_dirs.py
```

### 4. Test Installation (Optional)
```bash
python test_installation.py
```

### 5. Configure Environment Variables
Create a `.env` file in the root directory with your API keys:

```env
# IBM watsonx.ai
IBM_CLOUD_API_KEY=your_ibm_cloud_api_key
WATSONX_PROJECT_ID=your_watsonx_project_id
IBM_CLOUD_URL=https://us-south.ml.cloud.ibm.com
WATSONX_API_KEY=your_watsonx_api_key

# Climate APIs
OPENWEATHER_API_KEY=your_openweather_api_key
CARBON_INTERFACE_API_KEY=your_carbon_interface_api_key
NASA_API_KEY=your_nasa_api_key

# API Base URLs (pre-configured)
CLIMATETRACE_API_BASE=https://api.climatetrace.org/v6
CARBON_INTERFACE_API_BASE=https://www.carboninterface.com/api/v1
NASA_API_BASE=https://power.larc.nasa.gov/api/temporal
OPENWEATHER_API_BASE=https://api.openweathermap.org/data/2.5
UN_SDG_API_BASE=https://unstats.un.org/SDGAPI/v1
WORLD_BANK_API_BASE=https://api.worldbank.org/v2

# Default settings
DEFAULT_OUTPUT_FORMAT=json
```

### 6. Run the Application
```bash
python run_app.py
```

The application will be available at:
- **Local**: http://localhost:12000
- **Network**: Available on your local network

## 🎮 Usage Guide

### Getting Started
1. **Launch the app** using `python run_app.py`
2. **Set up your profile** in the sidebar:
   - Enter your location
   - Select lifestyle type
   - Choose areas of interest
   - Set your budget range

### Main Features

#### 🎯 Action Plan Tab
- Click "Generate New Action Plan" for personalized recommendations
- View prioritized actions based on your profile
- See estimated impact and cost savings
- Access supporting information sources

#### 📊 Impact Tracker Tab
- Monitor your carbon footprint over time
- View emission equivalents (trees planted, gasoline saved)
- Track progress with interactive charts
- Compare with community averages

#### 🌤️ Local Data Tab
- View real-time weather conditions
- Check air quality index
- See local climate trends
- Get environmental alerts

#### 💬 AI Assistant Tab
- Chat with the AI climate assistant
- Ask questions about sustainability
- Get personalized advice
- Use quick action buttons for common queries

#### 🏆 Community Tab
- View community impact leaderboard
- See collective achievements
- Join challenges and initiatives
- Share your progress

## 🔄 Demo Mode

The platform includes a comprehensive demo mode that activates when:
- API keys are not configured
- External services are unavailable
- Network connectivity issues occur

Demo mode provides:
- Sample climate data and visualizations
- Pre-built action plans
- Intelligent fallback responses
- Full interface functionality

## 📁 Project Structure

```
Climate-Action-Intelligence-Platform/
├── backend/
│   ├── watsonx_integration/     # IBM watsonx.ai integration
│   ├── rag_system/             # RAG system with ChromaDB
│   ├── api_handlers/           # Climate API integrations
│   └── data_processors/        # Data processing utilities
├── frontend/
│   └── dashboard/              # Streamlit application
├── data/                       # Local data storage
├── config.py                   # Configuration settings
├── requirements.txt            # Python dependencies
├── run_app.py                 # Application launcher
└── .env                       # Environment variables
```

## 🔑 API Keys Setup

### Required APIs (for full functionality):
1. **IBM watsonx.ai**: Sign up at [IBM Cloud](https://cloud.ibm.com/)
2. **OpenWeatherMap**: Get free API key at [OpenWeatherMap](https://openweathermap.org/api)
3. **Carbon Interface**: Register at [Carbon Interface](https://www.carboninterface.com/)
4. **NASA POWER**: Request access at [NASA POWER](https://power.larc.nasa.gov/)

### Optional APIs:
- Climate Trace (public API)
- UN SDG API (public API)
- World Bank API (public API)

## 🚀 Deployment Options

### Local Development
```bash
python run_app.py
```

### Production Deployment
The application is designed for local use but can be deployed to:
- Cloud platforms (AWS, GCP, Azure)
- Container environments (Docker)
- Streamlit Cloud
- Heroku or similar PaaS

## 🎯 Project Features

### Unique Value Propositions
1. **Hyper-Personalized Climate Action Plans** - Uses RAG to combine global climate data with local context
2. **Real-Time Impact Measurement** - Tracks and quantifies actual environmental impact
3. **Community-Driven Solutions** - Crowdsources and validates climate solutions
4. **Economic Incentivization** - Connects users with green financing and carbon offset opportunities
5. **Scalable Implementation** - Works for individuals, SMEs, and large organizations

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Troubleshooting

### Common Issues

**Application won't start:**
- Check Python version (3.8+ required)
- Verify all dependencies are installed: `pip install -r requirements.txt`
- Ensure port 12000 is available

**API errors:**
- Verify API keys in `.env` file
- Check internet connectivity
- Review API rate limits
- Use demo mode for testing without APIs

**Performance issues:**
- Clear browser cache
- Restart the application
- Check system resources

### Getting Help

- Check the [Issues](https://github.com/Nordic116/Climate-Action-Intelligence-Platform/issues) page
- Review the troubleshooting section
- Contact the development team

## 🌟 Acknowledgments

- IBM watsonx.ai for advanced AI capabilities
- Climate data providers (OpenWeatherMap, NASA, etc.)
- Streamlit for the amazing web framework
- The open-source community for various libraries and tools

---

**Built with ❤️ for a sustainable future 🌱**

*ClimateIQ - Empowering individuals to take meaningful climate action through AI-driven insights and personalized recommendations.*
