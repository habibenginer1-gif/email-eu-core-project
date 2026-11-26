# Email-Eu-core Network Analysis

## Research Question

How do email communication patterns in a European research institution 
reflect its departmental structure and which individuals act as connectors 
between different departments?


## Team Members

- [Habib Ullah] — @[habibenginer1-gif]
- [Colin Boisron ] — @[ranyac]
- [Abdulai Bah] — @[bahabdulai1993]

---

## Dataset & Source

- **Name:** Email-Eu-core — [SNAP, Stanford](https://snap.stanford.edu/data/email-Eu-core.html)
- **Files:** `email-Eu-core.txt.gz` (edges), `email-Eu-core-department-labels.txt.gz` (labels)
- **Raw:** 25,571 edge rows, 1,005 label rows, 642 self-loops, 0 duplicates, 0 missing values
- **Clean network:** 1,005 nodes, 24,929 directed unweighted edges, 42 departments, density 0.0247
- **Nodes:** Employees of a European research institution
- **Edges:** Directed (sender → receiver); binary (email exists or not, no weights/timestamps)


## Instruction for Reproducing Results

### Prerequisites
- Python 3.9+
- pip

### Files needed
- `Project.ipynb` — main analysis notebook
- `email-Eu-core.txt.gz` — edge list (download from [SNAP](https://snap.stanford.edu/data/email-Eu-core.html))
- `email-Eu-core-department-labels.txt.gz` — department labels (same link)
- `requirements.txt` — dependencies

### Step 1: Clone and install

```bash
git clone https://github.com/your-username/email-eu-core-project.git
cd email-eu-core-project
pip install -r requirements.txt
```

### Step 2: Get the data

The dataset is not redistributed in this repo (size + license). Download both files from 
[SNAP](https://snap.stanford.edu/data/email-Eu-core.html) and place them in the 
**same folder as `Project.ipynb`**:

```
email-eu-core-project/
├── Project.ipynb
├── email-Eu-core.txt.gz
├── email-Eu-core-department-labels.txt.gz
└── requirements.txt
```

Alternatively, use curl:

```bash
curl -O https://snap.stanford.edu/data/email-Eu-core.txt.gz
curl -O https://snap.stanford.edu/data/email-Eu-core-department-labels.txt.gz
```

### Step 3: Run the notebook

```bash
jupyter notebook Project.ipynb
```

Then **Run All** (Cell → Run All). The notebook executes sequentially:






