# assignments
Machine Learning Assignments

Assignment 1 -

Problem statement :- An ecommerce company is trying to figure out the average time taken by the user to buy an item since the user logged in.

Approach to the solution, with reference to the different files :- Created a dataset, using different features gathered across multiple users, over various session times, time spent on website, yearly amount spent by the users, and avg time spent by the user to buy an item based on the login time to checkout time difference per session. 
File used in this assignment is "ecommerce_predictions_upd.ipynb"

Known issues and future scope for improvement :- Every dataset has to have multiple features included by default to help us avg the user time to buy an item, if the session length and time spent on website are not part of the feature space then it is not possible to compute and predict the target label.

Assignment 2 -

Problem Statement - To predict the flow of page sequence on an ecommerce website for a user that he ends up purchasing the item or reaching to a final checkout page.

Approach to the solution - This is a case of finding the n-th order markov chain, based on the previous states or pages which the user has visited. We need to calculate the state transition probabilities using markov chain. If the user starts with only a specific page every time then we need to find the next probable page that the user will visit based on the avaialble states and their respective transitions.
Files used for this approach are "uesrflow_varun_markov.ipynb" and the dataset file is "customerflow.csv"

"userflow_predictions.ipynb" is an attempt of creating the proabilities of the page actions and implementing xgboost algorithm on top of that.

Known Issues - Generating a 2nd order markov using transition probability matrix is a viable solution, but creating a n-th order markov chain which doesnt have a fixed number of actions followed by the user to reach a checkout page is an issue that needs to be resolved.

Note - For my personal crave and urge to solve this, I have been reading a book on Markov Models. 
I will keep solving it for my personal interest.
