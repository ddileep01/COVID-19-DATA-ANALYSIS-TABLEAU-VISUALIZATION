## COVID-19 Data Analysis Dashboard  
**Course:** Data Visualization & Interpretation

---

### **Overview**

This project presents a Tableau dashboard analyzing the spread and impact of COVID-19 across India, with a focus on trends relevant to engineering college students as campuses plan to reopen. The dashboard leverages data visualization best practices to inform and empower students to make safe, data-driven decisions during the ongoing pandemic[1].

---

### **Problem Statement**

COVID-19, caused by SARS-CoV-2, has significantly disrupted life worldwide. As of September 2020, India faced millions of cases and a national lockdown. With educational institutions considering reopening, there is a need for clear, accessible data to help students understand the risks and trends associated with the pandemic[1].

---

### **Audience**

- **Primary Audience:** Engineering college students
- **Persona:** A final-year student anxious about returning to campus and seeking to understand safety and risk factors
- **Audience Concerns:**
  - Trends in COVID-19 cases in their state
  - Safety of attending offline classes
  - Understanding pandemic evolution and its impact on education
  - Making informed decisions about returning to campus
  - Awareness of preventive measures and risk zones[1]

---

### **Objectives**

- Demonstrate the context and importance of COVID-19 data visualization
- Raise awareness about the seriousness of the pandemic using data-driven insights
- Enable informed decision-making regarding campus attendance and safety protocols
- Encourage adherence to health guidelines to minimize risk[1]

---

### **Big Idea**

> Understanding India's COVID-19 trends through interactive visualizations empowers students to make informed decisions as they return to campus post-lockdown[1].

---

### **Key Questions Addressed**

1. **How has the number of COVID-19 active cases changed over time in different regions?**
2. **Which states in India have been most affected by COVID-19?**
3. **How have COVID-19 recovery trends varied over time in India?**[1]

Each question is answered through a dedicated Tableau visualization.

---

### **Data Preparation**

- Data was preprocessed to create an "Active Adjustment" column using the formula:
  ```
  IF [Status] = "Confirmed" THEN [Count]
  ELSEIF [Status] = "Recovered" THEN -[Count]
  ELSEIF [Status] = "Deceased" THEN -[Count]
  ELSE 0
  END
  ```
- Additional preprocessing was performed as needed for clean, analysis-ready datasets[1].

---

### **Visualizations & Design Rationale**

| Visualization                           | Type                        | Purpose & Rationale                                                                                              | Gestalt Principles Used                     | Pre-attentive Attributes Used           |
|------------------------------------------|-----------------------------|------------------------------------------------------------------------------------------------------------------|---------------------------------------------|-----------------------------------------|
| COVID-19 Active Cases Trend by State     | Multi-Line Time Series Chart| Compare trends across states over time; highlight peaks and responses                                            | Similarity, Continuity, Proximity           | Colour (hue), Position, Orientation     |
| State-wise Spread of COVID-19 in India   | Symbol Map (Geo Map)        | Show geographic distribution and severity of cases; enable quick regional comparison                             | Proximity, Similarity, Enclosure, Figure/Ground | Colour gradient, Position, Shape        |
| India's COVID-19 Recovery Journey        | Line Chart (Time Series)    | Track recovery trends over time; visualize rises, peaks, and plateaus                                            | Continuity, Figure/Ground, Enclosure        | Position, Length/Size, Orientation      |

---

### **Disclaimer**

> I am a data visualization student, not an infectious disease expert or epidemiologist. This dashboard was created only to fulfill the academic requirements of the course and should not be used for medical decision making. I bear no responsibility towards the correctness of the data[1].

---
![WhatsApp Image 2025-06-16 at 10 50 17 AM](https://github.com/user-attachments/assets/7684218b-866b-4ede-8c09-fbd0a87da7c1)
![WhatsApp Image 2025-06-16 at 10 50 17 AM (2)](https://github.com/user-attachments/assets/8c2ff5f7-c749-4eef-9bae-7833a99076aa)
![WhatsApp Image 2025-06-16 at 10 50 17 AM (1)](https://github.com/user-attachments/assets/af43fad8-2849-49eb-a620-0fb826b98284)

