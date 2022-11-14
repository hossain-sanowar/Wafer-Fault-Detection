# Problem Statement:

* Various sensor inputs for various wafers have been supplied. A wafer (also known as a slice or substrate) is a thin slice of semiconductor material used in the manufacture of integrated circuits.

* The objective is to develop a machine learning model capable of predicting whether a wafer has to be changed or not (i.e., whether it is functioning or not) based on the inputs from several sensors. Two classes exist: +1 and -1.

# Project Steps:
1. Template Create using Bash:
```
chmod +x bash_script.sh
./bash_script.sh
```
2. Virtual Environment Create using Bash: `setup.sh`
```
chmod +x setup.sh
./setup.sh
source virtualenv/bin/activate
```
3. Create web application using Flask API
```
touch app.py
pip install -r requirements.txt
python app.py
```
4. Create yaml file through github for some scripting
link: https://github.com/marketplace/actions/build-push-and-release-a-docker-container-to-heroku
```
mkdir .github
mkdir .github/workflows
touch .github/workflows/main.yaml
```
5. Create Docker File 
```
touch Dockerfile
FROM python:3.7
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
EXPOSE $PORT
CMD gunicorn --workers=4 --bind 0.0.0.0:$PORT app:app
```
6. Create `setup.py` file to find the own packages and py module
7. Create Heroku deployment file: runfile and procfile
7.1 Inside the runfile: just write python version for heroku
```
touch runtime.txt
touch Procfile
```
