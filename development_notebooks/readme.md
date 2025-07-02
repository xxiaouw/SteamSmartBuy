# 🧪 Jupyter Notebooks – Development & Data Pipeline

This folder contains the core Jupyter notebooks used throughout the development and testing phases of the **SteamSmartBuy** project. Each notebook plays a key role in data collection, cleaning, transformation, and preparation for dashboard integration.

---

## 📓 Notebook Descriptions

### 1. `data_collection.ipynb`
- **Purpose**: Handles the initial retrieval of game data from external APIs.
- **APIs Used**: IsThereAnyDeal, Steam, RAWG.
- **Tasks**:
  - Querying APIs using game titles.
  - Collecting price history, reviews, metadata.
  - Performing simple cleaning and formatting.

---

### 2. `table_generation.ipynb`
- **Purpose**: Performs in-depth data processing and organizes cleaned data into structured formats ready for SQL.
- **Tasks**:
  - Deduplication and deal logic cleanup.
  - Merging and aligning across data sources.
  - Prepares normalized tables suitable for relational database ingestion.

---

### 3. `score_calculation.ipynb`
- **Purpose**: Implements core business logic for calculating deal and game scores.
- **Tasks**:
  - Normalize various metrics (e.g. review rates, deal scarcity).
  - Compute weighted scores for game quality and deal quality.
  - Create the final `score` tables used in the dashboard.

---

### 4. `SQL_connection.ipynb`
- **Purpose**: Handles database operations to sync data with our production MySQL instance on PlanetScale.
- **Tasks**:
  - Establishes MySQL connection.
  - Creates or updates SQL tables.

---

## 🗂 How They Work Together

1. **`data_collection.ipynb`** gathers raw data  
2. → **`table_generation.ipynb`** cleans & organizes it  
3. → **`score_calculation.ipynb`** computes deal index  
4. → **`SQL_connection.ipynb`** pushes results to the database  

These notebooks together power the backend pipeline that supports the Power BI dashboard and ongoing deal analysis.

---