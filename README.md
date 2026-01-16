# Netflix Analytics: From Data Insights to Vector-Based Recommendations
## 📌 Project Overview

Author: Mubeen Akhund  
Focus: Data Cleaning, Exploration, basic Feature Enginerring, One-Hot Encoding and Understanding  

This project explores the Netflix library through 40+ analytical lenses and implements a Content-Based Recommender System. It demonstrates a full data science pipeline: from fixing "messy" data anomalies to mapping movie metadata into a high-dimensional vector space for real-time similarity retrieval.

## 📊 Key Highlights
***Anomalous Data Correction:*** Identified and resolved "feature-swapped" columns where duration and rating values were mismatched.

***Exploratory Insights:*** Discovered a 2015 "content pivot" and confirmed a statistically significant relationship between audience maturity (TV-MA) and content duration.

***Mathematical Modeling:*** Engineered a 36-dimensional feature matrix using One-Hot Encoding and Min-Max scaling.

## 🧠 Technical Deep Dive: Backend Logic
Following my core development philosophy, here is how the recommendation engine functions at a hardware and logical level:

**The "Brain" of the Recommender: Vector Space Alignment**

sim_matrix = cosine_similarity(genre_features)

## The Backend Process:
***Vector Mapping:*** The backend treats each movie not as a string, but as a Coordinate in a 36-dimensional universe.

***Dot Product Calculation:*** To find similarity, the CPU calculates the Dot Product of two vectors. This measures how much the "arrows" overlap in direction.

***Angular Distance:*** By dividing the dot product by the product of magnitudes, the logic isolates the Cosine Angle.

1.0 (Perfect Alignment): Identical genre/length profiles.

0.0 (Orthogonal): No common attributes.


## 🛠️ How to Run

**Clone the repository:**

git clone https://github.com/AkhundMubeen/Netflix-Deep-EDA-and-Content-Based-Recommendation-Engine.git

**Install Dependencies:**

pip install pandas numpy scikit-learn matplotlib seaborn

**Open the Notebook:** 

Launch Netflix_EDA_Notebook.ipynb in Jupyter or Colab 

## 📂 Dataset
The data is sourced from the Kaggle Netflix Movies and TV Shows dataset. It includes over 8,800 records of content available on the platform as of 2021.

Raw Dataset Link: (https://www.kaggle.com/datasets/shivamb/netflix-shows/code?datasetId=434238&sortBy=dateRun&tab=profile&excludeNonAccessedDatasources=false)

## 📝 Conclusion
This project successfully bridges the gap between raw data and automated decision-making. By leveraging Linear Algebra and Feature Engineering, I have created a scalable system that moves beyond simple search filters to provide mathematically-backed recommendations.

Author: Mubeen Akhund

Focus: Data Science & Machine Learning Implementation
