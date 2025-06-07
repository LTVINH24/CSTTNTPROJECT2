# Project 2: Decision Tree

This repository contains code and experiments for building and evaluating decision tree classifiers on multiple real-world datasets using **scikit-learn**.

## Datasets Used

1. **UCI Heart Disease Dataset** – Binary classification.  
2. **Palmer Penguins Dataset** – Multi-class classification.  
3. **Custom Dataset** – Additional dataset (with at least 300 samples and 2+ classes).  

Each dataset is analyzed separately using the same pipeline described in the project instructions.

---

## Requirements

Make sure you have **Python 3.10+** installed.

It is recommended to use a **virtual environment** to isolate project dependencies.

### Step 1: Create and activate virtual environment

```bash
python -m venv venv
venv\Scripts\activate      # On Linux/macOS: source venv/bin/activate
```

### Step 2: Install required packages

```bash
pip install -r requirements.txt
```

> [!Note]
> If you encounter issues with Graphviz:
>   - **Windows:** 
>       Install Graphviz from https://graphviz.org/download/ and add it to your PATH.
>   - **Ubuntu/Debian:**  
>       ```bash
>       sudo apt-get install graphviz
>       ```

---

## How to Run

The project is implemented in **Jupyter Notebook (.ipynb)** format.

To run the notebooks:

1. Launch Jupyter:  
    ```bash
    jupyter notebook
    ```

2. Open one of the notebooks:
   - `HeartDisease_DecisionTree.ipynb`
   - `Penguins_DecisionTree.ipynb`
   - `CustomDataset_DecisionTree.ipynb`

3. Select the **train/test ratio** and execute the notebook cell-by-cell.

---

## Tasks Covered

Each notebook includes the following sections:

1. **Data Preparation**
   - Load dataset  
   - Shuffle and stratified split into 4 ratios: 40/60, 60/40, 80/20, and 90/10  
   - Create 16 subsets: `(feature_train, label_train, feature_test, label_test)`

2. **Decision Tree Training**
   - Use `sklearn.tree.DecisionTreeClassifier` with `criterion='entropy'` (information gain)  
   - Visualize trees with Graphviz

3. **Performance Evaluation**
   - Predict test set  
   - Show `classification_report` and `confusion_matrix`  
   - Provide interpretation of the metrics

4. **Tree Depth vs Accuracy (80/20 split)**
   - Evaluate different `max_depth` values: `None, 2, 3, 4, 5, 6, 7`  
   - Compare accuracies and visualize trees  
   - Plot depth vs accuracy

5. **Repeat on All Datasets**
   - Same process repeated for 3 datasets  
   - Comparative analysis written in report

---

## Project Requirements

This project follows all instructions as outlined in the **CS14003 Artificial Intelligence Project 2**:

- Use of **scikit-learn** and **decision trees**
- Support for **multiple train/test splits**
- Visualizations using **Graphviz**, **matplotlib**
- Comparative analysis across datasets
- Final submission includes:
  - Jupyter notebooks (`.ipynb`)
  - Project report (PDF)
  - README and requirements.txt

---

## Group Information

- [Student Name 1] – [Student ID]  
- [Student Name 2] – [Student ID]  
- [Student Name 3] – [Student ID]
- [Student Name 4] – [Student ID]
- Trương Lê Anh Vũ – 22120443

Each member's contribution and self-evaluation is detailed in the report.
