# Netflix Data Analytics + AI Project

**Student:** Arpitakhan  
**Program:** IBM SkillsBuild Data Analytics with AI – Academic Internship  
**Project Type:** Exploratory Data Analysis + AI-based Recommendation System

## 1. Project Description

This project performs an end-to-end analysis of the `netflix_titles.csv` dataset using Python.

The project includes:

- Data loading and validation
- Data cleaning
- Missing-value analysis
- Movie vs TV Show comparison
- Release-year and Netflix-added-year analysis
- Country analysis
- Genre/category analysis
- Rating analysis
- Movie duration analysis
- TV-show season analysis
- Data visualizations
- A content-based AI recommendation system using TF-IDF and cosine similarity

## 2. Dataset

The project uses the well-known **Netflix Movies and TV Shows** dataset.

Dataset link:

https://www.kaggle.com/datasets/shivamb/netflix-shows

The standard version contains 8,807 records and 12 columns. Dataset versions can differ, so the notebook calculates the actual figures from the local CSV rather than hard-coding them.

### Main columns

- `show_id`
- `type`
- `title`
- `director`
- `cast`
- `country`
- `date_added`
- `release_year`
- `rating`
- `duration`
- `listed_in`
- `description`

## 3. Project Structure

```text
Netflix Project/
│
├── netflix_titles.csv
├── ArpitakhanNetflix Data Analytics Project.ipynb
├── requirements.txt
├── README.md
└── ArpitakhanProjectReport.docx
```

## 4. Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## 5. How to Run

### Step 1 – Install Python

Install Python 3.10+ if it is not already installed.

### Step 2 – Put the dataset in the project folder

Place:

```text
netflix_titles.csv
```

in the same folder as the Jupyter Notebook.

### Step 3 – Install dependencies

Open Command Prompt / Terminal in the project folder and run:

```bash
pip install -r requirements.txt
```

### Step 4 – Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
ArpitakhanNetflix Data Analytics Project.ipynb
```

### Step 5 – Run the notebook

Run the cells from top to bottom.

## 6. AI Component

The project contains a **content-based recommendation system**.

It combines:

- `listed_in` (genres/categories)
- `description`

The text is converted into numerical vectors using **TF-IDF**. Then **cosine similarity** is used to find titles with similar content.

This approach does not require a paid API or external AI service.

## 7. Example AI Workflow

```text
Netflix title
     ↓
Genre + Description
     ↓
Text preprocessing
     ↓
TF-IDF vectorization
     ↓
Cosine similarity
     ↓
Similar Netflix titles
```

## 8. Important Data-Quality Notes

- Director, cast, and country contain missing values.
- `country` and `listed_in` can contain multiple comma-separated values.
- `duration` stores movie minutes and TV-show seasons in the same column, so they must be separated before numeric analysis.
- The dataset is a historical snapshot and should not be treated as today's Netflix catalog.

## 9. Expected Learning Outcomes

After completing this project, the learner demonstrates:

1. Basic data loading with Pandas.
2. Data cleaning and missing-value handling.
3. Exploratory data analysis.
4. Data visualization.
5. Feature engineering.
6. Basic machine-learning text representation.
7. Similarity-based recommendation.
8. Interpretation of analytical results.
9. Reproducible project documentation.

## 10. Submission Files

This submission contains the four requested files:

1. `ArpitakhanNetflix Data Analytics Project.ipynb`
2. `requirements.txt`
3. `README.md`
4. `ArpitakhanProjectReport.docx`

## 11. References

- Kaggle Netflix Movies and TV Shows dataset:
  https://www.kaggle.com/datasets/shivamb/netflix-shows
- Pandas: https://pandas.pydata.org/docs/
- Scikit-learn: https://scikit-learn.org/stable/
- Matplotlib: https://matplotlib.org/stable/

## 12. Academic Note

This project is intended as a beginner-friendly academic data analytics project. It demonstrates reproducible analysis and a simple AI/ML application without claiming that the algorithm is Netflix's production recommendation system.
