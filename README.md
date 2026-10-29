# Graph-Based Predictive Analytics for Student Performance

## Project Overview
This project combines graph analytics and machine learning to analyze student relationships and predict academic performance. It uses student academic and demographic data to construct a similarity network, analyze network properties, and evaluate predictive models.

## Objectives
- Build a student similarity graph using NetworkX.
- Analyze network structure using degree, closeness, betweenness, and eigenvector centrality.
- Apply PageRank and community detection to identify important nodes and groups.
- Use graph-derived features alongside student attributes for predictive modeling.
- Compare traditional machine learning models with graph-enhanced models.

## Technologies Used
- Python
- Google Colab / Jupyter Notebook
- Pandas and NumPy
- NetworkX
- Matplotlib
- Scikit-learn

## Dataset
The project uses the Student Performance dataset, which contains student demographic, social, and academic attributes. The final grade (`G3`) is the prediction target.

## Methodology
1. Data loading and preprocessing
2. Exploratory data analysis
3. Student similarity graph construction
4. Centrality and community analysis
5. Graph feature extraction
6. Machine learning model training and evaluation
7. Results visualization and comparison

## Repository Structure
- `notebooks/` — analysis and modeling notebook
- `data/` — dataset resources
- `figures/` — generated graph and model visualizations
- `results/` — exported analysis and model comparison files
- `presentation/` — project presentation
- `docs/` — additional documentation

## How to Run
1. Open the notebook in Google Colab.
2. Upload or load the dataset according to the notebook instructions.
3. Install any missing dependencies listed in `requirements.txt`.
4. Run the notebook cells in order.

## Important Notes
Model performance metrics should be taken from the final exported results. Graph-enhanced models do not necessarily outperform traditional models. Results depend on the dataset, graph construction method, and validation strategy.

## Author
Sai Sridhar Alasakani
