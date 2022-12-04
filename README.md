# cs506 midterm: Amazon Movie Star Rating Prediction
### Kaggle: Ruiding Feng 
## Introduction
#### This project examines the realtionship between the star rating score between user reviews from Amazon Movie Reviews using the available features. The features include unique identifier for the product/user, the number of users who found the review helpful, the number of users who indicated whether they found the review helpful, the timestamp for the review, the brief summary of the review and the text of the review. In the rest of this notebook, I’m going to utilize these features on the prediction of the star rating score. This project, if successful, is beneficial to estimate any unlisted movie’s popularity or reputation, which could be further used in the recommendation system in this field.

summary_matrix = summary_vectorizer.fit_transform(df['Summary'])
```
We used a standardized approach to accelerate the training.
```
scaler = StandardScaler()
```
Storage is done as a matrix to each row and column.
```
for i in range(features_num):
        df["features"+str(i)] = ""
    samples_num = len(df)
    for i in range(samples_num):
        row_list = X.getrow(i)
        row_list = row_list.toarray()
        for j in range(features_num):
            df.at[i, "features"+str(j)] = row_list.tolist()[0][j] 
    return df
```
## Data Preprocessing Summary:
1. Fill in missing values
2. Normalize the values
3. Fit them into the matrix
## Improvements
The computer could have been configured a little better to get more accurate data. Currently my computer crashes if I don't put restrictions on the filtered data.
