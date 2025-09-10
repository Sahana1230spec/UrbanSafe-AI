 # UrbanSafe-AI 🚨
## Smart City Mobility & Accident Risk Prediction - Data Analysis Phase
### 🎯 Project Overview
Initial phase of a smart traffic safety prediction system analyzing UK road accident data. This project explores accident patterns and builds a baseline machine learning model to predict accident severity.

### 📊 Current Results
- **104,258 accident records** analyzed from UK Department of Transportation (2023)
- **73.6% prediction accuracy** achieved with Random Forest model
- **Rush hour risk identified**: Peak accidents at 17:00 (9,216 incidents)
- **Key insight**: 78.7% of accidents occur in good weather conditions

### 🛠️ Technology Stack
- **Data Processing**: Python, Pandas, NumPy
- **Machine Learning**: Scikit-learn, Random Forest
- **Visualization**: Matplotlib
- **Data Source**: UK Road Safety Data (2023)

### 📈 Key Findings
1. **Accident Severity Distribution**:
   - Fatal: 1.5% (1,522 cases)
   - Serious: 22.5% (23,438 cases) 
   - Slight: 76.1% (79,298 cases)

2. **Risk Patterns**:
   - Peak hour: 17:00 (rush hour)
   - Most accidents: Single carriageways (72.6%)
   - Weather impact: Minimal difference between fine/rainy conditions

3. **ML Model Performance**:
   - Overall accuracy: 73.6%
   - Best at predicting slight injuries (95% recall)
   - Time of day is most important feature (38.9% importance)

### 🔧 What's Implemented
- [x] Data loading and exploration
- [x] Statistical analysis and insights
- [x] Data visualization (charts and graphs)
- [x] Feature engineering 
- [x] Random Forest classification model
- [x] Model evaluation and feature importance analysis

### 📁 Project Structure
```
UrbanSafe-AI/
├── data/
│   └── raw/                    # UK road safety datasets (3 files)
├── results/                    # Generated visualizations
├── check_data.py              # Main analysis pipeline
├── README.md                  # Project documentation
└── requirements.txt           # Python dependencies
```

### ⚡ Quick Start
1. **Clone and setup**
   ```bash
   git clone https://github.com/Sahana1230spec/UrbanSafe-AI.git
   cd UrbanSafe-AI
   pip install pandas numpy matplotlib scikit-learn
   ```

2. **Add your data**
   - Download UK Road Safety Data (2023) from gov.uk
   - Place CSV files in `data/raw/` folder

3. **Run analysis**
   ```bash
   python check_data.py
   ```

### 📊 Current Model Performance
| Metric | Value |
|--------|-------|
| Accuracy | 73.6% |
| Training Samples | 104,258 |
| Features Used | 7 (time, weather, road type, etc.) |
| Most Important Feature | Hour of day (38.9%) |

### 🚀 Next Phase (Planned)
- [ ] Apache Spark integration for big data processing
- [ ] Geospatial analysis with coordinate mapping
- [ ] Interactive Streamlit dashboard
- [ ] Real-time prediction API
- [ ] Advanced ML models (ensemble methods)
- [ ] Spatiotemporal risk modeling

### 📚 Data Source
UK Department for Transport - Road Safety Data (2023)
- Collision records: 104,258 incidents
- Casualty records: 132,977 people involved  
- Vehicle records: 189,815 vehicles involved

### 🔒 Note
This repository is currently private during development. Data files are not included in the repository due to size - download instructions provided above.

---
*Building safer cities through data-driven insights* 🚗📊
