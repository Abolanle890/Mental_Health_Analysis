# Mental_Health_Analysis

# 🧠 Mental Health Analysis

This project explores a dataset on mental health to understand how various factors—such as sleep, diet, work hours, screen time, social interaction, and stress—correlate with mental well-being across different demographics and countries.

## 📂 Dataset
  - Age, Gender, Country
  - Mental Health Condition
  - Happiness Score
  - Work Hours per Week
  - Sleep Hours
  - Screen Time
  - Stress Level (Low, Moderate, High)
  - Diet Type (Balanced, Junk Food, Vegan, etc.)
  - Social Interaction Score

## 📊 Dashboard Overview

Power BI dashboard contains:

1. **Happiness Score by Country**
2. **Happiness Score by Diet Type**
3. **Sleep Hours & Screen Time by Gender**
4. **Work Hours by Mental Health Condition**

---

## 📈 DAX Measures

All calculated fields and measures used in Power BI are stored in the [`dax/calculated_measures.dax`](dax/calculated_measures.dax) file.

Example:

```DAX
Average Happiness = AVERAGE('MentalHealthData'[Happiness Score])


## 📊 Visualizations Included

### 1. Happiness Score by Country
- **Description**: Compares the average happiness score across countries.
- **Insight**: Countries like the USA, Australia, and Canada report higher average happiness compared to countries like Brazil and Germany.
- **DAX Used**:
  ```DAX
  Average Happiness Score = AVERAGE('MentalHealthData'[Happiness Score])
2. Happiness Score by Diet Type
Description: Donut chart showing average happiness scores across different diet types (e.g., Balanced, Junk Food, Vegan).

Insight: People on a balanced diet or vegetarian diet tend to report slightly higher happiness.

DAX Used:

DAX
Copy
Edit
Average Happiness by Diet = AVERAGE('MentalHealthData'[Happiness Score])
3. Sleep Hours and Screen Time by Gender
Description: Clustered bar chart comparing average sleep hours and screen time across genders.

Insight: Females report slightly higher sleep hours; screen time is consistent across genders.

DAX Used:

DAX
Copy
Edit
Average Sleep Hours = AVERAGE('MentalHealthData'[Sleep Hours])
Average Screen Time = AVERAGE('MentalHealthData'[Screen Time])
4. Work Hours per Week by Mental Health Condition
Description: Line chart showing how work hours vary with different mental health conditions (Anxiety, PTSD, Depression, etc).

Insight: Individuals with bipolar disorder work the fewest hours on average, followed by those with depression.

DAX Used:

DAX
Copy
Edit
Average Work Hours = AVERAGE('MentalHealthData'[Work Hours])
5. Filter Options
Age

Mental Health Condition

Stress Level

Diet Type

These slicers help users drill down into specific subgroups to explore deeper insights.

📁 Files
mental_health_dashboard.pbix – Power BI report file

README.md – Dashboard documentation

🚀 Future Improvements
Include gender vs mental condition ratio

Add correlation analysis between multiple factors

Integrate exercise data when available

🧠 Summary of Insights
Work Hours: Fewer work hours are associated with severe mental health conditions.

Diet: Balanced diets correlate with higher happiness scores.

Country: USA, Australia, and Canada lead in happiness metrics.

Gender: Minimal variation in screen time, with females slightly ahead in sleep.

💬 Questions Addressed
❌ Ratio of mental condition by gender: Not yet visualized.

✅ Work hours vs. mental health: Covered in line chart.

❌ Combined contribution of sleep, diet, stress, interaction, screen time: Partially covered. Could improve with a correlation matrix or scatter plots.

✅ Happiness by country: Fully covered.
