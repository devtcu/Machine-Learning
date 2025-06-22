# Machine_Learning

This repository contains a collection of machine learning projects, including:
- Neural networks built from scratch (see `Playground/`)
- Quantitative finance and sentiment analysis notebooks (see `Quant/`)
- Example data science workflows

---

## Setting Up the Environment

This project uses a Python virtual environment to manage dependencies.  
**Do not push your virtual environment folder (`my_venv/`) to GitHub.**

### 1. Create and activate a virtual environment

```bash
python3 -m venv my_venv
source my_venv/bin/activate
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```
*(If `requirements.txt` is missing, install packages as needed, e.g. `pip install numpy pandas matplotlib tensorflow yfinance`)*

---

## Neural Network from Scratch (`Playground/NN_scratch.ipynb`)

- Implements a simple feedforward neural network **without using PyTorch or TensorFlow**.
- Loads and preprocesses the MNIST dataset (CSV files, not tracked in git).
- Demonstrates forward and backward propagation, parameter updates, and accuracy calculation using only NumPy.
- Useful for learning the fundamentals of neural networks and backpropagation.

---

## Quantitative Analysis & Sentiment (`Quant/`)

- **`sentiment.ipynb`**:  
  - Loads Twitter sentiment data for NASDAQ 500 stocks.
  - Calculates engagement ratios (comments/likes) to filter out likely bot activity.
  - Ranks stocks monthly by engagement and simulates a portfolio based on top-ranked stocks.
  - Compares strategy returns to NASDAQ/QQQ.

- **Data**:  
  - The file `sentiment_data.csv` is required but **not tracked in git** (add your own or request a sample).

---

## Data

- **Large files and virtual environments are ignored** via `.gitignore`.
- If you need the MNIST CSVs or sentiment data, download them separately and place them in the appropriate folders.

---

## Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/ML.git
   cd Machine_Learning
   ```

2. **Set up your virtual environment and install dependencies** (see above).

3. **Run the notebooks** using Jupyter or VS Code.

---

## Notes

- **Do not commit your virtual environment (`my_venv/`) or large data files.**
- If you encounter git errors about large files, follow the instructions in the README or use [BFG Repo-Cleaner](https://rtyley.github.io/bfg-repo-cleaner/).
- For any questions or issues, please open an issue on GitHub.

---

Enjoy exploring machine learning and quantitative finance!
