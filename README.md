# **Google-Trends-Analyzer**

A Python script that scrapes and analyzes data using Google Trends and various Python  libraries.

![image](https://user-images.githubusercontent.com/108644811/218410166-55c0f2c1-6567-44d5-b5e7-1d2c08ab7f02.png)

# π₯ Installation Guide

### Step 1 : Clone the Repository

Clone the repository using the following command.

```
$ git clone https://github.com/sbeen1840/Google-Trends-Analyzer.git
```

### Step 2 : Install Dependencies

**Note** : It is recommended to use a `conda environment` with `Python 3.6` with this code. Before running the commands in this guide, make sure you activate the environment using `$ source activate <name of the env>`

The use the `requirements.txt` file given in the repository to install the dependencies via `pip`.

```
$ pip install -r requirements.txt
```

### Step 3 : Verify the installation of dependencies

To verify whether `pandas`, `pytrends` and `trend` were installed properly, run the following.

```
$ python
>>> import pandas
>>> import pytrends
>>> import trend
```

If there are no error messages upon importing the above dependencies, it would indicate that the they are correctly installed.

# π Usage

### Step 1 : Update the keywords in the three CSV files.

|1|2|3|4|5|
|---|---|---|---|---|
|JAVA| java|
|C++| c++|
|PYTHON| python| py| PY|
|javaScript| javascript| JAVASCRITP|

Suppose you have a CSV file containing keywords up to five in one row.

The first index of each row becomes the representative keyword.

Keywords similar to the representative keywords may be entered in each row.

### Step 2 : Change the route of csv file and set the themes of the files in main.py

```
csv1 = "C:/Users/user/Desktop/swa-java-2023/ννλ‘μ νΈ/keyword_language.csv"
csv2 = "C:/Users/user/Desktop/swa-java-2023/ννλ‘μ νΈ/keyword_jobgroup.csv"
csv3 = "C:/Users/user/Desktop/swa-java-2023/ννλ‘μ νΈ/keyword_academy.csv"

theme1 = "νλ‘κ·Έλλ°μΈμ΄"
theme2 = "κ°λ°μ§κ΅°"
theme3 = "κ°λ°κ΅μ‘"
```

### Step 3 : Change the variables for data collection in trend.py file.
```
self.numb = 2 # μμλΆν° μΆμΆ κ°μ 
self.lang = 'ko' # pytrend κΈ°μ€ μΈμ΄ μ€μ 
self.time = 540 # pytrend κΈ°μ€ μκ°λ μ€μ 
self.geo = 'KR' # pytrend κΈ°μ€ μμΉ μ€μ 
self.month = 1 # νμ¬λΆν° nκ°μκ°μ κΈ°λ‘ (μ μλ§ μλ ₯)
self.update = 1 # μλ°μ΄νΈν  μ£ΌκΈ°(λ¨μ sec)  # 86400 νλ£¨
self.address = csv_address # main.pyμμ μ§
self.dicts = 7 # jsonνμΌμ μ΄κΈ°
```


### Step 4 : Run the script by typing python `main.py` in the terminal.
![image](https://user-images.githubusercontent.com/108644811/218135256-a527b011-0b86-4f49-98ee-83b8b41698b1.png)

### Step 5 : Access the data by visiting `http://localhost:5000/home` in your web browser.

After running the script, you can access keywords representing the search trend by visitingΒ [http://localhost:5000/home](http://localhost:5000/home) in your web browser. You can also see their search volume, normalized. The data will be presented in the form of  json and sorted in descending order.

# π‘ Results
|Web json data http://localhost:5000/home |
|:---:|
|![image](https://user-images.githubusercontent.com/108644811/218414366-905ba67a-d3e1-4375-ae13-2c011fe7d6bd.png)|
|Console output |
| ![image](https://user-images.githubusercontent.com/108644811/218413841-05fec875-6d98-48b4-9215-0130952b2411.png)|




# π Execution

`docs/trend_exec.ipynb` describes the execution steps of this program pipeline in detail.

# π Notes

As of `2023/02/10`, the above installation and execution steps are only tested on `Window11`. We will update as soon as we test the installation and execution steps on `Linux` and `MacOS`.

# π€ Authors

- sbeen1840

# π· License

- This project is licensed under the `MIT License` - see the [LICENSE](notion://www.notion.so/LICENSE) file for details

# π Acknowledgments

# β References
