# Steam Games Analytics & Prediction

## Predicting Game Popularity and User Satisfaction using Machine Learning

**Course Assignment 1 | Supervised Machine Learning**
**Supervisor:** Prof. Raja Hashim Ali

---

##  Project Overview

This project applies supervised machine learning and data analysis techniques to the Steam Games dataset to study **game popularity, engagement, and user satisfaction**.

The goal is to understand how factors such as pricing, discounts, genres, multiplayer features, and reviews influence game performance. In addition, predictive models are built to estimate **game popularity (peak concurrent users)**.

The project is structured around seven research questions covering behavioral analysis, feature relationships, and predictive modeling.

---

##  Dataset

| Attribute   | Details                                                         |
| ----------- | --------------------------------------------------------------- |
| **Name**    | Steam Games Dataset                                             |
| **Source**  | https://www.kaggle.com/datasets/artermiloff/steam-games-dataset |
| **Rows**    | ~89,000                                                         |
| **Columns** | ~47                                                             |
| **Domain**  | Gaming Analytics                                                |

###  Target Variables

| Type                     | Variable                              |
| ------------------------ | ------------------------------------- |
| **Primary (Regression)** | `peak_ccu` (Peak Concurrent Users)    |
| **Secondary**            | `pct_pos_total` (User Satisfaction %) |

###  Key Features

* Price, Discount
* Genres, Categories
* Playtime (average, recent)
* Reviews (recent & total)
* Metacritic score
* Estimated owners

---

## Repository Structure

```bash
steam-games-ml-assignment/
│
├── RQ1-checkpoint.ipynb
├── RQ2-checkpoint.ipynb
├── RQ3-checkpoint.ipynb
├── RQ4-checkpoint.ipynb
├── RQ5-checkpoint.ipynb
├── RQ6-checkpoint.ipynb
├── RQ7-checkpoint.ipynb
│
├── figures/
├── tables/
│
├── requirements.txt
└── README.md
```

---

##  Research Questions

| #   | Research Question                                                  | Notebook             |
| --- | ------------------------------------------------------------------ | -------------------- |
| RQ1 | How does pricing affect user engagement and satisfaction?          | RQ1-checkpoint.ipynb |
| RQ2 | What is the impact of discounts on player activity and popularity? | RQ2-checkpoint.ipynb |
| RQ3 | Do critically acclaimed games align with user satisfaction?        | RQ3-checkpoint.ipynb |
| RQ4 | How do game genres influence engagement and success?               | RQ4-checkpoint.ipynb |
| RQ5 | Does multiplayer functionality drive higher engagement?            | RQ5-checkpoint.ipynb |
| RQ6 | What factors predict game popularity (peak_ccu)?                   | RQ6-checkpoint.ipynb |
| RQ7 | Are recent reviews more positive than overall reviews?             | RQ7-checkpoint.ipynb |

---

##  Models Used

* Linear Regression
* Decision Tree
* k-Nearest Neighbors (k-NN)
* Random Forest
* XGBoost
* Support Vector Regression (SVR)

---

##  How to Run on Kaggle

1. Go to https://www.kaggle.com and log in
2. Open dataset:
   https://www.kaggle.com/datasets/artermiloff/steam-games-dataset
3. Click **New Notebook**
4. Upload the `.ipynb` files
5. Use dataset path:

```
/kaggle/input/steam-games-dataset/
```

6. Click **Run All**

> Each notebook is independent and can be run separately.

---

Generated Outputs

Figures

| File                              | Description                          | RQ  |
| --------------------------------- | ------------------------------------ | --- |
| Figure_1_1_class_distribution.png | Engagement/satisfaction distribution | RQ1 |
| Figure_2_1_discount_effect.png    | Discount vs activity                 | RQ2 |
| Figure_3_1_critic_vs_user.png     | Metacritic vs user comparison        | RQ3 |
| Figure_4_1_genre_analysis.png     | Genre impact visualization           | RQ4 |
| Figure_5_1_multiplayer.png        | Multiplayer vs single-player         | RQ5 |
| Figure_6_1_prediction.png         | Model prediction performance         | RQ6 |
| Figure_7_1_review_trends.png      | Review sentiment trends              | RQ7 |

---

Tables

| File                      | Description              | RQ  |
| ------------------------- | ------------------------ | --- |
| Table_1_1_pricing.csv     | Pricing vs engagement    | RQ1 |
| Table_2_1_discount.csv    | Discount impact          | RQ2 |
| Table_3_1_scores.csv      | Critic vs user scores    | RQ3 |
| Table_4_1_genres.csv      | Genre comparison         | RQ4 |
| Table_5_1_multiplayer.csv | Multiplayer analysis     | RQ5 |
| Table_6_1_model.csv       | Prediction model results | RQ6 |
| Table_7_1_reviews.csv     | Review trend comparison  | RQ7 |

---

 Key Findings

* Lower-priced games tend to have higher engagement but mixed satisfaction
* Discounts create short-term spikes in player activity
* Critic scores do not always match user opinions
* Genres strongly influence both engagement and popularity
* Multiplayer features generally increase player engagement
* Machine learning models can effectively predict popularity
* Review trends reveal changes in player perception over time

---

Requirements

See `requirements.txt`

Main libraries:

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn
* xgboost
* shap

 How to Run
🔧 Step 1: Install Required Libraries

Make sure Python (>=3.8) is installed. Then install dependencies using:

pip install -r requirements.txt

Or install manually:

pip install pandas numpy matplotlib seaborn scikit-learn xgboost shap
 Step 2: Download Dataset
Go to: https://www.kaggle.com/datasets/artermiloff/steam-games-dataset
Download the dataset
Extract it and place the file in your project folder
 Step 3: Run Notebooks Locally
Open Jupyter Notebook or VS Code
Navigate to the project folder
Run:
jupyter notebook
Open any RQ*.ipynb file
Click Run All
 Step 4: Run on Kaggle (Alternative)
Go to https://www.kaggle.com and log in
Open dataset page
Click New Notebook
Upload your .ipynb files
Use dataset path:
/kaggle/input/steam-games-dataset/
Click Run All
