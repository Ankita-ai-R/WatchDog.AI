# 📊 Log Analytics Report

This report includes visual insights extracted from system logs using AI techniques such as sentiment analysis, log severity classification, and alert detection. It complements the main ML pipeline of the project.

---

##  Sentiment Analysis

We used **TextBlob** to detect the emotional tone of each log message. Polarity scores were categorized as:

- 😊 **Positive** → system health, successful operations  
- 😐 **Neutral** → info/debug messages, no clear emotion  
- 😞 **Negative** → potential issues, failures, or alerts


### 🔍 Distribution Overview

| Sentiment | Description              |
|-----------|--------------------------|
| Positive  | Smooth logs, no action   |
| Neutral   | Informative              |
| Negative  | Investigate immediately  |

---
### Sample's Sentiment Analysis Prediction :

### 🎯 Sample Dual Prediction Output

This graph shows how the system classifies two sample emotional log messages based on severity and sentiment:

![Dual Prediction Plot](assets/sample_dual_plot.png)
 

### 📊 Bar Chart

![Bar Chart - Sentiment](assets/sentiment_bar_chart.png)

---

### 🥧 Pie Chart

![Pie Chart - Sentiment](assets/sentiment_pie_chart.png)

---

## 🚨 Severity-Based Alert Classification

In parallel, we trained a machine learning model (Logistic Regression) to classify logs into:

- `INFO`
- `WARNING`
- `ERROR`
- `CRITICAL`

![Alert PLot - Sentiment](assets/content/alert_distribution.png)

### 💫 Performance Summary:

| Metric     | Value (approx) |
|------------|----------------|
| Accuracy   | ~55% (demo data) |
| F1-score   | ~54% macro avg  |
| Technique  | TF-IDF + Stratified K-Fold |

> ⚠️ _This performance is based on a small, demo-scale dataset. Easily extendable to real-world logs for production-ready accuracy._

---

##  Combined Intelligence

| Log Message                        | Severity | Sentiment |
|------------------------------------|----------|-----------|
| "Service crashed unexpectedly."    | CRITICAL | Negative  |
| "System booted successfully."      | INFO     | Positive  |
| "Disk space low."                  | WARNING  | Neutral   |

> 💡 *The combo of severity + sentiment lets humans prioritize with more empathy and efficiency.*

---

##  Future Scope

- Use larger real-time log datasets
- Plug into cloud logging systems
- Add intent classification + cause prediction

---

## 🔗 Back to Main Project  
👉 [View Main README](README.md)
#for readme: 📑 [Log Analytics Report](Log_Analytics_Report.md)


---

> 💖 Created with love & Python  🌈
