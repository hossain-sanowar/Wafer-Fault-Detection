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