# DishRadar: Dish-Level Restaurant Review Analytics

DishRadar is a business analytics project that analyses customer reviews to identify dish-level sentiment changes, detect emerging restaurant issues, and support data-driven operational decisions.

## Problem Statement

Overall restaurant ratings can hide problems with individual dishes or service areas. DishRadar aims to identify these issues earlier by tracking customer sentiment over time and generating alerts when performance declines.

## Key Features

- **Dish-Level Sentiment Analysis:** Identifies sentiment associated with individual dishes and service aspects.
- **Early-Warning Alerts:** Compares recent sentiment against historical baselines to flag potential problems.
- **Complaint Analysis:** Highlights recurring negative keywords to help explain why sentiment may be declining.
- **Trend Monitoring:** Tracks monthly sentiment changes and compares dish performance over time.
- **Forecasting:** Generates short-term sentiment forecasts and uncertainty intervals.
- **Interactive Dashboard:** Provides dish-level analysis, alerts, forecasting, review testing, and CSV upload functionality.

## Methodology

The project follows a review-processing and monitoring workflow:

1. Preprocesses customer reviews and splits them into clauses.
2. Matches review clauses to dishes and service aspects using keywords and spelling variants.
3. Calculates sentiment scores using a custom positive and negative word lexicon.
4. Aggregates sentiment scores by month.
5. Compares recent performance against historical baselines to identify potential declines.
6. Examines complaint keywords to provide context for alerts.
7. Applies time-series methods to generate short-term forecasts.

## Dataset

The project uses a **simulated dataset of 1,193 restaurant reviews spanning 18 months, from January 2025 to June 2026**, created for the project.

The dataset includes review dates, review text, and star ratings. It was designed to demonstrate how dish-level sentiment monitoring can identify changes that may be hidden by overall restaurant ratings.

## Tools & Technologies

- Python
- Google Colab
- HTML, JavaScript and Chart.js
- Custom lexicon-based sentiment analysis
- Time-series analysis and forecasting

## Key Findings

Using the simulated dataset, DishRadar identified a decline in Chicken Dum Biryani sentiment and generated an alert in January 2026, approximately two months before the overall rating crossed the selected decline threshold in March 2026.

The analysis also highlighted service speed as a persistent issue, demonstrating how dish-level and service-level monitoring can provide more specific insights than an overall star rating.

*These findings demonstrate the system's behaviour on simulated data and do not establish performance on real restaurant reviews.*

## Limitations

- The dataset is simulated and requires validation using real restaurant reviews.
- Sentiment scoring relies on predefined keywords and may miss sarcasm, context, and complex expressions.
- Historical baselines assume that the initial period represents normal performance.
- Low review volumes can make monthly sentiment estimates unreliable.
- Forecasts are subject to uncertainty and require further evaluation.

## Future Improvements

- Validate the system using real restaurant review data.
- Incorporate trained aspect-based sentiment analysis models.
- Improve handling of multilingual reviews.
- Evaluate alert accuracy, false positives, and warning lead time.
- Extend monitoring to multiple restaurant outlets.
- Integrate operational data to investigate potential causes of declining sentiment.

## Project Resources

- **Dashboard:** [Add your deployed dashboard URL]
- **Google Colab Notebook:** [Open the analysis notebook](https://colab.research.google.com/drive/1DeLKP3R00l8rX3qVphnVDvEiUUR3Adm4)
- **Project Report:** See `report.pdf` in this repository.

## Academic Context

Developed as a group capstone project for *Business Transformation using Analytics and AI* at Manipal Academy of Higher Education (MAHE), Bengaluru.

The project involved problem identification, analytical methodology development, dashboard implementation, and interpretation of results. Claude (Anthropic) was used to assist with selected aspects of code and dashboard development, formatting, and result checking.

---

**Disclaimer:** DishRadar is an academic prototype developed for educational purposes. Its findings are based on simulated data and should not be interpreted as validated business predictions.
