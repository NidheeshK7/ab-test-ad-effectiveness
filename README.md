# Did the ad campaign lift conversion enough to justify spend?

This project analyses an A/B test of an online ad campaign. Users were randomly assigned to see either an **ad** (treatment) or a **public service announcement (PSA)** in the same slot (control). The question is whether the ad lifted purchases by enough to pay for the impressions.

*Work in progress: the analysis is being built in [`analysis.ipynb`](analysis.ipynb).*

## Data

The data is [Marketing A/B Testing](https://www.kaggle.com/datasets/faviovaz/marketing-ab-testing) on Kaggle: the file `marketing_AB.csv`, with one row per user.

**To download:** get `marketing_AB.csv` from the Kaggle page linked above (you need a free Kaggle account) and save it as `data/marketing_AB.csv`. The `data/` folder is git-ignored, so the file is never committed.

## How to run

You need Python 3.12 or newer.

```bash
git clone https://github.com/NidheeshK7/ab-test-ad-effectiveness.git
cd ab-test-ad-effectiveness
python3 -m venv venv
source venv/bin/activate          # Windows: venv\Scripts\activate
pip install -r requirements.txt
# download marketing_AB.csv from Kaggle into data/ (see "Data" above)
jupyter notebook analysis.ipynb   # then Kernel > Restart & Run All
```
