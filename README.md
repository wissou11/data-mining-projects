# Data Mining Projects

Two mini-projects on Tunisian data that follow the same progression: baseline models, an improvement step, a tuned neural network, a specialized model, then a prediction map in UTM 32N.

**Author:** Wissem Bahrouni

| Project | Question | Specialized model | Best R² on tabular target | Best R² overall |
| --- | --- | --- | --- | --- |
| [Hotel satisfaction](hotel-satisfaction/) | Can tabular data and French reviews predict satisfaction? | TF-IDF + Ridge | 0.3259 (tuned MLP) | 0.8350 (TF-IDF + Ridge) |
| [Drought risk](drought-risk/) | Can climate data forecast drought risk? | LSTM | 0.8183 (Random Forest + KMeans) | 0.9442 (tuned LSTM) |

The best overall model in each project predicts a different target from the tabular models. Each project's README covers this and its other limitations.

Each folder contains a notebook with saved outputs, a report in French and the main figures.

## Setup

Developed on Python 3.11.

```bash
git clone https://github.com/wissou11/data-mining-projects.git
cd data-mining-projects
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

## Tech stack

Python, pandas, NumPy, scikit-learn, XGBoost, TensorFlow/Keras, GeoPandas, pyproj, Matplotlib
