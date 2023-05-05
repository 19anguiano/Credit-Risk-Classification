# Credit-Risk-Classification

## Analysis Overview
The purpose of this analysis is to create an efficient model that can determine the creditworthiness of borrowers. The data included vital information, such as: loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks, total debt, and loan status. In order to create the model, I assigned the loan status column to the labels set (y) and the remaining columns to the features (X). I used 'value_counts' on the labels set and found the data was not balanced; there are 75,036 healthy loans and 2,500 high risk loans in the dataset. The data was then split into training and testing datasets by using 'train_test_split.' Two Logistic Regression Models were created, each with a slightly different approach. Both approaches included using the LogisticRegression classifier, fitting the model, making predictions, and evaluating the model's performance. The first approach created the model with the original data, while the second approach utilized reampled training data. The resampled data had a 1:1 ratio of healthy and high risk loans.

## Results
 - Machine Learning Model 1 (Original Data)
    - Balanced Accuracy Score: 0.9520479254722232
    
    ![original_data](https://user-images.githubusercontent.com/119361768/236379890-64360eb3-5e02-421f-a448-ec3b09c7da95.png)

 
 - Machine Learning Model 2 (Reasmpled Data)
    - Balanced Accuracy Score: 0.9936781215845847
    
    ![resampled_data](https://user-images.githubusercontent.com/119361768/236379905-efd6555e-dfb8-4443-96f0-2bbe49f8b1e7.png)

## Summary
Overall, both machine learning models performed well. However, I'd recommend the second model which used the resampled data, since the data is more balanced. This model yielded higher balanced accuracy and recall scores. Predicting both healthy and high risk loans are important, however high risk loans may have a higher importance. Predicting high risk loans can ensure lenders are secure.
