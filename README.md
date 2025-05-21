# 🔋⚡ V2G Optimizer: Electricity Cost Optimization with Vehicle-to-Grid Technology

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE.txt) 
[![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/downloads/)
[![Streamlit Version](https://img.shields.io/badge/streamlit-1.20%2B-ff69b4.svg)](https://streamlit.io/)
[![MATLAB/Simulink](https://img.shields.io/badge/MATLAB%2FSimulink-R20XXx-orange.svg)](https://www.mathworks.com/products/matlab.html)

## 🚧 Project Status: Under Active Development 🚧

![V2G Concept Illustration](https://i.imgur.com/placeholder.jpg)

## 📋 Quick Links
- [Overview](#overview)
- [V2G Technology Explained](#v2g-explained)
- [Key Features](#key-features)
- [Technology Stack](#technology-stack)
- [Repository Structure](#repository-structure)
- [Simulation Details](#simulation-details)
- [Installation & Usage](#running-the-application)
- [Acknowledgements](#acknowledgements)
- [License](#license)
- [Contact](#contact)

## Overview

V2G Optimizer is an advanced energy management solution that leverages Vehicle-to-Grid (V2G) technology to minimize electricity production costs. This project extends a foundational MATLAB/Simulink V2G simulation to model monthly timeframes and incorporates:

- Real-world solar irradiance data from Meknès, Morocco
- Custom-generated residential load profiles representative of Moroccan consumption patterns
- Comprehensive cost optimization algorithms

Our Streamlit-based web application provides weekly forecasts to help decision-makers determine the optimal balance between utilizing stored EV energy via V2G technology versus supplementing with diesel generation during peak demand periods.

## V2G Explained

### What is Vehicle-to-Grid (V2G)?

Vehicle-to-Grid (V2G) is a cutting-edge technology enabling bidirectional energy flow between electric vehicle batteries and the power grid. Unlike conventional EV charging, V2G allows vehicles to not only consume electricity but also return it to the grid when beneficial.

### How It Works

![V2G Process Flow](https://i.imgur.com/placeholder2.jpg)

When connected to a V2G-enabled charging station, the system manages electricity flow through:

1. **Charging Mode:** The EV draws power from the grid to charge its battery
2. **Discharging (V2G) Mode:** The EV feeds stored energy back to the grid when:
   - Grid demand peaks 
   - Energy prices are high
   - Renewable energy generation is low

This process is coordinated through sophisticated control systems with EV owner consent, typically including financial incentives for participation.

### V2G Use Cases

V2G technology offers multiple benefits across the energy ecosystem:

| Use Case | Description |
|----------|-------------|
| **Peak Shaving** | Reduces grid strain during high-demand periods by supplying stored EV energy |
| **Grid Stabilization** | Provides ancillary services like frequency regulation and voltage support |
| **Renewable Integration** | Stores surplus renewable energy for use when generation is insufficient |
| **Emergency Backup** | Offers potential backup power during outages |
| **Economic Optimization** | Creates revenue opportunities for EV owners through energy arbitrage |

Our project specifically focuses on cost optimization by determining when V2G utilization is more economical than alternative generation sources.

## Key Features

- **Enhanced Simulation Timeframe:** Extended MATLAB/Simulink model for monthly energy analysis (vs. original 24-hour scope)
- **Localized Data Integration:**
  - Actual solar irradiation data from Meknès, Morocco
  - Realistic residential load profiles mirroring Moroccan consumption patterns
- **Advanced Optimization Engine:** Cost-minimization algorithms to determine optimal energy sourcing strategies
- **Interactive Decision Support:** Streamlit application providing:
  - Weekly energy forecasts
  - Cost-comparison between V2G and diesel generation
  - Actionable recommendations for energy management
- **Comprehensive Analytics:** Data visualization and insights on load patterns, solar production, and V2G availability

## Technology Stack

### Simulation Environment
- MATLAB R20XXx
- Simulink

### Data Processing & Analysis
- Python 3.x
- Pandas
- NumPy
- Scikit-learn

### Web Application
- Streamlit 1.20+
- Plotly
- Altair

### Data Sources
- Solar irradiation measurements from Meknès, Morocco
- Synthetic residential load profiles based on Moroccan consumption patterns

## Repository Structure

```
V2G_TS_Project/
├── Notebooks/                  # Jupyter notebooks for data analysis
├── Best_Models/                # Optimized predictive models
├── Datasets/                   # Raw and processed datasets
│   ├── solar_irradiance/       # Solar data for Meknès
│   └── load_profiles/          # Generated residential load data
├── Simulation/                 # MATLAB/Simulink simulation files
├── App_version_one/            # Streamlit application
│   ├── app.py                  # Main application entry point
│   ├── modules/                # Application components
│   └── assets/                 # Static resources
├── requirements.txt            # Python dependencies
├── README.md                   # This documentation
└── LICENSE.txt                 # MIT License
```

## Simulation Details

Our simulation builds upon a foundation provided by MathWorks, with significant adaptations for this project:

### Key Modifications
- **Temporal Extension:** Monthly simulation periods versus the original 24-hour window
- **Component Refinement:** Removed wind farm component to focus on solar + V2G integration
- **Localization:** Integration of Morocco-specific data sources

### Data Inputs
- **Solar Irradiance:** High-resolution measurements from Meknès region
- **Residential Load:** Synthesized load profiles reflecting Moroccan consumption patterns
- **EV Fleet Parameters:** Battery capacity, charging/discharging rates, and availability schedules

### Simulation Outputs
- Total Residential Load (kW)
- Solar Energy Production (kW)
- Available V2G Power Capacity (kW)
- Cost Optimization Metrics (MAD/kWh)

## Running the Application

### Prerequisites
- Python 3.7+
- Git
- (Optional) MATLAB/Simulink for simulation modifications

### Installation Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/sohaibdaoudi/V2G_TS_Project.git
   cd V2G_TS_Project
   ```

2. **Set up a Python virtual environment:**
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch the Streamlit application:**
   ```bash
   cd App_version_one
   streamlit run app.py
   ```

5. **Access the application:**
   Open your browser and navigate to `http://localhost:8501`

## Acknowledgements

This project builds upon the "24-hour Simulation of a Vehicle-to-Grid (V2G) System" example provided by MathWorks. We extend our gratitude to MathWorks for providing this valuable foundation. The original simulation concept can be found [here](https://www.mathworks.com/help/sps/ug/24-hour-simulation-of-a-vehicle-to-grid-v2g-system.html).

## License

This project is licensed under the [MIT License](./LICENSE.txt) - see the LICENSE.txt file for details.

## Contact

### Project Maintainers

- **Sohaib Daoudi**
  - Email: [soh.daoudi@gmail.com](mailto:soh.daoudi@gmail.com)
  - GitHub: [@sohaibdaoudi](https://github.com/sohaibdaoudi)

- **Marouane Majidi**
  - Email: [majidi.marouane0@gmail.com](mailto:majidi.marouane0@gmail.com)
  - GitHub: [@marouanemajidi](https://github.com/marouanemajidi)

---

<p align="center">
  <em>Powering the future, one vehicle at a time.</em>
</p>
