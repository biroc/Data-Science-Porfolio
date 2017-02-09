Soccer Result Prediction
-----------------------

Predict 2008-2016 soccer game results(Win/Draw/Lose) of 11 European lead league based on the 25K+ match result Kaggle datase [here](https://www.kaggle.com/hugomathien/soccer). The prediction is based on the bet odds and the FIFA game team attribute.

*+25,000 matches

*+10,000 players

*11 European Countries with their lead championship

*Seasons 2008 to 2016

*Players and Teams' attributes* sourced from EA Sports' FIFA video game series, including the weekly updates

Result
----------------------

The Deep FNN gives us 53.86% Accuracy in test set and 53.12% accuracy in validation set.
The Random Forest gives us 50.42% Accuracy in test set and 50.33% accuracy in validation set.

Installation
----------------------

### Download the data

* Clone this repo to your computer.

* Get into the folder using `cd soccer-prediction`.

* Switch into the `data` directory using `cd data`.

* Download the data files from Kaggle into the `data` directory.  
    * You can find the data [here](https://www.kaggle.com/hugomathien/soccer).

* Extract all of the `.zip` files you downloaded.

* Remove all the zip files by running `rm *.zip`.

* Switch back into the `loan-prediction` directory using `cd ..`.

### Install the requirements
 
* Install the requirements using `pip install -r requirements.txt`.
    * Make sure you use Python 2.7.
    * You may want to use a virtual environment for this.

Usage
-----------------------

* Run `mkdir Processed` to create a directory for our processed datasets.
* Run  `clean.ipynb` in jupyter notebook to combine the `Acquisition` and `Performance` datasets.
    * This will create `clean_data.csv` in the `Processed` folder.
* Run `classic.ipynd`.
    * This will create random forest prediction results
* Run `FNN.ipynd`.
    * This will cread Forward Neural network prediction results