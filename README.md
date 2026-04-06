# trendpulse-saranya

# 🚀 TrendPulse — What's Actually Trending Right Now

TrendPulse is a data pipeline project that fetches, processes, analyzes, and visualizes trending Reddit posts in real time using the official Reddit Data API.

---

## 📌 Project Overview

This project demonstrates how to build an end-to-end data pipeline using Python. It collects trending posts from Reddit, cleans and processes the data, performs analysis, and generates visual insights.

The goal is to simulate a real-world data engineering workflow using publicly available data.

---

## ⚙️ Features

* 🔐 OAuth-based authentication using Reddit API
* 📡 Fetch trending posts from r/popular and selected subreddits
* 🧹 Data cleaning and transformation using Pandas
* 📊 Data analysis using NumPy and Pandas
* 📈 Visualization using Matplotlib
* 🔄 Real-time pipeline with periodic updates
* ⚡ Token caching for efficient API usage

---

## 🏗️ Project Structure

```
trendpulse/
│
├── auth.py              # Handles OAuth token generation and caching
├── fetch_data.py        # Fetches data from Reddit API
├── clean_data.py        # Cleans and processes raw data
├── analyze_data.py      # Performs analysis
├── visualize_data.py    # Generates charts
│
├── data/
│   ├── raw_posts.json
│   ├── cleaned_posts.csv
│   ├── token_cache.json
```

---

## 🔑 Authentication (Reddit API)

This project uses Reddit’s OAuth2 `client_credentials` flow for application-only access.

Steps:

1. Create a Reddit app (type: **script**)
2. Obtain:

   * `client_id`
   * `client_secret`
3. Store them securely in your environment or config file

---

## ▶️ How to Run

### 1. Install dependencies

```
pip install requests pandas numpy matplotlib
```

### 2. Add your credentials

Update `auth.py`:

```python
CLIENT_ID = "your_client_id"
CLIENT_SECRET = "your_client_secret"
```

### 3. Run the pipeline

```
python fetch_data.py
python clean_data.py
python analyze_data.py
python visualize_data.py
```

---

## 📊 Example Output

* Top trending subreddits
* Engagement metrics (score + comments)
* Score distribution histogram
* Bar charts of trending topics

---

## 🧠 Learning Objectives

* Understand OAuth2 authentication
* Work with REST APIs
* Build modular Python pipelines
* Perform data cleaning and analysis
* Visualize real-world data

---

## ⚠️ Disclaimer

This project uses Reddit’s public Data API and complies with their usage policies.
It is intended for educational and non-commercial purposes only.

---

## 🔮 Future Improvements

* 🌐 Streamlit dashboard for live visualization
* 🧠 NLP-based trend detection (keywords/topics)
* 🗄️ Database integration (SQLite/PostgreSQL)
* ⚡ Async data fetching for performance

---

## 👨‍💻 Author

Saranya

---

## ⭐ Acknowledgements

* Reddit Data API
* Python ecosystem (Requests, Pandas, NumPy, Matplotlib)
