create environment

```bash
conda create -n wineqal python=3.7 -y
```

activate environment
```bash
conda activate wineqal
```

create a requirements file and install the req
```bash
pip install requirements.txt
```

```bash
git init
```

```bash
dvc init
```

dvc add will track the data file 
```bash
dvc add data_given/winequality.csv
```

Pushing it to github
```bash
git add . && git commit -m 'first commit'

git remote add origin url

git branch -M main

git push origin main
```

comment to commit dvc stages

```bash
dvc repro
```

dvc cooment to view parmas and scores, also diff

```bash
dvc metrics show

dvc metrics diff
```git config --global --unset http.proxy