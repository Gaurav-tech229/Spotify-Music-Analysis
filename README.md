# Spotify Music Analysis

## 📌 Project Overview
In today’s digital music era, understanding listening behavior is vital for both **streaming platforms** and **music lovers**.  
This project analyzes **Spotify listening history** to uncover **trends in albums, artists, and tracks**, along with **time-based listening patterns**.  

The goal is to answer key business questions such as:
- Which albums, artists, and tracks are most popular?
- How has listening behavior changed over time?
- Are there noticeable differences between weekday and weekend listening?
- At what times of day do people listen to music the most?
- How do different tracks perform in terms of listening time vs frequency?

---

## 📂 Dataset Details
Data is extracted from Spotify’s listening history logs and contains key fields:

| Column Name        | Description |
|--------------------|-------------|
| **spotify_track_uri** | Unique track identifier in Spotify’s database. |
| **ts** | Timestamp when playback stopped (UTC, ISO 8601). |
| **platform** | Device/platform used (`desktop`, `mobile`, `web`, `smart_speaker`). |
| **ms_played** | Listening duration in milliseconds. |
| **track_name** | Name of the song. |
| **artist_name** | Name of the artist. |
| **album_name** | Name of the album. |
| **reason_start** | Reason playback started (`trackdone`, `clickrow`, etc.). |
| **reason_end** | Reason playback ended (`trackdone`, `fwdbtn`, etc.). |
| **shuffle** | Whether shuffle was enabled. |
| **skipped** | Whether the track was skipped. |

---

## 🎯 Analysis & Dashboard Insights

### **1️⃣ Albums Analysis**
**Key Metrics:**
- **Total Albums Played Over Time** – Shows how album engagement has evolved monthly & yearly. (Track monthly & yearly listening trends)
- **Albums per Year** – Detects shifts in listening habits and diversity (min/max values highlight best and worst years). (Identify annual listening habits and find min/max album counts)
- **Weekday vs Weekend Listening** – Determines if users prefer different albums based on day type. (Detect listening pattern differences)
- **Top 5 Albums** – Identifies most frequently played albums. (Based on listening frequency)
- **Year-over-Year (YoY) Growth** – Measures change between the latest and previous year. (Compare LY vs PY and calculate YoY growth)

**Dashboard:**  
![Albums Dashboard](https://github.com/Gaurav-tech229/Spotify-Music-Analysis/blob/main/Dash_Img/album_artist_track.png)  
**Insight:**  
> In 2024, listening shifted heavily towards “÷ (Divide)” with a 25% YoY growth, peaking in weekend plays.

---

### **2️⃣ Artists Analysis**
**Key Metrics:**
- **Total Artists Played Over Time** – Identifies artist popularity trends. (Monthly & yearly listening evolution)
- **Artists per Year** – Measures diversity in music preferences. (Identify artist diversity each year (min/max values))
- **Top 5 Artists** – Reveals favorite artists. (Most played artists)
- **Weekday vs Weekend Patterns** – Captures mood shifts across days. (Find pattern differences)
- **LY vs PY Analysis** – Compares popularity trends. (Artist engagement change with YoY growth)

**Dashboard:**  
![Artists Dashboard](https://github.com/Gaurav-tech229/Spotify-Music-Analysis/blob/main/Dash_Img/album_artist_track.png)  
**Insight:**  
> “Ed Sheeran” dominated 2024 with a 35% YoY increase, especially on Friday evenings.

---

### **3️⃣ Tracks Analysis**
**Key Metrics:**
- **Total Tracks Played Over Time** – Detects periods of high engagement. (Yearly & monthly consumption patterns)
- **Tracks per Year** – Identifies variety in listening. (Annual diversity in track choices (min/max values))
- **Top 5 Tracks** – Reveals most replayed songs. ( Most played tracks)
- **YoY Trend** – Finds growing or declining track popularity. (Track engagement changes with YoY growth)

**Dashboard:**  
![Tracks Dashboard](https://github.com/Gaurav-tech229/Spotify-Music-Analysis/blob/main/Dash_Img/album_artist_track.png)  
**Insight:**  
> “Shape of You” maintained top position for 3 years straight, but new tracks in 2024 showed faster growth.

---

### **4️⃣ Listening Patterns**
**Key Metrics:**
- **Listening Hours Heatmap** – Shows peak times by hour/day.
- **Listening Time vs Frequency Scatter Plot** – Categorizes tracks into:
  - **High Time + High Frequency** → Addictive hits (Most engaging tracks)
  - **Low Time + High Frequency** → Short tracks (Niche but loved tracks)
  - **High Time + Low Frequency** → Deep-focus tracks (Short, frequently played tracks)
  - **Low Time + Low Frequency** → Least engaging (Least popular tracks)

**Dashboard:**  
![Listening Patterns Dashboard](https://github.com/Gaurav-tech229/Spotify-Music-Analysis/blob/main/Dash_Img/listiningpattern.png)  
**Insight:**  
> Listening peaks at **8 PM on weekends**, with niche but long-play tracks dominating late-night sessions.

---

### **5️⃣ Details Grid**
- **Interactive Grid** – Displays Album, Artist, Track details with filtering.
- **Drill Through** – Lets users deep-dive into specific data and export CSV.
- **Hierarchical Navigation** – Drill up/down between album → artist → track.

**Dashboard:**  
![Details Grid](https://github.com/Gaurav-tech229/Spotify-Music-Analysis/blob/main/Dash_Img/detailgrid.png)  
**Insight:**  
> Users can click on “Shape of You” in the grid to see full listening history by platform, day, and time.

---

## 📈 Findings
- Weekend listening is **15% higher** than weekdays.
- Listening peaks at **8 PM**, with smaller peaks around **10 AM**.
- 2024 saw a **20% increase** in unique artists listened to.
- Top albums are **more consistent year-to-year** than top tracks.

---
