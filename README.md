# 🎬 Movie Data Analysis

An end-to-end movie dataset preprocessing and exploratory data analysis project built using **Python, Pandas, Matplotlib, and Seaborn**.

This project focuses on transforming raw movie data into a structured and analysis-ready format while extracting meaningful insights about movie genres, popularity, ratings, and release trends.

---

# 📌 Project Overview

Real-world datasets are messy.

This project demonstrates how raw movie data can be:

* cleaned,
* transformed,
* categorized,
* visualized,
* and analyzed to uncover patterns and trends.

The dataset contains information about thousands of movies including:

* release dates,
* popularity scores,
* vote averages,
* genres,
* titles,
* and vote counts.

---

# 🚀 Features

✅ Data Cleaning
✅ Missing Value Handling
✅ Datatype Conversion
✅ Feature Engineering
✅ Genre-wise Analysis
✅ Popularity Categorization
✅ Exploratory Data Analysis (EDA)
✅ Data Visualization

---

# 🛠️ Tech Stack

| Tool             | Purpose                   |
| ---------------- | ------------------------- |
| Python           | Core Programming          |
| Pandas           | Data Processing           |
| NumPy            | Numerical Operations      |
| Matplotlib       | Data Visualization        |
| Seaborn          | Statistical Visualization |
| Jupyter Notebook | Interactive Analysis      |

---

# 📂 Dataset Columns

| Column       | Description          |
| ------------ | -------------------- |
| Release_Date | Movie release date   |
| Title        | Movie title          |
| Popularity   | Popularity score     |
| Vote_Count   | Total votes          |
| Vote_Average | Average movie rating |
| Genre        | Movie genres         |

---

# ⚙️ Data Preprocessing Steps

## 🔹 Initial Dataset Inspection

Performed:

* `head()`
* `info()`
* `describe()`
* shape analysis

Goal:

* understand structure,
* identify null values,
* inspect datatypes.

---

## 🔹 Removing Unnecessary Columns

Dropped:

* `Overview`
* `Poster_Url`
* `Original_Language`

Reason:
These columns were not required for the current analysis workflow.

---

## 🔹 Handling Missing Values

Used:

```python
df.isnull().sum()
df.dropna(inplace=True)
```

This ensured:

* cleaner analysis,
* fewer visualization errors,
* better dataset consistency.

---

## 🔹 Vote Average Categorization

Converted numerical ratings into categories:

| Category      |
| ------------- |
| not_popular   |
| below_average |
| average       |
| popular       |

This made movie ratings more interpretable during analysis.

---

## 🔹 Release Date Transformation

Converted:

```python
object → datetime → release year
```

This helped in:

* year-wise analysis,
* trend visualization,
* release distribution studies.

---

## 🔹 Genre Explosion

Movies contained multiple genres in one row.

Example:

```python
Action, Adventure, Science Fiction
```

Used:

```python
str.split()
explode()
```

This transformed genres into individual rows for accurate genre analysis.

---

# 📊 Exploratory Data Analysis

## 🎭 Genre Distribution

Discovered that:

* Drama dominates the dataset
* Comedy and Action are highly frequent
* Thriller and Adventure are also common

---

## ⭐ Vote Category Analysis

Movies were analyzed based on popularity categories:

* popular
* average
* below_average
* not_popular

The dataset showed a relatively balanced distribution among categories.

---

## 📅 Release Trend Analysis

Release years were visualized to understand:

* movie production trends,
* dataset concentration,
* release frequency over time.

---

# 📈 Key Insights

🔹 Drama is the most dominant genre in the dataset
🔹 Genre explosion significantly improved genre-level analysis
🔹 Categorizing ratings simplified interpretation
🔹 Data preprocessing directly improved visualization quality
🔹 Proper datatype conversion made temporal analysis easier

---

# 🧠 What I Learned

Through this project, I gained hands-on experience with:

* real-world dataset preprocessing,
* data cleaning workflows,
* Pandas operations,
* categorical transformations,
* feature engineering,
* exploratory data analysis,
* and visualization techniques.

This project also improved my understanding of how preprocessing affects the quality of insights generated from data.

---

# 📸 Sample Visualizations

* Genre Distribution Plot
* Vote Category Countplot
* Release Year Distribution
* Popularity Analysis

---

# ▶️ Run Locally

Clone the repository:

```bash
git clone https://github.com/arpit-purohit01/Movie-Data-Analysis.git
```

Move into the project folder:

```bash
cd Movie-Data-Analysis
```

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn notebook
```

Run Jupyter Notebook:

```bash
jupyter notebook
```

---

# 📁 Project Structure

```bash
Movie-Data-Analysis/
│
├── Movie/
│   └── Data Processing/
│       └── movies.ipynb
│
├── dataset/
│
└── README.md
```

---

# 🌟 Future Improvements

* Add interactive dashboards
* Build recommendation system
* Perform sentiment analysis on movie overviews
* Add machine learning models
* Deploy visualizations using Streamlit

---

# 👨‍💻 Author

## Arpit Purohit

Passionate about:

* Data Science
* AI/ML
* Web Development
* Building impactful tech projects

LinkedIn: https://linkedin.com/in/arpit-purohit06

---

# ⭐ If you liked this project

Give this repository a star and feel free to contribute.
