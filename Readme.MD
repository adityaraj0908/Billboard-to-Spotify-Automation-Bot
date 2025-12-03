# 🎵 Billboard to Spotify Automation Bot

A Python automation project that scrapes the **Billboard Hot 100** songs for any selected date and automatically creates a **Spotify playlist** with those songs using the **Spotify Web API**.

This project demonstrates:

* ✅ Web Scraping (BeautifulSoup)
* ✅ API Integration (Spotify Web API)
* ✅ Automation
* ✅ Secure Environment Variable Management

---

## 🚀 Features

* Scrape Billboard Hot 100 chart for any historical date
* Automatically create a private Spotify playlist
* Search each scraped song on Spotify
* Add all available tracks to the playlist automatically
* Secure API authentication using environment variables

---

## 🛠️ Tech Stack

* **Python 3.10+**
* **Requests** – for fetching Billboard HTML
* **BeautifulSoup (bs4)** – for web scraping
* **Spotipy** – Python wrapper for Spotify Web API
* **python-dotenv** – for managing environment variables

---

## 📂 Project Structure

```
Billboard-to-Spotify-Automation-Bot/
│
├── main.py                  # Main automation script
├── .env                     # Environment variables (NOT committed)
├── .gitignore               # Ignored files
└── README.md                # Project documentation
```

---

## 🔑 Spotify API Setup (One-Time)

1. Go to the Spotify Developer Dashboard:

```
https://developer.spotify.com/dashboard
```

2. Create a new app

3. Copy:

* Client ID
* Client Secret

4. Add this Redirect URI in the app settings:

```
http://localhost:8888/callback
```

---

## ⚙️ Environment Variables (.env)

Create a `.env` file in the project root with the following content:

```
SPOTIFY_CLIENT_ID=your_client_id_here
SPOTIFY_CLIENT_SECRET=your_client_secret_here
SPOTIFY_REDIRECT_URI=http://localhost:8888/callback
```

⚠️ Do NOT commit this file to GitHub.

---

## 📦 Installation

### 1. Create and activate virtual environment

```bash
python -m venv venv
venv\Scripts\activate
```

### 2. Install dependencies

```bash
pip install requests bs4 spotipy python-dotenv
```

---

## ▶️ How to Run the Project

Run the main script:

```bash
python main.py
```

Enter a date in this format when prompted:

```
YYYY-MM-DD
```

Example:

```
2005-08-12
```

✅ A private Spotify playlist will be created automatically with the Top 100 songs of that date.

---

## 🧠 What This Project Demonstrates

* Real-world web scraping
* OAuth-based API authentication
* End-to-end automation
* Secure handling of API keys
* Practical integration of scraping + APIs

