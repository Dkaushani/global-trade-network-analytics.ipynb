# global_trade_network_analytics.ipynb

# 🌐 Global Commodity Trade & Network Risk Dashboard

An interactive Business Intelligence (BI) pipeline and data application built to model global commodity trade flows ($5B+ dataset) and evaluate supply chain vulnerabilities using official **UN Comtrade** data (HS 3102 - Nitrogenous Fertilizers).

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![SQL](https://img.shields.io/badge/SQL-SQLite-lightgrey.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-red.svg)
![NetworkX](https://img.shields.io/badge/NetworkX-Graph_Theory-orange.svg)

---

## 📌 Project Overview

Global supply chains for critical commodities like fertilizers are highly concentrated, making economies vulnerable to geopolitical shocks and trade bottlenecks. This project processes thousands of bilateral trade records to:
1. **Map Global Supply Corridors:** Clean and aggregate complex UN Comtrade datasets into structured relational tables.
2. **Identify Trade Chokepoints:** Apply Graph Centrality algorithms to identify systemic transit hubs versus simple high-volume importers/exporters.
3. **Interactive BI Dashboard:** Deploy a real-time web interface allowing users to filter trade volumes by country, minimum dollar threshold, and supply dependencies.

---

## 🛠️ Tech Stack & Methods

* **Data Processing & ETL:** Python (`Pandas`)
* **Database & Querying:** SQLite (Common Table Expressions / CTEs, Window Functions `DENSE_RANK()`, `HAVING`)
* **Network Analysis:** `NetworkX` (In-Degree, Out-Degree, Betweenness, and Eigenvector Centralities)
* **Visualization & BI:** `Plotly` & `Streamlit`
* **Dataset:** UN Comtrade (2022 Bilateral Fertilizer Trade - HS 3102)

---

## 📊 Key Findings

* **Major Trade Hubs:** **Brazil** ($1.55B from China) and **India** ($1.27B from Oman) represent massive regional import nodes heavily dependent on concentrated supplier sets.
* **Network Chokepoints:** **Germany** and the **USA** exhibit high **Betweenness Centrality**, acting as critical bridge economies connecting regional trading corridors to global supply chains.
* **Supplier Concentration:** Over 70+ importing nations rely on 3 or fewer partner countries for more than 80% of their fertilizer imports.

---

## 🚀 Interactive Dashboard Features

The Streamlit web application includes:
* **Dynamic Corridor Filtering:** Filter global trade networks by minimum transaction values ($M).
* **Country Node Selection:** Isolate individual nations (e.g., *Oman* or *Brazil*) to inspect their specific import/export web.
* **Real-time KPI Metrics:** Instantly recalculates total trade volume ($M), active trade routes, and participating economies based on user filters.

<img width="865" height="596" alt="image" src="https://github.com/user-attachments/assets/59f21316-3c4f-41a7-a3fd-57b3f4b649bf" />

<img width="505" height="653" alt="image" src="https://github.com/user-attachments/assets/c4c44980-e15a-4db8-b6ea-4bd4436172cc" />


<img width="1881" height="809" alt="image" src="https://github.com/user-attachments/assets/9ee4b675-fd7d-4848-90ed-d43e9a5b5506" />

<img width="1527" height="513" alt="image" src="https://github.com/user-attachments/assets/60c22ad6-b92a-4e19-8972-1c0c56c12d04" />


**HHI Concentration & Geopolitical Sanction Simulation**

<img width="870" height="464" alt="image" src="https://github.com/user-attachments/assets/484cff3c-cc9e-42ef-b9bf-3fda4a434756" />


**Unit Pricing, Merit-Order Supply Curve & Chokepoint Analysis**

<img width="734" height="261" alt="image" src="https://github.com/user-attachments/assets/af1541fa-54c8-43bc-ae0f-35e810f4acc0" />

<img width="1568" height="729" alt="image" src="https://github.com/user-attachments/assets/a9455f31-39d7-4e54-80af-f72ad14b50e9" />

<img width="898" height="136" alt="image" src="https://github.com/user-attachments/assets/53c53b9a-2a26-44c6-84ba-c33eecd9a2f3" />
