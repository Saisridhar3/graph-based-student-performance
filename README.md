# Graph-Based Predictive Analytics for Student Performance

A student project exploring whether graph analytics can complement machine-learning models for predicting final student grades.

## Project overview

This project uses the Student Performance Mathematics dataset (`student-mat.csv`) to:
- explore student academic and demographic attributes;
- represent students as nodes in a similarity network;
- analyze graph structure using NetworkX;
- calculate centrality measures and PageRank;
- identify communities in the network;
- compare traditional regression models with graph-enhanced models for predicting the final grade (`G3`).

## Tools and technologies

- Python
- Google Colab / Jupyter Notebook
- pandas and NumPy
- Matplotlib and Seaborn
- NetworkX
- scikit-learn
- Plotly (for interactive network visualizations, if used)

## Repository structure

```text
.
├── notebooks/
│   └── Graph-Based-Predictive-Analytics.ipynb
├── data/
│   └── README.md
├── results/
│   └── README.md
├── figures/
│   └── README.md
├── presentation/
│   └── project-presentation.pptx
├── docs/
│   └── README.md
├── .gitignore
├── requirements.txt
└── README.md
```

## Dataset

The project uses the Student Performance dataset, Mathematics subset (`student-mat.csv`).

Dataset source: UCI Machine Learning Repository, *Student Performance* dataset. Add the exact dataset URL used in your project here.

The notebook previously loaded 395 records and 33 original columns. The target variable is `G3`, the final-period grade, on a 0–20 scale.

**Dataset note:** Check the dataset's license and source terms before redistributing the CSV. If unsure, do not commit the dataset; instead, provide download instructions in `data/README.md`.

## How to run

### Option 1: Google Colab
1. Open the notebook in `notebooks/`.
2. Upload `student-mat.csv` to the Colab session or mount Google Drive.
3. Run cells from top to bottom.
4. Review the generated metrics and visualizations.

### Option 2: Local Python environment
1. Install Python 3.10 or later.
2. Create and activate a virtual environment.
3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Put `student-mat.csv` in the `data/` folder and update the notebook's data path if needed.
5. Open the notebook with Jupyter or VS Code and run it from top to bottom.

## Evaluation

The notebook compares regression models using:
- **RMSE** — lower is better;
- **MAE** — lower is better;
- **R²** — higher is generally better.

Only report the metrics produced by the final, successfully executed notebook. Do not claim that graph features improve prediction unless the measured results support that conclusion.

## Methodology

1. Load and inspect the dataset.
2. Perform exploratory data analysis.
3. Select student attributes and prepare features.
4. Calculate student similarity and construct a graph.
5. Analyze graph properties, shortest paths, centrality, PageRank, and communities.
6. Add graph-derived features to the predictive dataset.
7. Compare traditional and graph-enhanced regression models.
8. Save evaluation tables and visualizations.

## Limitations

- The dataset contains 395 students from one dataset, so findings may not generalize to other populations.
- Earlier-period grades (`G1` and `G2`) are strong predictors of the final grade (`G3`).
- If the graph is built before the train/test split, the experiment is transductive: test-student features may contribute to graph structure. This should be disclosed, and future work should evaluate a leakage-safe graph construction procedure.
- Network centrality indicates structural position in this constructed graph; it does not measure a student's personal worth, ability, or influence in real life.

## Project team

- **Author:** SAI SRIDHAR ALASAKANI
- **Team members:** Add names and student IDs here
- **Department / Institution:** Add details here
- **Faculty guide:** Add name here

## License

Choose an appropriate license for your own code and documentation after checking your institution's requirements and the dataset's terms. Do not imply that third-party data is yours.
