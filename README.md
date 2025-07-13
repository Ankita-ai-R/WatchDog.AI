# WatchDog.AI
✨An AI-powered log monitoring system that detects severity levels 🚨(INFO, WARNING, ERROR, CRITICAL) and analyzes the emotional sentiment of system logs using NLP. Built using Scikit-learn, TextBlob, and visualized with Matplotlib.✨ Ideal for IT teams, professionals, students, and developers who want smarter, empathy-driven log alerts.  😊

## Sentiment Analysis of Log Messages :-

To add emotional intelligence to traditional log severity detection, this project includes a **TextBlob-powered sentiment analysis** component.

Each log message is analyzed for its **polarity score**, and categorized into:

- 😊 **Positive** — Likely to be safe/normal messages  
- 😐 **Neutral** — Informative but emotionally neutral  
- 😞 **Negative** — Often correlate with failures, crashes, or alerts

### 📊 Visualized Sentiment Distribution

![Sentiment Chart](/content/assets/sentiment_bar_chart.png)

> 💡 *This analysis helps prioritize which logs may require human attention based on emotional tone in addition to severity level.*

---
![Sentiment Chart](assets/sentiment_chart.png)

## 📊 Analytics

This project also includes sentiment and severity analytics of logs.

### 🎯 Sample Dual Prediction Output

This graph shows how the system classifies two sample emotional log messages based on severity and sentiment:

![Dual Prediction Plot](assets/sample_dual_plot.png)


📊 [View full log analytics report here](Log_Analytics_Report.md)
