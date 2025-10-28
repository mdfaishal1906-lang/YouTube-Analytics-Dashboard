# 🎬 YouTube Channel Performance Dashboard (Power BI)

## 📊 Project Overview
This Power BI project analyzes YouTube channel performance to uncover **top-performing videos**, **audience engagement trends**, and **growth patterns** over time.  
The dashboard helps creators and marketers make data-driven decisions about content strategy, posting frequency, and audience targeting.

---

## 🎯 Objectives
- Track key performance metrics such as **views, likes, comments, and subscribers**  
- Identify **top-performing videos and categories**  
- Measure **engagement rate** and analyze trends over time  
- Visualize audience demographics and watch behavior  

---

## 🧩 Dataset
- **Source:** [YouTube Trending Videos Dataset (Kaggle)](https://www.kaggle.com/datasets/datasnaek/youtube-new)  
- **Data Fields:**  
  - Video ID, Title, Category  
  - Publish Time  
  - Views, Likes, Dislikes, Comments  
  - Tags and Channel Title  

*(You can also use your own exported data from YouTube Studio for real-time insights.)*

---

## ⚙️ Tools & Technologies
- **Power BI Desktop** – for dashboard design and DAX calculations  
- **Power Query** – for data cleaning and transformation  
- **Microsoft Excel / CSV** – dataset storage and preparation  
- **DAX (Data Analysis Expressions)** – for custom measures and KPIs  

---

## 🧮 DAX Measures Used
```DAX
Total Views = SUM(YouTube[views])
Total Likes = SUM(YouTube[likes])
Total Comments = SUM(YouTube[comment_count])
Engagement Rate = DIVIDE([Total Likes] + [Total Comments], [Total Views])
Average Views = AVERAGE(YouTube[views])
