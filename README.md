# 🏨 Hotelytics: Data-Driven Hotel Analytics and Recommendation Dashboard

Hotelytics is an intelligent hotel analytics platform built using **Power BI**, **Python**, and a custom **AI-powered recommendation engine**. It leverages data from over **8,900 hotel entries** scraped across **53 cities in 36 countries**, providing actionable insights into hotel services, pricing, ratings, and room types. 

This project demonstrates the complete data science lifecycle — from **web scraping and data cleaning** to **advanced visual analytics** and **machine learning integration**.

---

## 📊 Project Dashboard (Power BI)
> Fully interactive report available in Power BI (.pbix)

- Dynamic filtering by city, country, stars, ratings, price, room type, services, smoking status, and more.
- Key Performance Indicators (KPIs): Total hotels, average room price, guest rating, star rating, service availability.
- Interactive AI-based hotel recommendation panel powered by **TF-IDF & Cosine Similarity**.
- Drill-through capability to explore hotel-level room details, reviews, and amenities.

---

## ✨ Features

- 🌍 Web scraping from **Expedia** for global hotel data
- 🧼 Advanced data cleaning with Power Query and Python
- 🧠 AI-based hotel recommendation using **TF-IDF + Cosine Similarity**
- 🧾 Multi-table **star schema** architecture for optimized querying
- 📈 Fully dynamic and interactive **Power BI dashboard**
- 📊 Visuals include:
  - Tree maps, scatter plots, bar charts, KPI cards, and influencer charts
  - Insights on room pricing, guest satisfaction, and service popularity

---

## 🔍 Use Case

Ideal for:

- Hospitality analysts looking to identify pricing trends
- Tourists seeking best hotels based on dynamic filters
- Business stakeholders seeking data-driven investment decisions
- Developers & data scientists as an end-to-end data analytics project reference

---

## 🛠️ Technologies Used

| Tool | Purpose |
|------|---------|
| **Python (Selenium, pandas)** | Web scraping & preprocessing |
| **Power BI** | Data cleaning, transformation, dashboarding |
| **Power Query** | Service name standardization, column parsing |
| **TF-IDF & Cosine Similarity** | Content-based recommendation system |
| **GitHub** | Version control & collaboration |

---

## 🧠 AI Recommendation Engine

The model ranks hotels based on:

- City  
- Price range  
- Star rating  
- Guest rating  
- Amenities  
- Room type  
- Smoking status  

**Why TF-IDF?**

| Model | Suitability |
|-------|-------------|
| TF-IDF + Cosine Similarity | ✅ Lightweight, interpretable, no user history needed |
| Collaborative Filtering | ❌ Requires past user behaviour |
| Neural Networks | ❌ Overkill, low interpretability |
| Hybrid Systems | ❌ Too complex for initial phase |

---

## 🧹 Data Processing Steps

1. **Scraping** hotel data per city via Selenium
2. **Cleaning** & parsing data:
   - Standardizing room names, prices, amenities
   - Handling missing star ratings and guest reviews
   - Extracting structured info from unstructured "Offers"
3. **Room categorization**:
   - Room type (e.g., Suite, Deluxe)
   - Bed type (e.g., King, Twin)
   - View (Sea View, City View)
   - Smoking status
4. **Price Bucketization**:
   - Budget (<$100)
   - Economy ($100–$200)
   - Standard ($200–$500)
   - Premium ($500–$1000)
   - Luxury & Ultra Luxury (>$1000)

---

## 🗂️ Data Architecture

A **star schema** was used to build relational models in Power BI:

- **Fact Table**: Property Offers (rooms, prices)
- **Dimension Tables**:
  - Hotels (stars, rating, location, services)
  - Location (city, country)
  - Services (mapped & standardized)
  - Room details (bed, smoking, view)

---

## 📌 Key Insights

- 🔝 **Premium Rooms** and **Suites** are the most common room types.
- 💰 High guest ratings correlate with **Economy** and **Luxury** price ranges.
- 📍 Cities like **Rome**, **London**, and **Bali** have dense hotel availability.
- 💬 **Breakfast, WiFi, and Parking** services influence positive reviews.
- 📈 Price drops often correlate with improved review sentiment.

---

## 🧩 Challenges & Solutions

| Challenge | Solution |
|----------|----------|
| Dynamic web pages | Used `Selenium` with wait controls |
| Inconsistent room data | Used Power Query text parsing |
| Outliers in price | Applied cleaning and filtering |
| Dashboard performance | Used star schema + query optimization |

---

## 📚 Learning Outcomes

- End-to-end data pipeline experience
- Dashboard design and interactivity (filters, drill-throughs)
- TF-IDF based AI systems for real-world data
- Data wrangling with both Python and Power BI
- Agile team collaboration and reporting

---

## 🚀 Future Enhancements

- 🌐 **Live data feed** integration (via APIs)
- 🧠 **Sentiment analysis** on guest reviews using NLP
- 📱 **Mobile-optimised dashboard**
- 🤖 **Hybrid ML models** (Collaborative + Content-based)
- 🧭 **Geospatial analysis** for proximity insights
- ☁️ **Cloud hosting** (Azure/AWS) for scalability
- 🗣️ **Voice/Chatbot interface** for accessibility

---

## 👨‍💻 Team

- Ghazal E Ashar (2112143)  
- Shahzeb Ahmed Iqbal (2112166)  
- Mohammad Ali Hassan (2112148)  
- Muhammad Ammar Thahim (2112247)  
- Usama Habib (2112168)

Project submitted for **CSC4818 Data Sciences**  
Supervised by **Dr Imran Amin** & **Sir Muhammad Ahsan Nisar**

---

## 📎 License

This project is for academic use only. Please contact the authors for any reuse or collaboration proposals.

---
