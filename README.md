# Sender Email Classification (CAB420 Project)

This project uses the [Enron Email Dataset](https://www.cs.cmu.edu/~enron/) to classify emails by sender based on message content. It supports multiple ML models, including traditional and deep learning approaches.

## Setup Instructions

### 1. Clone the Repository
```bash
git clone git@github.com:JacobHsl/cab420-assessment2.git
cd cab420-assessment2/
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

MAke sure this file is in the project root directory, the code will extract this file.

---

## Launch Jupyter Lab

Jupyter lab should be installed via the requirements, if not run:

```bash
pip install jupyterlab
```

Then launch:

```bash
jupyter lab
```

---

## Notes

- The dataset is large (~423MB compressed, ~2.3GB extracted).
- Ensure you have sufficient disk space and memory (~8–16GB recommended).
- The preprocessing pipeline filters spam, trims metadata, and prepares the dataset for classification.
