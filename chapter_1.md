# Installing Data Science Tools
This chapter of the workshop will focus on installing the necessary tools for fundamental data science analysis. We will be coding in Python, using the
Jupyter Lab developer environment.

## Installing Python
[Click here to download Python](https://www.python.org/downloads/)

## Installing JupyterLab
Open a terminal and type the following code
```
pip install jupyterlab
```
**note: customize the installation to ensure that pip is installed**

## Installing Python Packages
Now that we have Python installed and a developer environment (IDE) to run Python programs, we can install the most important Python packages that are
relevant to data science.

### 1. NumPy
NumPy is a fundamental package for scientific computing in Python. Its most handy feature is facilitating array-like math and data storage.
```
pip install numpy
```

### 2. SciPy
Similar to NumPy, SciPy is a library designed for adding functionality to standard Python that would be useful to scientists, mathematicians, and 
engineers. One feature I really like is the [linear regression package](https://docs.scipy.org/doc/scipy-1.6.2/reference/generated/scipy.stats.linregress.html).
```
pip install scipy
```

### 3. Matplotlib
Matplotlib is a plotting tool for making charts and figures in Python. It is a very popular feature for data visualization.
```
pip install matplotlib
```

### 4. Pandas
Pandas is a tool used to read and manipulate datasets. It represents data as "DataFrame" objects which makes them easier to handle than raw Python data 
types. Pandas requires several dependencies, which should get installed when we use pip...
* setuptools
* dateutil
* numpy (installed in 1)
* pytz
type the following command into the terminal to install
```
pip install pandas
```

# Checking for a proper install
1. To verify that Python is installed, type in the terminal
```
python --version
```
This command should yield the Python version number. If it does not, then try re-installing Python!
2. Next, run the Jupyter Lab by typing in the terminal
```
jupyter lab
```
If this command does not work, then try re-installing Jupyter.
3. Download the file called *verify_install.ipynb*, located in the *chapter_1* folder of this repo and place it in your project folder. 
4. Navigate to your project folder, open the *verify_install.ipynb* file, and select *Run -> Run All Cells*.
5. The notebook should run without error, indicating that all packages were installed correctly. If it does not, try re-installing the packages.

# Saving your installation details
Now that you've successfully installed the fundamental tools for data science in Python, you can save the details of your installation using a
*requirements.txt* file. To do this, open your terminal and type 
```
pip freeze > requirements.txt
```
this saves all of the packages and their version numbers so that the environment can easily be recreated using 
```
pip install -r requirements.txt
```
