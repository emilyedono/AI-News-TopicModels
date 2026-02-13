# AI-News-TopicModels

**Project:** Media Bias & AI — news coverage of artificial intelligence across outlet types (Business, Tech, General, Political).

**Purpose:** Repository for a class project (collaborative) exploring sentiment and topical coverage of AI in news headlines. This version is prepared for a data science portfolio and highlights my primary contributions in topic modeling.

**Contents:**
- **Data:** `Data/newsapi_keyword_articles.csv` — NewsAPI keyword pulls used for analysis.
- **Notebooks:**
	- `Notebooks/Collaborative Contributions/8414_Final_Project_Codebook_prod.ipynb` — Full project notebook (group work).
	- `Notebooks/Section_7_Topic_Modeling.ipynb` — Standalone, runnable notebook with the Topic Modeling section I developed (recommended for portfolio review).
- **Environment:** `requirements.txt` is included for reproducibility.

**My Role (highlight):**
- **Topic modeling:** I led the BERTopic-based topic modeling (Section 7). I
	- implemented BERTopic workflows to discover themes across all outlets,
	- created a balanced dataset subset and keyphrase extraction using KeyBERT,
	- produced visualizations (topic tables, word clouds, and bar charts) for portfolio presentation.

**Quick Start**
- Clone the repo and change directory:

	```bash
	git clone <repo-url>
	cd AI-News-TopicModels
	```

- Create and activate the virtual environment (macOS / zsh):

	```bash
	python3 -m venv .venv
	source .venv/bin/activate
	```

- Install dependencies and enable the Jupyter kernel (already included in this repo):

	```bash
	pip install -r requirements.txt
	# optional: install kernel with a friendly name
	python -m ipykernel install --user --name ai-news-venv --display-name "AI-News-TopicModels (.venv)"
	```

- Run the standalone topic modeling notebook (recommended):

	```bash
	jupyter lab  # or `jupyter notebook`
	# then open `Notebooks/Section_7_Topic_Modeling.ipynb`
	```

**Notes & Assumptions**
- The notebooks expect the datasets at `Data/newsapi_keyword_articles.csv` (already present). If you regenerate the dataset via NewsAPI, ensure the same column names (`title`, `description`, `source`, `publishedAt`, etc.).


**Attribution & License**
- This work was originally a group project for an academic course. The topic modeling section (Section 7) is my primary contribution and is safe to showcase in a portfolio.
- License: see `LICENSE` in repo root.
