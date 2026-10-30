# Smart Grid Digital Twin & Power Distribution Simulator

**Version:** 1.0.0  
**Language:** Python  
**Environment:** Google Colab  
**Simulation Type:** Fully Simulated

## Overview

The Smart Grid Digital Twin is a Python-based simulation platform designed to model and monitor an interconnected electrical power distribution network.

The project simulates interactions between power generation facilities, substations, transformers, battery energy storage systems, and electricity consumers. It demonstrates how software systems can be used to monitor grid conditions, evaluate power demand, identify potential equipment issues, and support operational decision-making.

## Key Features

- **Grid Topology Modeling:** NetworkX-based representation of generators, substations, transformers, and consumers.
- **Power Generation Simulation:** Models thermal, solar, and wind generation.
- **Demand Forecasting:** Simulates changing electricity consumption across residential, commercial, industrial, and critical infrastructure loads.
- **Energy Storage:** Models battery state of charge, discharge limits, and generation balancing.
- **Transformer Monitoring:** Evaluates transformer loading and identifies potential overload conditions.
- **Load Redistribution:** Demonstrates simplified load redistribution to reduce transformer loading.
- **Grid Diagnostics:** Monitors simulated voltage and frequency measurements.
- **Fault Management:** Registers simulated equipment faults, assigns severity levels, and initiates response workflows.
- **Telemetry Database:** Stores grid measurements and fault records using SQLite.
- **Machine Learning:** Uses Scikit-learn Isolation Forest for unsupervised anomaly detection.
- **Interactive Dashboards:** Uses Plotly for engineering charts and operational monitoring.
- **3D Grid Visualization:** Displays the simulated infrastructure as a three-dimensional network.

## Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core simulation logic |
| NumPy | Numerical calculations |
| Pandas | Data processing and analysis |
| NetworkX | Grid topology modeling |
| Scikit-learn | Machine learning and anomaly detection |
| SQLite | Telemetry and fault data storage |
| Plotly | Interactive dashboards and visualization |
| Google Colab | Development and execution environment |

## System Architecture

The simulation follows a layered workflow:

1. **Infrastructure Layer:** Models generation facilities, substations, transformers, and electricity consumers.
2. **Simulation Layer:** Calculates generation, demand, power balance, and battery dispatch.
3. **Monitoring Layer:** Evaluates transformer loading, voltage, frequency, and system conditions.
4. **Fault Management Layer:** Processes simulated faults and assigns response priorities.
5. **Data Layer:** Stores telemetry and fault records in SQLite.
6. **Analytics Layer:** Applies machine learning to identify unusual operating patterns.
7. **Visualization Layer:** Presents grid topology, operational metrics, and three-dimensional infrastructure views.

## Running the Project

The notebook is designed to run in Google Colab.

1. Download `Smart_Grid_Digital_Twin_Final.ipynb` from this repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Select **File → Upload notebook**.
4. Upload the downloaded notebook.
5. Run the notebook cells sequentially, starting with the environment setup.

The first cell installs the required Python dependencies.

## Validation

The completed simulation passed 11 out of 11 final validation checks, covering:

- Grid topology and connectivity
- Generation and consumer models
- Transformer monitoring
- Fault management
- Telemetry and fault database operations
- Machine learning initialization
- 3D visualization
- Engineering dashboard generation

## Engineering Disclaimer

This project is an educational software simulation. Electrical behavior, power-flow calculations, transformer loading, protection systems, and grid operating conditions are simplified models.

It is not a validated electrical engineering tool and is not intended for real-world utility operations or control of physical infrastructure.

## Project Status

**Version 1.0.0 | Initial release**
