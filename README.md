# 🎬 Netflix Data Analysis


An exploratory data analysis (EDA) of Netflix's content library uncovering trends in movies vs TV shows, top genres, country-wise production, release patterns, and more.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Key Findings](#key-findings)
- [Technologies Used](#technologies-used)
- [Setup & Installation](#setup--installation)
- [How to Run](#how-to-run)
- [Visualizations](#visualizations)
- [Future Improvements](#future-improvements)
- [License](#license)

---

## Overview

Netflix is one of the world's largest streaming platforms, with thousands of titles spanning movies and TV shows across every genre and country. This project dives into Netflix's publicly available catalog data to answer key questions:

- What is the split between Movies and TV Shows on Netflix?
- Which countries produce the most content?
- What genres dominate the platform?
- How has content volume grown over the years?
- What ratings are most common on Netflix?
- Who are the most featured directors and cast members?

---

## Dataset

- **Source:** [Kaggle — Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- **Size:** ~8,800 records
- **Format:** CSV

### Columns

| Column | Description |
|---|---|
| `show_id` | Unique ID for each title |
| `type` | Movie or TV Show |
| `title` | Name of the title |
| `director` | Director(s) of the title |
| `cast` | Main cast members |
| `country` | Country of production |
| `date_added` | Date added to Netflix |
| `release_year` | Original release year |
| `rating` | Content rating (e.g., TV-MA, PG-13) |
| `duration` | Duration in minutes or seasons |
| `listed_in` | Genres |
| `description` | Short description |

---

## Project Structure

```
Netflix-Data-Analysis/
│
├── data/
│   └── netflix_titles.csv          # Raw dataset
│   └── analysis.ipynb           # Main analysis notebook
|
│             
│
├── charts/                         # Exported visualizations
│   ├── content_type.png
│   ├── ratings.png
│   ├── top_countries.png
│   └── yearly_growth.png
│
|
└── README.md                       # Project documentation
```

---

## Key Findings

- 📽️ **Movies dominate** Netflix's catalog, making up roughly ~70% of all content vs. ~30% TV Shows.
- 🌍 **United States** is the top content-producing country, followed by **India** and the **United Kingdom**.
- 📅 **2019–2020** saw the peak in content additions; numbers have shifted post-pandemic.
- 🎭 **Dramas, Comedies, and Documentaries** are the most listed genres on the platform.
- 🔞 **TV-MA** is the most common rating, indicating a strong lean toward mature content.
- 🎬 A handful of directors appear repeatedly, with international directors featuring prominently.

---

## Technologies Used

| Tool | Purpose |
|---|---|
| Python 3.x | Core programming language |
| Pandas | Data loading, cleaning, manipulation |
| NumPy | Numerical operations |
| Matplotlib | Base visualizations |
| Jupyter Notebook | Interactive analysis environment |

---

## Setup & Installation

### 1. Clone the repository

```bash
git clone https://github.com/kunwarsaurav/Netflix-Data-Analysis.git
cd Netflix-Data-Analysis
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

**`requirements.txt`** should contain:
```
pandas
numpy
matplotlib
jupyter
```

---

## How to Run

```bash
jupyter notebook notebooks/Netflix_EDA.ipynb
```

Then run all cells from top to bottom. The notebook is structured as:
1. Setup
2. Data Cleaning (handling nulls, type conversion)
3. Core Analysis
4. Advanced Analysis
5. Visualizations & Insights
6. Summary & Conclusions

---

## Visualizations

Some of the charts generated in this project:

- **Content Type Distribution** — Pie/bar chart of Movies vs. TV Shows
- **Top 10 Countries by Content** — Horizontal bar chart
- **Genre Distribution** — Bar chart of most listed genres
- **Content Added Over the Years** — Line/bar chart showing growth trends
- **Rating Distribution** — Count plot of content ratings
- **Top Directors** — Most frequently occurring directors

> All visualizations are saved in the `/charts` folder.

---

## Future Improvements

- [ ] Add NLP-based sentiment analysis on descriptions
- [ ] Build a simple content-based recommendation system
- [ ] Create an interactive dashboard using Plotly/Dash or Tableau
- [ ] Incorporate IMDb ratings for quality analysis
- [ ] Compare Netflix trends with other platforms (Prime, Disney+)

---

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 🙋 Author

**Kunwar Saurav**  
📫 [GitHub Profile](https://github.com/kunwarsaurav)

> ⭐ If you found this project helpful, consider giving it a star!
