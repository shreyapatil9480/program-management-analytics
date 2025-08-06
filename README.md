# Program Management Analytics Project

This repository contains a synthetic dataset and an analysis notebook designed to showcase the skills of a **Business Analyst**, **Program Manager** or **Data Analyst**. The project walks through data exploration, visualization and predictive modeling using a fictitious program management dataset.

## Overview

Organizations often track metrics such as budgets, schedules, team size and stakeholder satisfaction to gauge the health of projects. This project simulates those metrics across 200 projects and demonstrates how to:

1. **Import and explore the data** – load a CSV file into a pandas DataFrame, inspect data types and basic statistics.
2. **Perform exploratory data analysis (EDA)** – create distribution plots, summary statistics and a correlation heatmap to discover patterns in budget and schedule performance.
3. **Build a predictive model** – train a logistic regression model to predict whether a project is successful based on budget adherence, schedule adherence, team size and stakeholder satisfaction.

The resulting notebook is fully annotated and ready to run out of the box. It can serve as a showcase of your analytic skills when applying for Business Analyst, Program Manager or Data Analyst roles.

## Synthetic Dataset

The dataset (`synthetic_program_management_dataset.csv`) contains 200 simulated program management records with the following fields:

| Column | Description |
|-------|------------|
| `project_id` | Unique identifier for each project |
| `start_date` | Date when the project started |
| `planned_duration_days` | Planned duration in days |
| `actual_duration_days` | Actual duration in days (a variation of the planned duration) |
| `end_date_planned` | Planned end date based on the start date and planned duration |
| `budget` | Planned budget (randomly generated between \$50k and \$500k) |
| `actual_spend` | Actual spend (varying around the budget) |
| `num_team_members` | Number of team members assigned |
| `stakeholder_satisfaction` | Stakeholder satisfaction score (1–5) |
| `project_success` | Binary flag indicating whether the project is considered successful (1) or not (0). A project is successful if it stays within 10% of budget and schedule and has satisfaction ≥ 3. |

Since the data is synthetic, it poses no privacy concerns and can be freely shared.

## Files in This Repository

- `synthetic_program_management_dataset.csv` – the synthetic dataset described above.
- `program_management_analysis.ipynb` – Jupyter notebook containing the analysis. It loads the dataset, performs EDA, visualizes distributions and correlations, and trains a logistic regression model to predict `project_success`.
- `requirements.txt` – list of Python dependencies required to run the notebook.

## Getting Started

To run the analysis on your local machine:

1. **Clone the repository** (replace the URL once you publish it to your GitHub account):
   ```bash
   git clone https://github.com/<your-username>/program-management-analytics.git
   cd program-management-analytics
   ```
2. **Create and activate a virtual environment** (optional but recommended):
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
4. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook program_management_analysis.ipynb
   ```

The notebook will open in your browser. Follow the comments and outputs to understand the data and modeling process.

## Project Structure and Difficulty

This project is structured to incrementally demonstrate your skills:

1. **Data Generation**: Creating a realistic synthetic dataset requires understanding of project management metrics and how they interact.
2. **Exploratory Analysis**: Visualizing distributions and correlations helps to identify patterns and potential drivers of success.
3. **Predictive Modeling**: Building and evaluating a logistic regression model shows how to translate insights into actionable predictions.

Feel free to extend the notebook with additional visualizations (e.g., box plots, scatter plots), alternative models (e.g., decision trees or random forests), or feature engineering steps. Each extension can showcase a deeper level of proficiency.

## Usage and Adaptation

This repository can be used as-is to demonstrate your analytic workflow. If you wish to adapt it for a particular domain or interview case study, consider adjusting:

- The features included in the dataset (e.g., add risk scores, resource utilization, or geographic regions).
- The target metric (e.g., predicting budget overruns rather than overall success).
- The modeling approach (e.g., experimenting with classification algorithms or regression to predict continuous outcomes).

Contributions and improvements are welcome. This project is licensed under the MIT License.

## License

This project is released under the [MIT License](LICENSE). You are free to use, modify and distribute it with attribution.
