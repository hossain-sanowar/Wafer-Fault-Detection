# Problem Statement:

* Various sensor inputs for various wafers have been supplied. A wafer (also known as a slice or substrate) is a thin slice of semiconductor material used in the manufacture of integrated circuits.

* The objective is to develop a machine learning model capable of predicting whether a wafer has to be changed or not (i.e., whether it is functioning or not) based on the inputs from several sensors. Two classes exist: +1 and -1.

# step 1 install cookiecutter
```
$ pip install cookiecutter
```
#MLOps
```
cookiecutter -c v1 https://github.com/drivendata/cookiecutter-data-science

You've downloaded /Users/mdsanowarhossain/.cookiecutters/cookiecutter-data-science before. Is it okay to delete and re-download it? [yes]: yes
project_name [project_name]: wafer
repo_name [wafer]: wafer
author_name [Your name (or your organization/company/team)]: sanowar
description [A short description of the project.]: it's a wafer project using MLOps
Select open_source_license:
1 - MIT
2 - BSD-3-Clause
3 - No license file
Choose from 1, 2, 3 [1]: MIT
Error: 'MIT' is not one of '1', '2', '3'.
Select open_source_license:
1 - MIT
2 - BSD-3-Clause
3 - No license file
Choose from 1, 2, 3 [1]: 1
s3_bucket [[OPTIONAL] your-bucket-for-syncing-data (do not include 's3://')]: 
aws_profile [default]: 
Select python_interpreter:
1 - python3
2 - python
Choose from 1, 2 [1]: 1
```

# Step 2 Create Conda Environment
```
conda create -n wafer python=3.9 -y
conda activate wafer
`````
# STEP 3 Initialize git in Current working directory in your terminal, command prompt or git bash.

```
git init

```
# STEP 4 Install DVC and its gdrive extension

```
pip install dvc
pip install 'dvc[gdrive]'

```
STEP 5 Initialize DVC

```
dvc init

```
STEP 6 Do the first commit and push to the remote repository

```
git add . && git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/<USERNAME>/<REPONAME>.git

```
