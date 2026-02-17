# **Cocoa Artesanal: Colombian and Global Cocoa Market Analysis with R and SQL**

### **Introduction**

This project delivers a data-driven analysis of the Colombian cocoa sector, from raw bean prices to finished chocolate exports, within the context of the 2023–2024 global price surge. It explains why Colombia mirrors global trends while exports remain resilient to currency fluctuations.

The goal is to provide Cocoa Artesanal with statistically grounded insights to guide strategic decisions for 2025–2026.


### **The Project Framework: A 5-Phase Methodology**

I followed a structured data analysis lifecycle to ensure the insights were both accurate and actionable:

1. **Ask:** Defined business tasks focusing on price transmission and export growth.
2. **Prepare:** Sourced data from Comtrade Plus, the FRED (The Federal Reserve Bank of St. Louis), and local Colombian indices (Agronet).
3. **Process:** Executed a "Double-Cleaning" pipeline (Excel + R) to ensure zero-defect data.
4. **Analyze:** Conducted linear regressions, time-series decomposition (STL), Cointegration tests, and Lagged regressions.
5. **Share:** Created a executive presentation for non-technical stakeholders building the analysis into a clear data story and following a strategic framework for effective data communication.


### **Technical Skills & Rigor Showcased**

To ensure **Data Integrity**, I applied several validation techniques:

* **ROCC Compliance:** Verified that all data sources were Reliable, Original, Comprehensive, and Current.
* **The "Double-Cleaning" Pipeline:** I performed initial data hygiene in **Excel** to handle structural anomalies, followed by a secondary, reproducible cleaning script in **R** to ensure a "gold standard" dataset.
* **SQL for Cross-Validation:** Utilized SQL queries to perform "crusade" validation, cross-referencing insights between local and global datasets to ensure internal consistency.
* **Econometric Modeling:**
    * **Stationarity (ADF Tests):** Validated that data was fit for modeling by removing shared "drift."
    * **Johansen Cointegration:** Mathematically proved that cocoa prices and exchange rates are not "locked" in the long run.
    * **Lagged Regression:** Identified the three-month "industrial pulse" of price transmission.
* **Environment Validation:** Documented full **Session Info** and RAM validation to ensure the code remains reproducible in any professional R environment.


### **Analytical Framework**
To bridge the gap between data and strategy, the project includes a **conceptual frameworks** before each statistical model (Linear, Cointegration Tests, Lagged Regression, etc.). This ensures that every coefficient and test result is grounded in a clear business context before the technical execution.


### **Strategic Analysis Overview**

#### **1. Seasonality**

Using **STL Decomposition** to find the market's heartbeat.

**Visual Insight:**
![STL Decomposition](..docs/Images/stl_decomposition.png)

* **Key Finding:** A dominant October-December surge aligns with global holiday gift-giving, though "market noise" remains the primary driver of monthly volatility.

#### **2. The Price Transmission Engine**

Analysis of the **Producer Price Index (PPI)** vs. **Global Prices**.

**Visual Insight:**
![STL Decomposition](..docs/Images/colombian_exports_&_global_cocoa.png)

* **Key Finding:** A clear "three-month lag" exists where the industry absorbs costs gradually.

#### **3. Industrial Interactions: Global Prices vs. Chocolate PPI**
    
* **Key Finding:** The statistical evidence suggests that the industrial sector does not react instantly to raw material spikes; instead, it absorbs costs gradually.

**Visual Insight:**
![STL Decomposition](..docs/Images/global_cocoa_&_chocolate_ppi.png)

#### **4. The Currency Myth: Exports vs. TRM**

A multiple regression analysis on the **Exchange Rate (TRM)** and **Export Values**.

**Visual Insight:**
![STL Decomposition](..docs/Images/trm_&_colombia_cocoa.png)

* **Key Finding:** Colombian chocolate exports are "Currency Neutral." Success is driven by quality and market positioning, not a cheap Peso.


### **Project Files**

* **Analysis Script:** `cocoa_artesanal_market_analysis.Rmd` (Includes R and SQL integration)
* **Executive Presentation:** [Cocoa Artesanal - Market Strategic Presentation]()
