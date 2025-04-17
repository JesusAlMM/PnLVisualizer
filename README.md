# Profit and Loss Visualizer

This interactive Shiny-based application implements the Black-Scholes model to calculate Call and Put option prices. Through a user-friendly and intuitive panel, it allows users to explore how prices and expected profits/losses (PnL) change based on variations in key parameters such as spot price and volatility. The app includes dynamic visualizations using heatmaps and features a connection to a MySQL database, where inputs and simulation results are automatically stored for traceability and further analysis.

*Basic app:  
http://038p5o-jesus-martinez.shinyapps.io/pet1  

## 📂 Repository Contents  

- `app/`: Version ready for deployment on shinyapps.io.  
- `app_db/`: Advanced version with database connectivity.  
- `sql/schema.sql`: Queries to create and populate required tables.  
- `README.md`: Documentation.  

## 🚀 Features  

### 1. Option Calculation and Simulation  

- Calculation of option prices (Call and Put) using the Black-Scholes model.  
- Buy/sell simulation with PnL (profit/loss) calculation.  
- Real-time visualization of Call and Put prices.  

### 2. Interactive Dashboard  

- Input panel for key parameters:  
  - Spot (S)  
  - Strike (K)  
  - Time to maturity (T)  
  - Volatility (σ)  
  - Risk-free rate (r)  

- Custom range configuration for heatmap generation.  
- Dynamic heatmaps for prices and PnL under different scenarios.  
- Reset button to restore default parameters.  

### 3. Database Persistence  

- Automatic logging of each simulation in a MySQL database.  
- Structured storage of inputs, outputs, and relative shocks (spot and volatility).  

## ⚙️ Scalability  

Although this application is currently connected to a MySQL database, its architecture allows easy adaptation to other storage systems such as PostgreSQL, SQLite, or cloud services like Amazon RDS, Google Cloud SQL, or Azure SQL Database.  

