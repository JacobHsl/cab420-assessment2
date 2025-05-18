# Sender Email Classification (CAB420 Project)

This project uses the [Enron Email Dataset](https://www.cs.cmu.edu/~enron/) to classify emails by sender based on message content. It supports multiple ML models, including traditional and deep learning approaches.

## Setup Instructions

### 1. Clone the Repository
```bash
git clone <your-repo-url>
cd <your-repo-directory>
```

### 2. Create a Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
source venv/bin/activate
```

### 3. Install Required Python Packages
```bash
pip install -r requirements.txt
```

If you have an `Nvidia GPU`, run

```bash
pip install tensorflow[and-cuda]
```
Otherwise, run
```bash
pip install tensorflow
```
---

## Download the Enron Dataset

Run the following `curl` command to download the dataset archive:

```bash
curl -O https://www.cs.cmu.edu/~enron/enron_mail_20150507.tar.gz
```

Place this file in the project root directory — the data extraction code will handle the rest.

---

## Launch Jupyter Lab

If not already installed, run:

```bash
pip install jupyterlab
```

Then launch:

```bash
jupyter lab
```

Open the notebook provided (e.g., `preprocessing.ipynb`) to begin processing the dataset and training models.

---

## Notes

- The dataset is large (~423MB compressed, ~2.3GB extracted).
- Ensure you have sufficient disk space and memory (~8–16GB recommended).
- The preprocessing pipeline filters spam, trims metadata, and prepares the dataset for classification.
