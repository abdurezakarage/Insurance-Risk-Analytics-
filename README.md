# Insurance Risk Analytics

A comprehensive Python-based analytics toolkit for insurance risk assessment and portfolio analysis. This project provides powerful tools for analyzing insurance data, identifying patterns, and generating insights to support risk management decisions.

## Features

- **Data Analysis & Quality Assessment**
  - Comprehensive data type analysis
  - Missing value detection and analysis
  - Data quality metrics calculation
  - Outlier detection and handling

- **Portfolio Analysis**
  - Premium and claims analysis
  - Loss ratio calculations
  - Portfolio metrics and key insights
  - Financial distribution analysis

- **Geographic Analysis**
  - Regional trend analysis
  - Province-level metrics comparison
  - Geographic pattern identification
  - Regional correlation analysis

- **Temporal Analysis**
  - Monthly trend analysis
  - Time-based pattern detection
  - Seasonal variation analysis
  - Historical trend visualization

- **Vehicle Analysis**
  - Make and model analysis
  - Vehicle type distribution
  - Age and value analysis
  - Risk assessment by vehicle characteristics

- **Advanced Analytics**
  - Correlation analysis
  - Pairwise relationship analysis
  - Statistical distribution analysis
  - Pattern recognition

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/Insurance-Risk-Analytics.git
cd Insurance-Risk-Analytics
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

### Basic Usage

```python
from src.services.insurance_analysis import InsuranceAnalysis
import pandas as pd

# Load your insurance data
df = pd.read_csv('your_insurance_data.csv')

# Initialize the analysis
analysis = InsuranceAnalysis(df)

# Run comprehensive analysis
analysis.run_analysis()
```

### Specific Analysis Examples

```python
# Analyze geographic trends
analysis.analyze_geographic_trends()

# Analyze correlations between variables
analysis.analyze_correlations()

# Analyze monthly changes by zipcode
analysis.analyze_monthly_changes_by_zipcode()

# Analyze vehicle metrics
analysis.analyze_vehicle_metrics()
```

## Data Requirements

The analysis expects the following key columns in your dataset:
- TotalPremium
- TotalClaims
- Province
- PostalCode
- VehicleType
- Make
- TransactionMonth
- VehicleIntroDate

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
