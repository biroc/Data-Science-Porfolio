Credit modelling using linancial lending data from Lending Club
------------------------------------------

Modeling Credit status by making predictions about whether or not a loan will be paid off on time, which is contained in the *loan_status* column of the clean dataset.

40000 approved loan data with loan status feature from 2017 to 2011 are analyzed in the project. The datasets using in the project is in the Data folder.

Using False Positive Rate(fpr) and Accuracy as error metric. With a false positive, we predict that a loan will be paid off on time, but it actually isn't. This costs us money. Our objective in this is to make money -- we want to fund enough loans that are paid off on time to offset our losses from loans that aren't paid.

Prediction Goal: Minimize the fpr results to reduce the risk; Maximize the Accuracy to maximize the potential money.

Results
----------------------
* Linear Regression with self defined weight penality
	* 33.02% Accuracy
	* 8.41% fpr

* Random Forest tree with balance weight penality
	* 85.19% Accuracy
	* 97.34% fpr

* Deep Forward Neural network(FNN) with self defined weight penality
	* 85.01% Accuracy
	* 14.99% fpr


Background Information
----------------------

Lending Club is a marketplace for personal loans that matches borrowers who are seeking a loan with investors looking to lend money and make a return. Each borrower fills out a comprehensive application, providing their past financial history, the reason for the loan, and more. Lending Club evaluates each borrower's credit score using past historical data (and their own data science process!) and assign an interest rate to the borrower.

Usage
-----------------------

* Run `mkdir Processed` to create a directory for our processed datasets.
* Run  `clean.ipynb` in jupyter notebook to combine the sql dataset and clean the data
    * This will create `clean_loan_2007.csv` in the `Processed` folder.
* Run `prediction.ipynd`.
    * This will create logistic regression,random forest, and FNN prediction results
