create env

```bash
conda create -n simple_env python=3.9 -y
```

Activate env
```bash
conda activate simple_env
```

Create requirements file

Install the requirements
```bash
pip install -r requirements.txt
```

Download the data from:
https://drive.google.com/drive/folders/18zqQiCJVgF7uzXgfbIJ-04zgz1ItNfF5?usp=sharing

```bash
git init

dvc init

dvc add data_given/winequality.csv

git add . && git commit -m "first commit"

git remote add origin git@github.com:satyajeet-prakash/simple_dvc_demo.git

git branch -M main
 
git push -u origin main
```


<h3> Testing </h3>
<pre>Add pytest and tox to requirements file</pre>

tox command - 
```bash
tox
```

tox command for rebuilding -
```bash
tox -r
```

pytest command
```bash
pytest -v
```

setup command
```bash
pip install -e .
```

build your own package commands -
```bash
python setup.py sdist bdist_wheel
```


create an artifacts folder 


mlflow server command - 


mlflow server \
    --backend-store-uri sqlite:///mlflow.db \
    --default-artifact-root ./artifacts \
    --host 0.0.0.0 -p 1234



