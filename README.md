# CourseProject

### Presentation and Tutorial Available at - https://mediaspace.illinois.edu/media/t/1_ammbs24f?st=0

### Code folder contains 

1. Final Project V4.ipynb  (whole source code)
2. Test.ipynb (Code for testers to run)
3. requirements.txt (libraries to install)
4. sentiment_analyzer.joblib (trained sentiment classifier model)

### Data Folder contains 

1. preprocess_airbnb.csv (Airbnb data with necesaary n-grams extracted with source code  to be used for topic extraction and sentiment analysis)
2. preprocess_hotel.csv (Hotel data with necesaary n-grams to be used for topic extraction and sentiment analysis)

### Complete documentation available in Project Documentation.pdf

### Software Implementation and Usage

#### 1. (Optional) Create a Python3 virtual environment

```python3 -m venv py3-env-final-proj```

#### 2. (Optional) Activate virtual environment

```source py3-env-final-proj/bin/activate``` 

#### 3. ```pip install jupyter```

#### 4. Install ipykernel in this environment-  

```python3 -m ipykernel install --user —name=final-proj```
 
 (final-proj will be used as env in jupter notebook)

#### 5. 

```pip install -r requirements.txt```

#### 6. Start Jupyter-notebook from shell using command :  

```jupyter notebook```

#### 7. Download repository and open the Test.ipynb file 

#### 8. Switch to final-proj kernel defined in step 4.

#### 9. Change the file path to where the preprocessed files are i.e. under folder data and Run all the cells in the notebook
