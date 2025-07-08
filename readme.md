# SteamSmartBuy 📉🎮

[**SteamSmartBuy**](https://app.powerbi.com/view?r=eyJrIjoiMmJjZDYxYjgtOTNjYS00Y2ZiLTljYmUtYjNmNGVmMjcxODA4IiwidCI6IjE2MDkzNTg2LTFmN2ItNDVhYy1hYTAxLTRjZDRkYzFkNjUwOCIsImMiOjEwfQ%3D%3D) is a smart data analysis dashboard built to help gamers track and discover the best Steam deals. It leverages a combination of API-driven data collection, hands-on data analysis, and visual storytelling through Power BI—helping users make smarter purchasing decisions based on pricing history, discount patterns, and game quality.

---

## 🚀 Try It Out!

Check out the dashboard here:  
[🔗 Power BI Report](https://app.powerbi.com/view?r=eyJrIjoiMmJjZDYxYjgtOTNjYS00Y2ZiLTljYmUtYjNmNGVmMjcxODA4IiwidCI6IjE2MDkzNTg2LTFmN2ItNDVhYy1hYTAxLTRjZDRkYzFkNjUwOCIsImMiOjEwfQ%3D%3D)

---

## 💡 Overview

This project integrates multiple data sources and analytical techniques to create a centralized view of Steam game pricing and deal quality. Our goal is not just to surface discounts—but to evaluate whether a deal is *actually worth it* using historical data, scarcity metrics, and quality scores.

---

## 📊 Features

- 🧠 **Deal Scoring Engine** that evaluates discounts by factoring in current deal depth, historical trends, frequency, and scarcity—alongside game quality indicators.
- 📈 **Price and Deal History Visualization** showing how pricing and discount behavior evolve over time.
- 🔍 **Interactive Power BI Dashboard** for intuitive filtering, scoring, and searching—easily spot the best deals or search for your favorite titles.
- 🔮 **Built for Expansion**, with predictive features (e.g. estimating when the next good deal might arrive) planned in future updates.

---

## 🔧 Architecture

1. **Data Collection & Analysis**:
   - Python scripts handle data gathering and preprocessing.
   - Performed extensive analysis to calculate historical deal strength, frequency, and game review metrics to support the scoring logic.

2. **APIs Used**:
   - 🛒 [**IsThereAnyDeal API**](https://isthereanydeal.com/) – for price logs and deal data across multiple stores.
   - 🧪 [**Steamworks Web API**](https://partner.steamgames.com/doc/webapi) – for metadata, user review rates, and pricing info.
   - 🎮 [**RAWG API**](https://rawg.io/apidocs) – for enhanced Metacritic score access when Steam data is insufficient.

3. **Database (Self-hosted and maintained)**:
   - All data is stored in a **MySQL database hosted on [PlanetScale](https://planetscale.com/)**, self-hosted and maintained directly by the project author.
   - Database schema is modular and normalized for long-term scalability and analytics performance.
   - [**View Database Schema**](./development_notebooks/database_schema.png)

4. **Visualization with Power BI**:
   - Power BI connects directly to the PlanetScale database.
   - Built measures and transformations within Power BI to enable real-time filtering, scoring, and ranking of game deals.

---

## 📬 Contact the Author

If you’d like to get in touch:

- 💻 **Project or code-related inquiries** – Feel free to open an issue on this repo or reach out via email.
- 💼 **Job opportunities or collaborations** – I’m actively seeking roles in data analytics or related fields!

**Email**: [xx2448@columbia.edu](mailto:xx2448@columbia.edu)  
**LinkedIn**: [xx-xiaoxiao](https://www.linkedin.com/in/xx-xiaoxiao/)

---

## ✅ Acknowledgments

Special thanks to the following platforms whose APIs made this project possible:

- **[IsThereAnyDeal](https://isthereanydeal.com/)** – Historical deal records and real-time discount info.
- **[Steamworks Web API](https://partner.steamgames.com/doc/webapi)** – Game details, user reviews, and current pricing.
- **[RAWG API](https://rawg.io/apidocs)** – Expanded metadata including platform-specific Metacritic scores.

---

## 📄 License

This project is open-sourced under the [MIT License](LICENSE).

---