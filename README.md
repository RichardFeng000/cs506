# cs506 midterm: Amazon Movie Star Rating Prediction
### Kaggle: Ruiding Feng 
## Introduction
#### This project examines the realtionship between the star rating score between user reviews from Amazon Movie Reviews using the available features. The features include unique identifier for the product/user, the number of users who found the review helpful, the number of users who indicated whether they found the review helpful, the timestamp for the review, the brief summary of the review and the text of the review. In the rest of this notebook, I’m going to utilize these features on the prediction of the star rating score. This project, if successful, is beneficial to estimate any unlisted movie’s popularity or reputation, which could be further used in the recommendation system in this field.
## User ID & Product ID 
There are more than 1 million records inside the dataset. User IDs and product IDs are not the data we need. They don't help or influence our predictions and we can leave them alone. User IDs and product IDs are not the data we need. They don't help or influence our predictions and we can leave them alone.
<img width="293" alt="Screen Shot 2022-11-07 at 7 53 44 PM" src="https://user-images.githubusercontent.com/63218692/200452321-550d0336-4595-4549-95c1-a77b6a8dbd7e.png"> <img width="116" alt="Screen Shot 2022-11-07 at 8 11 37 PM" src="https://user-images.githubusercontent.com/63218692/200452227-86a22d55-8ffb-41c2-adbc-eadcb2ff45fb.png">
## Helpfulness Numerator & Denominator
We need to divide the total number of people evaluated by the total number of people viewed. Then will get the one called helpfulness.
<img width="389" alt="Screen Shot 2022-11-07 at 7 53 57 PM" src="https://user-images.githubusercontent.com/63218692/200453107-de865864-7420-4637-9a73-9553ea865238.png"> <img width="467" alt="Screen Shot 2022-11-07 at 8 11 24 PM" src="https://user-images.githubusercontent.com/63218692/200453153-09211a69-e5c0-45cf-bf09-e4ea2f282c0e.png">

## Summary & Text
There are some users who do not leave text or summaries, so we cannot include them inside our training data. Then we set them to Zero.
<img width="418" alt="Screen Shot 2022-11-07 at 7 53 31 PM" src="https://user-images.githubusercontent.com/63218692/200456527-90d49655-a722-4dfa-9b3f-55c02c1df494.png"> <img width="406" alt="Screen Shot 2022-11-07 at 7 54 16 PM" src="https://user-images.githubusercontent.com/63218692/200456640-5bc32dc1-e93f-4399-a256-52b32e4221b9.png">
