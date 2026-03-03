# Keep data

This repository demonstrates TBD
1. TBD
2. TBD

## Quick start (local)
1. Create and activate a venv (example using python 3.13 or 3.11):
    python -m venv .venv
    source .venv/bin/activate

2. Install dependencies:
    pip install --upgrade pip setuptools wheel
    pip install -r requirements.txt

dvc install

dvc init (might need to force)

https://archive.ics.uci.edu/dataset/186/wine+quality

dvc add data/winequality-red.csv

3. Train the model:
    python train.py

4. Run a single prediction from CLI:
    python run_model.py --input "[5.1, 3.5, 1.4, 0.2]"

5. Start the API:
    python src/app.py
   Then test:
    curl -X POST "http://127.0.0.1:5000/predict" -H "Content-Type: application/json" -d '{"features":[5.1,3.5,1.4,0.2]}'
