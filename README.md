# Strava Exploratory Data Analysis and Data Science Project

This is a mini data science project that focuses on data collected from Strava's API, an app that creates unique activity tracking for athletes.  

This project had two primary research questions:

1) Can we measure the intensity of a workout (taking into account distance and speed)?

To address this question, we created an "intensity score", that was loosely based off TSS and rTSS (Training stress scores).  

Our formula was as follows: (ElapsedTime(s) * NP * NP/FTP) / (ElapsedTime(s) * FTP) * Total Distance (m)
- NP stands for normalized power and was calculated as: Average speed (m/s) * (Elevation Gain / Total Distance)
- FTP stands for Power Threshold and was calculated as: Max Speed (m/s) * (Elevation Gain / Total Distance)

2) Which countries have the most efficient bike workouts when considering the workout time, moving time, and kilojoules burned. 

For addressing this question we created another measure for "efficiency" which multiplied the ratio of KJ to distance with the ratio of moving time to the total workout time. 

**Note: This project was completed as an assignment for a class and should not be used as a basis of forming any definitive conclusions.  The deliverable for this assignment was to submit a report with conclusions, however it's a project focused primarily on EDA (exploratory data analysis) and a little modeling**
