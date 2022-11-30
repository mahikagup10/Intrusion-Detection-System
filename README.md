# Intrusion-Detection-System
Implementation of Intrusion detection system using machine learning models 

Network Intrusion Detection Using Machine Learning Models.

A training model which helps us determine whether a packet being transmitted is a malicious/spoofed packet or an actual packet.

Multiple machine learning models like KNN, Naive Bayes Algorithm, Decision Tree, Random Forest, SVM, and Logistic Regression are used to determine which model is most efficient.

The dataset used is the regularly updated LUFlow dataset, and the models are trained and tested on the 2022 version. (created less than 6 months ago).
(https://www.kaggle.com/datasets/mryanm/luflow-network-intrusion-detection-data-set)

Methodology:
In order to acquire a general perspective of the dataset, exploratory analysis was done. The null values in the dataset were discovered to be insignificant a nd were disregarded. Analysing the dataset further we found that 2 attributes (src_ip and dst_ip) had only 1 unique value, and hence these columns were dropped from the dataframe.
The six methods that are most used in IDS were found and implemented. The dataset was split as 80% for training the models, and 20% for testing the models.
The accuracy score ,training time, and testing time was found for each model. These metrics were compared to find the model with the highest performance and accuracy. From this we came to the conclusion that the Random Forest model has the best score in terms of accuracy.

How to run the program:
- Download both the .ipynb file and the chosen dataset (.csv file)
- In the python notebook, replace the path for the .csv file with the path of the location of your csv file. (if it is in the same directory and the same file name, ignore this step)
- Run all the cells and note the difference in accuracy amongst all the models presented
- Repeat the steps with different datasets and compare to ensure no skewing of data

References:
Amarudin, Ridi Ferdianand and Widyawan, “A Systematic Literature Review of Intrusion Detection System for Network Security: Research Trends, Datasets and Methods”, 2020 4th International Conference on Informatics and Computational Sciences (ICICoS).

LUFlow Network Intrusion Detection Data Set, uploaded onto Kaggle by Ryan Mills. (Visit https://www.kaggle.com/datasets/mryanm/luflow-network-intrusion-detection-data-set to view more csv files)
