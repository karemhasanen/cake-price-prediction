# Machine Learning Task: Cake Price Prediction

This task has been prepared for the Machine Learning Engineer Virtual Internship Program in Intern2Grow.

## Objective

Your task is to build a machine learning model that can predict the price of cakes based on their features.

## Dataset

You are provided with a dataset containing the following features:

- Sold_On: The day on which the cake has been sold (e.g., Saturday, Sunday, Monday, Tuesday, Wednesday, Thursday, Friday).
- Size: The size of the cake (e.g., small, medium, large).
- Ingredients_Cost: The cost of the ingredients used to make the cake.
- Design_Complexity: The complexity of the cake's design (e.g., simple, complex).
- Time_Taken: The time taken to make the cake (in hours).
- Price: The price of the cake.
- Amount: The amount of similar cakes sold in the same order (Price and all other parameters are for one cake, not the whole order).
- Gender: The gender of person ordering the cake(s).

## Task Breakdown

1. **Data Preparation**: Load and explore the dataset. Perform any necessary data cleaning and preprocessing tasks. This may include handling missing values, dealing with outliers, normalizing the data, encoding categorical variables, etc.

2. **Feature Selection**: Decide which features from the dataset you will use to train your model. Remember that the goal is to predict the price of the cake, so this is your target variable.

3. **Model Selection**: Choose an appropriate machine learning algorithm for this regression task. Justify your choice.

4. **Model Training**: Split the dataset into a training set and a test set. Use the training set to train your model.

5. **Model Evaluation**: Use the test set to evaluate the performance of your model. You may use appropriate metrics for regression tasks such as Mean Absolute Error (MAE), Mean Squared Error (MSE), or Root Mean Squared Error (RMSE).

6. **Prediction**: Finally, use your trained model to predict the price of a new cake given its features.

## Deliverable

Submit a report detailing your approach, methodology, and results. Your report should include:

- An explanation of your data cleaning and preprocessing steps.
- The features you selected and your rationale behind this selection.
- The machine learning algorithm you chose and why you chose it.
- The results of your model evaluation, including the metrics you used.
- A discussion of any challenges you faced and how you overcame them.

Also, submit your code files along with your report. Your code should be well-commented and easy to understand.
