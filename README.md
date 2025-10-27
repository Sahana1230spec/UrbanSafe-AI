# UrbanSafe-AI
## Smart City Mobility & Accident Risk Prediction System

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-red.svg)](https://streamlit.io/)

**Live Demo:** [UrbanSafe-AI Dashboard](https://your-streamlit-url-here)

---

## Project Overview

UrbanSafe-AI analyzes over 104,000 UK road accident records to predict accident severity and identify high-risk scenarios using machine learning and interactive visualization.

### Key Results
- 104,258 accident records analyzed from UK Department of Transportation (2023)
- 73.4% prediction accuracy using Random Forest classifier
- Interactive web dashboard with real-time predictions
- Geospatial analysis with accident hotspot mapping

---

## Technology Stack

**Data Processing**: Python, Pandas, NumPy, Scikit-learn
**Visualization**: Streamlit, Plotly, Folium, Matplotlib
**Data Source**: UK Department for Transport - Road Safety Data (2023)

---

## Key Findings

### Accident Statistics
- Total Accidents: 104,258
- Fatal: 1,522 (1.5%)
- Serious: 23,438 (22.5%)
- Slight: 79,298 (76.1%)

### Risk Patterns
- Peak accident hour: 17:00 with 9,216 incidents
- Most accidents: Single carriageways (72.6%)
- 78.7% of accidents occur in good weather
- Minimal difference in fatal rates between weather conditions

### Model Performance
- Overall Accuracy: 73.4%
- Top Feature: Hour of day (38.9% importance)
- Best Performance: 95% recall for slight injury prediction

---

## Features

### Data Analysis Pipeline (`check_data.py`)
- Data loading and validation
- Statistical analysis and insights
- Feature engineering
- Machine learning model training
- Visualization generation

### Interactive Dashboard (`dashboard.py`)
- **Overview**: Key metrics and distribution charts
- **Risk Predictor**: Real-time severity predictions based on input scenarios
- **Hotspot Map**: Geospatial visualization with color-coded severity markers
- **Analytics**: Monthly trends, weather impact, and pattern analysis

---

## Project Structure

```
UrbanSafe-AI/
├── data/
│   └── raw/                    # UK road safety datasets
├── results/                    # Generated visualizations
├── check_data.py              # Analysis pipeline
├── dashboard.py               # Streamlit web application
├── requirements.txt           # Dependencies
└── README.md                  # Documentation
```

---

## Installation & Usage

### Prerequisites
- Python 3.8+
- pip

### Setup

```bash
# Clone repository
git clone https://github.com/Sahana1230spec/UrbanSafe-AI.git
cd UrbanSafe-AI

# Install dependencies
pip install -r requirements.txt
```

### Download Data
1. Visit [UK Road Safety Data](https://www.data.gov.uk/dataset/cb7ae6f0-4be6-4935-9277-47e5ce24a11f/road-safety-data)
2. Download: Collisions 2023, Casualties 2023, Vehicles 2023
3. Place CSV files in `data/raw/` folder

### Run Analysis
```bash
python check_data.py
```

### Launch Dashboard
```bash
streamlit run dashboard.py
```

Dashboard opens at `http://localhost:8501`

---

## Model Details

**Algorithm**: Random Forest Classifier
**Configuration**: 100 estimators, 80/20 train-test split
**Accuracy**: 73.4%

### Feature Importance
| Feature | Importance |
|---------|-----------|
| Hour of Day | 38.9% |
| Day of Week | 20.0% |
| Weather Conditions | 10.3% |
| Speed Limit | 8.6% |
| Road Surface | 8.6% |
| Road Type | 7.8% |
| Light Conditions | 5.8% |

---

## Deployment

### Streamlit Cloud
1. Push code to GitHub
2. Visit streamlit.io/cloud
3. Connect repository
4. Deploy

---

## Future Enhancements

- Apache Spark integration for distributed processing
- Real-time traffic data integration
- Deep learning models for improved accuracy
- REST API development
- Multi-city analysis

---

## Author

**Sahana**  
GitHub: [@Sahana1230spec](https://github.com/Sahana1230spec)

---

## License

MIT License

---

## Data Source

UK Department for Transport - Road Safety Data (2023)