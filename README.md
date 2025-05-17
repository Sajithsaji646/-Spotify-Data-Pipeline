
# Spotify Data Pipeline using MySQl & Python 🎵

A mini data engineering + analytics project that extracts Spotify track data using API, processes it using Python, stores it in a MySQL database, and visualizes it using matplotlib.

---

## 📊 Objective
Build an end-to-end data pipeline using real-time Spotify track data for analysis and visualization.

---

## 🔧 Tools & Technologies
- **Python**
- **MySQL**
- **Spotipy** (Spotify Web API)
- **Pandas**
- **Matplotlib**
- **Jupyter Notebook**

---

## 🚀 Workflow

### 1. Spotify Developer Setup
- Created an app on [Spotify Developer Dashboard](https://developer.spotify.com/dashboard)
- Generated `client_id` and `client_secret`
  
>![Screenshot 2025-05-15 191208](https://github.com/user-attachments/assets/c223a600-d673-4f83-9bfe-da4ee7548fa9)

### 2. Data Extraction (API)
- Used `Spotipy` library
- Converted track URLs into JSON format
- Extracted metadata: `track_name`, `artist`, `album`, `popularity`, `duration`

### 3. Data Transformation
- Processed JSON into structured format using `pandas`
- Converted into DataFrame and exported as `CSV`

### 4. Data Visualization
- Created bar charts and histograms using `matplotlib`
- Explored popularity and duration metrics visually

>![Screenshot 2025-05-15 203141](https://github.com/user-attachments/assets/57665f3b-31e8-4f82-b918-5a00dc2f4f24)


### 5. Load into MySQL
- Created a MySQL database: `spotify_db`
- Created a table: `spotify_tracks`
- Inserted cleaned data using `mysql.connector`
- Used a `.txt` file to batch upload track URLs
  
>![Screenshot 2025-05-15 204921](https://github.com/user-attachments/assets/ae067e8a-5997-4947-8b17-d746c5dc4949)


### 6. Analysis
- Performed SQL-based analytics:
  - Most popular tracks
  - Average track duration
  - Most frequent artists
    
  >![Screenshot 2025-05-15 205031](https://github.com/user-attachments/assets/df081b6e-a5fb-448f-9765-1bc6e331e72a)

## 💡 Sample Insights
- Average duration of tracks: `XX mins`
- Most popular track: `"Track Name" by Artist`
- Top 5 artists by frequency and popularity

## 🔄 Future Enhancements
- Integrate Streamlit dashboard
- Add playlist-level analytics
- Automate with Airflow.
