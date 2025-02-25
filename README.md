# 🗳️ Maharashtra Election Analysis (2019 vs 2024)

## 📌 Overview
This repository contains an in-depth analysis and visualization of the **Maharashtra Legislative Assembly Elections** for the years **2019** and **2024**. The primary goal is to compare party performances, seat distributions, and alliances over two election cycles and present these findings in both tabular and map-based visualizations.

## 🎯 Objectives
1. **Data Collection & Cleaning**  
   - Scrape and aggregate data from various public sources (e.g., news websites, Election Commission of India).  
   - Clean and format the data for consistent usage within the analysis notebook.
2. **Comparative Analysis**  
   - Compare how parties and alliances performed in **2019 vs 2024**.  
   - Identify which parties gained or lost seats and in which constituencies.
3. **Geospatial Visualization**  
   - Use **GeoPandas** to map the election results across Maharashtra constituencies.  
   - Highlight patterns or trends at the constituency level.
4. **Insight Generation**  
   - Draw conclusions about voter shifts, emerging alliances, and seat distribution changes.  
   - Provide visual representations to make data interpretation straightforward.

---

## 📂 Project Structure

Maharashtra_Election_Analysis/ ├── Data/ │ ├── election_maharastra2019.xls │ ├── election_maharastra2024.xls │ ├── maharashtra_AC.json # GeoJSON for constituency boundaries │ ├── Notebooks/ │ └── maharastra_election.ipynb # Main analysis notebook │ ├── requirements.txt # Required Python libraries ├── README.md # Project documentation ├── LICENSE # License file


- **Data/**: Contains raw data files (`.xls`) and the **GeoJSON** file for mapping.  
- **Notebooks/**: Holds the main Jupyter Notebook (`.ipynb`) that walks through data cleaning, analysis, and visualization.  
- **requirements.txt**: Lists all necessary libraries to replicate the environment.  
- **README.md**: The file you’re currently reading, describing the project and its usage.  
- **LICENSE**: Project license information (e.g., MIT).

---

## 📊 Data Description
- **Election Data**  
  - **2019 Data**: Contains constituency-level results (candidate names, party affiliation, votes, etc.).  
  - **2024 Data**: Similar structure as 2019 data, allowing direct comparison.  
- **GeoJSON (maharashtra_AC.json)**  
  - Used for mapping constituencies in **GeoPandas**.  
  - Each feature corresponds to a constituency boundary within Maharashtra.

**Note**: The data is cleaned **within** the Jupyter Notebook (`maharastra_election.ipynb`). If you need to replicate the cleaning process, simply run the notebook cells in order.

---

## ⚙️ Installation & Setup

1. **Clone this Repository**  
   ```bash
   git clone https://github.com/jerry2002yy/Maharashtra_Election_Analysis.git
   cd Maharashtra_Election_Analysis

2. **Install Dependencies**  
   Make sure you have Python 3.x installed. Then run:
   pip install -r requirements.txt

3. **Open the Notebook**
   jupyter notebook Notebooks/maharastra_election.ipynb
   This will launch Jupyter in your browser. Execute cells in sequence to see the data cleaning, analysis, and visualizations.

## 🔎 Analysis Steps

### 📥 Data Import & Preview
- Load 2019 and 2024 `.xls` files using `pandas.read_excel()`.
- Display initial rows to understand the data format.

### 🛠 Data Cleaning
- Handle missing values, data type inconsistencies, and rename columns for clarity.
- Filter out any incomplete or irrelevant entries.

### 📊 Comparative Analysis
- Merge or concatenate the data to facilitate side-by-side comparison.
- Calculate key metrics like:
  - Vote share
  - Seat share
  - Margin of victory

### 🗺 Geospatial Mapping
- Load GeoJSON into a GeoDataFrame.
- Merge election results with the GeoDataFrame using a matching constituency key.
- Plot maps visualizing:
  - Winning parties
  - Vote margins
  - Alliance distribution

### 📈 Visualization & Insights
- Use `Matplotlib` or `Seaborn` for:
  - Bar plots
  - Line charts
  - Pie charts
- Extract key insights:
  - Which parties gained or lost seats?
  - How alliances formed or changed?
  - Regional voting patterns and swings.


## 🤝 Contributing

### 🔥 How to Contribute
- Fork the repository and create a new branch.
- Make your changes and ensure they align with the project goals.
- Commit your changes with clear and descriptive messages.
- Push the changes to your forked repository.
- Open a **Pull Request** for review.

### 📜 Contribution Guidelines
- Ensure code follows best practices and is well-documented.
- Keep visualizations clear and meaningful.
- Any new data added should be properly cited and formatted.
- Follow PEP8 standards for Python code.
- Be respectful and constructive in discussions.

### 🛠 Areas to Contribute
- **Data Enhancement**: Improve data cleaning, add new datasets, or update existing data.
- **Visualization**: Create better graphs, maps, or charts to enhance insights.
- **Code Optimization**: Improve efficiency and readability of the analysis.
- **Feature Additions**: Implement new functionalities, such as interactive visualizations.
- **Bug Fixes**: Identify and resolve issues in data processing or visualization.

### 📩 Need Help?
If you need any help or have suggestions, feel free to open an issue or contact the project maintainer.
