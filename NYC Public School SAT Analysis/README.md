NYC Public High School SAT Score Analysis
-----------------------

Analysis of 2011 SAT scores of NYC 13 district high schoolers, among with various demographic and other information about them

*479 High School SAT score with demographic and graduation data

*District Level Data Visulization

*District Level NYC High School Clustering

Background Information
----------------------


1.New York City is divided into 5 boroughs, which are essentially distinct regions.

2.Schools in New York City are divided into several school district, each of which can contains dozens of schools.

3.Not all the schools in all of the datasets are high schools, so we’ll need to do some data cleaning.

4.Each school in New York City has a unique code called a DBN, or District Borough Number.

5.By aggregating data by district, we can use the district mapping data to plot district-by-district differences.


Data
----------------------
The Detail information of Data and its download link are list below

1.[2010 ap test resut](https://data.cityofnewyork.us/Education/AP-College-Board-2010-School-Level-Results/itfs-ms3e)

2.[2010-11 class size](https://data.cityofnewyork.us/Education/2010-2011-Class-Size-School-level-detail/urz7-pzb3)

3.[2006-12 demographic](https://data.cityofnewyork.us/Education/School-Demographics-and-Accountability-Snapshot-20/ihfw-zy9j)

4.[2005-10 graduation outcomes](https://data.cityofnewyork.us/Education/Graduation-Outcomes-Classes-Of-2005-2010-School-Le/vh2h-md7a)

5.[2010-11 School Attendance and Enrollment Statistics by District (hs_directory.csv)](https://data.cityofnewyork.us/Education/School-Attendance-and-Enrollment-Statistics-by-Dis/7z8d-msnt)

6.[2006-10 Math Result](https://data.cityofnewyork.us/Education/NYS-Math-Test-Results-By-Grade-2006-2011-School-Le/jufi-gzgp)

7.[2012 SAT Score Result](https://data.cityofnewyork.us/Education/SAT-Results/f9bf-2cp4)

8.[school district map](https://data.cityofnewyork.us/Education/School-Districts/r8nu-ymqj)

Installation
----------------------

### Download the data

* Clone this repo to your computer.

* Get into the folder using `cd NYC Public School SAT Analysis`.

* Switch into the `data` directory using `cd data`.

* Download the data files from the above links

* Extract all of the `.zip` files you downloaded.

* Remove all the zip files by running `rm *.zip`.

* Switch back into the `NYC Public School SAT Analysis` directory using `cd ..`.

### Install the requirements
 
* Install the requirements using `pip install -r requirements.txt`.
    * Make sure you use Python 2.7.
    * You may want to use a virtual environment for this.

Usage
-----------------------

* Run  `main.ipynb` in jupyter notebook to do the analysis
