# Data Engineering Project
The objective of this project was to write datasets of varying formats into a more convenient and user-friendly SQLite3 database file. All code was written in Python to take advantage of the pandas library. Similar work could be performed using SQL, but Python can often be easier to work with and connects well to SQLite3. 

The Jupyter Notebook found in this project has descriptive comments and outputs visible to make it easy to follow. If you wish to run the code yourself, follow the following instructions.

## Downloading Project
With git installed, this project can easily be downloaded locally by using 
`git clone https://github.com/neginkrahbar/Data-Engineering-Project.git`.

Alternatively, the project can be downloaded as a zip file using the green `Clone or download` button above.
It is recommended to download the entire project, as the data referenced in the code is contained in the folder.

## Installation Notes
The following are required to run this code:
* Python 3.4+ https://www.python.org/
* pandas https://pandas.pydata.org/
* xlrd https://pypi.org/project/xlrd/
* SQLite3

A Jupyter Notebook was used because of the great interactive coding experience. This is not required, but is highly recommnded. An easy way to get all the required software is by using the conda environment manager. Installing [miniconda](https://conda.io/miniconda.html) will get the basics set up, and any additional required packages can be added using the command `conda install package_name`.

With Jupyter installed, a Jupyter server must be launched by running the command `jupyter notebook`. This should open a page in the default browser where one can navigate through directories and open the project notebook. Each code block can be quickly and easily run by selecting the block and pressing `return`+`shift`.

## Data Information
There were three datasets used in this project: 
* Annual Estimates of the Resident Population - Metropolitan Statistical Area; and for Puerto Rico (2010-2017) [link](https://www.census.gov/data/datasets/2017/demo/popest/total-metro-and-micro-statistical-areas.html)
* Annual Average Unemployment Statistics - County Data (2010-2017) [link](https://www.bls.gov/lau/#tables)
* Annual Estimates of the Resident Population for Counties (2010-2017) [link](https://www.census.gov/data/datasets/2017/demo/popest/counties-total.html)
The actual files used can be found in the project.

## Output Information
The dataframes were written into a SQLite3 database file called popData containing two tables: 
* popMetropolitan - Table contains annual population estimates from 2010-2017 for the major metropolitan areas in the US, as well as the annual estimated US population that lives in a major metropolitan area. 
* popUnemploymentCounty - Table contains annual population estimates and annual unemployment rate from 2010-2017 for US counties.

A SQLite3 database file can be queried using terminal, Python (here is a useful [guide](https://sebastianraschka.com/Articles/2014_sqlite_in_python_tutorial.html)), or another interface.