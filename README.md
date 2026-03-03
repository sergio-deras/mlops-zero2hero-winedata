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

3. Init DVC
    dvc init (might need to force)

4. You can get some data from:
    https://archive.ics.uci.edu/dataset/186/wine+quality

5. You need to create your S3 bucket and configure AWS CLI access 

6. dvc add data/winequality-red.csv 
    A .dvc file is created, this is the one that will be in Git

7. Configure your remote repo
    dvc remote add -d mlops-zero2hero s3://mlops-zero2hero-dvc-bucket

8. Push your changes
    dvc push

These are not configured as versions, these are saved in different folders (diff objects)