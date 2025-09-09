# Hybrid Renewable Energy System Optimization (HRESO)

<p align="center">
   <img src="https://img.shields.io/badge/Python-3.8%2B-blue"/>
   <img src="https://img.shields.io/badge/SciPy-Optimization-green"/>
   <img src="https://img.shields.io/badge/Matplotlib-Visualization-orange"/>
   <img src="https://img.shields.io/badge/Renewable-Energy-brightgreen"/>
</p>

---

## 📖 Project Overview

This project implements a comprehensive optimization framework for a Hybrid Renewable Energy System (HRES) combining solar photovoltaic panels, wind turbines, and battery storage. The system is designed to minimize operational costs while meeting energy demand through intelligent resource allocation.
## 🏗️ Project Structure

```
HRESO/
├── Test data/
│   ├── weather_data.csv
│   └── demand_data.csv
├── Images/
│   └── [visualizations]
├── MAIN.ipynb
├── LICENSE
└── README.md
```

## 🎯 Energy Flow Breakdown

<p align="center">
   <img src="Images/Energy Flow Renewable Penetration Analysis.jpg" width="100%" alt="Renewable Generation Breakdown"/>
</p>



## 🌱 Overview
A modern, modular framework for optimizing hybrid renewable energy systems (solar, wind, battery) to minimize costs and maximize demand satisfaction. Includes advanced analytics and interactive visualizations.

---

## 🚀 Quick Start

1. **Clone & Install**
    ```bash
    git clone https://github.com/your-username/hybrid-renewable-energy-optimization.git
    cd hybrid-renewable-energy-optimization
    pip install -r requirements.txt
    ```
2. **Prepare Data**
    - Place `weather_data.csv` and `demand_data.csv` in the `Test data/` folder.
3. **Run Optimization**
    ```python
    from src.optimization import optimize_system
    result = optimize_system(weather_data, demand_data)
    ```
4. **Visualize Results**
    ```python
    from src.visualization import plot_breakdown, plot_sankey
    plot_breakdown(result)
    plot_sankey(result)
    ```

---

## 📂 Data Format

- **weather_data.csv**: `solar_irradiance (kW/m²)`, `wind_speed (m/s)`
- **demand_data.csv**: `energy_demand (kWh)`

---

**Optimization:**
- Truncated Newton Algorithm (TNC)
- Parameters: solar efficiency (10–30%), wind efficiency (20–40%), storage utilization (0–100%)

---

## 📊 Visualizations

- **Breakdown:** Daily solar, wind, storage vs. demand
- **Sankey:** Energy flow distribution
- **Heatmap:** Surplus/deficit patterns
- **Total vs Demand:** Aggregate output vs. requirements
---

## 💡 Insights

- Solar & wind complement each other for stable supply
- Storage smooths intermittency and boosts reliability
- Hybrid systems cut costs vs. single-source
- Performance depends on weather accuracy

---

## 🤝 Contributing & License

Contributions welcome! See [LICENSE](LICENSE) for details.

---

## 📊 Data Requirements

The system requires two input CSV files:

1. **Weather Data** (`weather_data.csv`):
   - `solar_irradiance` (kW/m²)
   - `wind_speed` (m/s)

2. **Demand Data** (`demand_data.csv`):
   - `energy_demand` (kWh)

🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.


Note: This project is for educational and research purposes. Real-world implementations may require additional considerations for grid integration, regulatory compliance, and safety standards.
