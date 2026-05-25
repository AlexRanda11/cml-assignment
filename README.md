# Classical Machine Learning [CML]: Assignment

Assignment for the **Classical Machine Learning (CML)** module held at the **MSc Software Engineering Programme** in **Oxford University**.

## Overview

This assignment compares six machine learning clustering algorithms across four datasets, analyzing their performance through multiple evaluation metrics and visual inspection. The analysis includes:

- **Algorithms Tested**: DBSCAN, HDBSCAN, OPTICS, Spectral Clustering, Birch, and Gaussian Mixture Models
- **Evaluation Metrics**: Silhouette Score and Davies-Bouldin Index
- **Datasets**: Four synthetic datasets with varying cluster structures and dimensionality
- **Comprehensive Analysis**: Theoretical explanations, performance comparisons, and algorithm selection rationale

## File Structure

```
cml-assignment/
├── cml-assignment.ipynb          # Main Jupyter Notebook (analysis & results)
├── README.md                      # This file
├── pyproject.toml                 # Project configuration
├── main.py                        # Utility script for character counting
├── CML_2026-04-27#3-dataset1.csv  # Dataset 1 (2D - ring structure)
├── CML_2026-04-27#4-dataset2.csv  # Dataset 2 (3D - Gaussian clusters)
├── CML_2026-04-27#5-dataset3.csv  # Dataset 3 (2D - multiple clusters)
├── CML_2026-04-27#6-dataset4.csv  # Dataset 4 (2D - additional analysis)
└── images/                        # Generated visualizations directory
```

## Setup & Requirements

### Prerequisites
- Python 3.11+
- pip or conda package manager

### Installation

1. **Clone or navigate to the project directory:**
   ```bash
   cd cml-assignment
   ```

2. **Create a virtual environment (optional but recommended):**
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. **Install required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   
   Or manually install:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn plotly missingno jupyter
   ```

## Running the Notebook

### Option 1: VS Code (Recommended)
1. Open the project folder in VS Code
2. Install the Jupyter extension (if not already installed)
3. Click the "Run All" button in the notebook, or run individual cells with Ctrl+Enter

### Option 2: Jupyter Lab
```bash
jupyter lab cml-assignment.ipynb
```

### Option 3: Jupyter Notebook
```bash
jupyter notebook cml-assignment.ipynb
```

## Exporting to PDF

To export the notebook as PDF:

1. **Install Pandoc** (if not already installed):
   ```bash
   brew install pandoc  # macOS
   # or
   sudo apt-get install pandoc  # Linux
   ```

2. **In VS Code**: Right-click the notebook tab → **Export as** → **PDF**

3. **Or via command line**:
   ```bash
   jupyter nbconvert --to pdf cml-assignment.ipynb
   ```

## Key Components

### Imported Libraries
- **Data Manipulation**: pandas, numpy
- **Clustering**: scikit-learn (DBSCAN, HDBSCAN, OPTICS, SpectralClustering, Birch, GaussianMixture)
- **Evaluation**: scikit-learn metrics (Silhouette Score, Davies-Bouldin Index)
- **Visualization**: matplotlib, seaborn, plotly, missingno

### Notebook Structure

1. **Imports & Setup** - All required libraries with source documentation
2. **Dataset 1 Analysis** - Ring structure clustering comparison
3. **Dataset 2 Analysis** - 3D Gaussian cluster analysis
4. **Dataset 3 Analysis** - Multi-cluster structure analysis
5. **Dataset 4 Analysis** - Additional dataset evaluation
6. **Appendix** - References in IEEE format

## Character Count

To verify the assignment is within the character limit (< 75,000):

```bash
python main.py
```

This will display character counts by cell type and total assignment size.

## Assignment Constraints

- **Character Limit**: < 75,000 characters
- **Submission Format**: Jupyter Notebook (.ipynb)
- **Datasets Provided**: 4 synthetic CSV files
- **Output**: PDF export for formal submission

## Notes

- All datasets are automatically standardized using Z-score normalization
- Clustering results include both quantitative metrics and visual validation
- Algorithm selection considers both performance scores and cluster quality
- References are formatted in IEEE citation style

## Jupyter Notebook

The main deliverable is the **Jupyter Notebook**: [cml-assignment.ipynb](./cml-assignment.ipynb)