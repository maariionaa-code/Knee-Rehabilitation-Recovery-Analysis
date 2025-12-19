# Knee-Rehabilitation-Recovery-Analysis
This project analyzes my knee rehabilitation recovery using real, self-collected data recorded daily after surgery. The goal is to apply core Data Mining, Time Series Analysis, and Machine Learning techniques to understand recovery patterns, identify effective rehabilitation behaviors, and predict future knee flexion.

1. Goal
  The goal of this project is to analyze my knee rehabilitation process using data science techniques in order to better understand recovery patterns over time. After undergoing knee     surgery,I collected daily measurements such as pain levels, maximum knee flexion, and rehabilitation activity. As a data science student, this project allowed me to apply data mining   techniques learned in class to a real and personally meaningful problem. The main objectives were to:
  - Explore recovery trends over time.
  - Identify unusual or problematic recovery days.
  - Discover associations between pain, activity, and progress.
  - Build simple predictive models for knee flexion.

2. Methods
  The dataset was manually collected over several weeks during rehabilitation. Each observation includes: date and time, maximum knee flexion, pain level, whether rehabilitation or       exercise was performed, days since surgery. Additional features were derived to capture recovery dynamics: daily change in flexion, daily change in pain, normalized flexion values      for comparison over time.

  Exploratory data analysis was performed using time-series plots, scatter plots, and boxplots. Similarity and clustering techniques (K-Means with PCA) were used to identify groups of    similar recovery days. Outlier detection was conducted using three methods taught in the course: extreme-value (Z-score), probability-density (KDE), and density-based approaches.       Association rule mining was implemented to uncover relationships between pain, activity, and recovery progress. Finally, linear regression and random forest models were trained to      predict knee flexion based on time since surgery.

3. Results
  The analysis revealed an overall upward trend in knee flexion over time, with temporary setbacks often associated with increased pain. Clustering identified three main types of         recovery days: high-progress days with exercise, intense rehabilitation days with higher pain, low-activity or regression days.

  Outlier detection consistently highlighted a small set of days corresponding to unusually intense rehabilitation sessions or potential setbacks. Association rule mining showed strong   relationships between exercise and flexion improvement, as well as between rehabilitation and exercise. Linear regression achieved moderate predictive performance, while the random     forest model performed poorly due to the small dataset size and limited temporal depth.

4. Conclusions
  This project demonstrates how data science techniques can provide objective insight into a highly personal recovery process. By analyzing my own rehabilitation data, I applied          clustering, outlier detection, association rule mining, and predictive modeling to real-world time-series data.

  The results highlight the importance of consistent exercise and show that high-effort days do not always correspond to immediate improvement. Personally, this project helped me         better understand my own recovery and reinforced my interest in applying data science to health-related problems.

5. Future work
  Future extensions of this project could include longer data collection periods and more advanced time-series models. Additionally, having undergone the same surgical procedure on       both knees, a comparative analysis between both recovery processes could provide valuable insights into how recovery differs despite identical surgeries.

6. Gen AI statement
  Generative AI (ChatGPT) was used as a support tool during this project to assist with code structuring, debugging, and refining the project direction. All analysis decisions and        interpretations were made by the author.

7. How to run this project
- Clone repository: git clone https://github.com/your-username/Knee-Rehabilitation-Recovery-Analysis.git
cd knee-rehabilitation-analysis
- Install the required libraries: pip install pandas numpy matplotlib seaborn scikit-learn scipy (you can run the requirements file).
- Run the jupyter notebook: jupyter notebook
- Open the notebook: notebooks/knee_rehabilitation.ipynb
- Notes: The project was developed using Python. The dataset is included in the repository and all results are fully reproducible by running the notebook from top to bottom.
