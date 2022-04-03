Create env
'''bash
conda create -n wineq python=3.7 -y
'''bash

Activate env
'''bash
conda activate wineq
'''bash

Create requirements file

Install the requirements
'''bash
pip install -r requirements.txt
'''bash

download the data from-:
https://drive.google.com/drive/folders/18zqQiCJVgF7uzXgfbIJ-04zgz1ItNfF5?usp=sharing

git init

dvc init

dvc add data_given/winequality.csv

git commit -m "First commit"

one liner update for readme
'''bash
git add . && git commit -m "updated README.md"
'''bash

'''bash
git remote add origin https://github.com/manuvats/simple-dvc-demo.git
git branch -M main
git push -u origin main
'''bash

tox command -
'''bash
tox
'''bash

for rebuilding -
'''bash
tox -r
'''

pytest command 
'''bash
pytest -v
'''

setup commands -
pip install -e .

build your own package commands-
'''bash
python setup.py sdist bdist wheel
'''