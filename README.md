## Yoni's Dashboard

Yoni's Dashboard is a simple interactive dashboard built with `Streamlit` and `pandas`.  
It demonstrates how to create a small HR-style analytics view over a mock employee dataset, including:

- **General data table** with employee details
- **Department distribution bar chart**
- **Average age metric** displayed as a highlight card

All labels and content in the app are in Hebrew, while the code and this README are in English so it is easy to follow and share on GitHub.

---

### Features

- **Interactive table**: View a small dataset of employees, including name, age, department, and score.
- **Department analysis**: A bar chart showing how many employees are in each department.
- **Summary metric**: A single-number KPI displaying the average employee age.
- **Randomized scores**: Each run generates new random scores, making the dashboard feel dynamic.


---

### Project Structure

- `dashboard.py` – Main Streamlit app defining the dashboard UI and logic.

---

### Requirements

This project was tested with:

- **Python** 3.9+ (any recent 3.x version should be fine)
- **Packages**:
  - `streamlit`
  - `pandas`
  - `numpy`

You can install the dependencies with:

```bash
pip install streamlit pandas numpy
```

If you prefer to keep things isolated, use a virtual environment (`venv` or `conda`) before installing packages.

---

### How to Run the Dashboard

From the project root (the folder that contains `dashboard.py`), run:

```bash
streamlit run dashboard.py
```

Then open the URL that Streamlit prints in the terminal (typically `http://localhost:8501`) in your browser.

---

### Usage Notes

- All text in the UI is in Hebrew, so the app is suitable for Hebrew-speaking users and demos.
- Since scores are generated randomly with `numpy`, refreshing / re-running the app may slightly change the score column.

---

### Contributing

If you want to extend this dashboard, some ideas:

- **Add filters** (e.g., by department or age range) using Streamlit widgets.
- **Add more charts** such as histograms of ages or scores.
- **Load real data** from a CSV or database instead of using mock data.

Feel free to fork the repository and open pull requests with improvements.

