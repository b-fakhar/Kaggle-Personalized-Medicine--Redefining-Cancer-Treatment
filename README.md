# Kaggle-Personalized-Medicine---Redefining-Cancer-Treatment
https://www.kaggle.com/c/msk-redefining-cancer-treatment

# Problem Statement
Although it is know that genetic testing is going to disrupt the way diseases like cancer are treated, this is only partially happening due to the huge amount of manual work this task required.

A cancer tumor can have thousands of genetic mutations. Classifying every single genetic mutation based on evidence from text-based clinical literature is a very time-consuming task since a clinical pathologist has to manually review and classify every single genetic mutation based on evidence from text-based clinical literature.


#  Objective:

- Develop a Machine Learning algorithm to classify the mutations that contribute to tumor growth (drivers) from the neutral mutations (passengers) based on clinical evidence (text).

- Design a highly accurte ML pipeline since this is a medical related problem and error can be really costly. Therefore, we would like to have result for each class in terms of Probablity (More accurate model at cost of lager processing time of ML algorithm is acceptable). 

- Have a highly interpritable model since a medical practitionar needs to provide proper reasonining on why ML algorithm is predicting any class.

Note: This is not a trivial task since interpreting clinical evidence is very challenging even for human specialists. Therefore, modeling the clinical evidence (text) will be critical for the success.

# Dataset:
This Kaggle project has two traning datasets, which are linked via the ID field:
- training_variants - a comma separated file containing the description of the genetic mutations used for training. Fields are
    - ID (the id of the row used to link the mutation to the clinical evidence).
    - Gene (the gene where this genetic mutation is located).
    - Variation (the aminoacid change for this mutations). 
    - Class (1-9 the class this genetic mutation has been classified on).
- training_text - a double pipe (||) delimited file that contains the clinical evidence (text) used to classify genetic mutations. Fields are 
    - ID (the id of the row used to link the clinical evidence to the genetic mutation)
    - Text (the clinical evidence used to classify the genetic mutation)

training/test_variants provides the information about the genetic mutations, whereas the other (training/test_text) provides the clinical evidence (text) that our human experts used to classify the genetic mutations. Both are linked via the ID field.

Note: Some of the test data is machine-generated to prevent hand labeling. 


