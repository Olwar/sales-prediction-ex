When developing machine learning models, it is important to document the process thoroughly to ensure that the work is reproducible and understandable to others. Here are some recommended best practices for documenting machine learning models:

    Problem Statement: Clearly define the problem that the model is trying to solve and the objectives of the project.
    Forecasting future total sales of ABCD's items based on the historical total sales.

    Data: Describe the data that is used for training and testing the model. Include details such as the source of the data, the number of samples, and any pre-processing steps that were applied to the data.
    The data is day-to-day total sales of ABCD's items from 21.08.2022 to 01.11.2023. It includes 144 datapoints.
    No pre-processing steps were needed for the data, it didn't include any missing or outlier values.

    Feature Engineering: Describe any feature engineering that was done, including the features that were created and the reasoning behind their creation.
    Feature Engineering was done for the LSTM and Prophet. Lagged sales from 1 to 5 days were added and rolling mean of 5, 10, 15 and 20 days' sales were added. I did not improve performance.

    Model Selection: Record the models that were tried and their performance, including the model's architecture, hyperparameters and any other relevant details.
    There are many models that can be used for Time-Series forecasting. These include Linear Regression, ARIMA, Random Forest, XGBoost,
    LSTM, DeepAR and Prophet. In this project all of these were tried except DeepAR. After fine-tuning and feature engineering ARIMA turned out to be the most accurate of these.
    Prophet: 55.80 MAE (and weird prediction)
    ARIMA: 23.56 MAE
    LSTM: 39.28 MAE  

    Evaluation: Document the evaluation metrics that were used to evaluate the model's performance. This could include metrics such as accuracy, precision, recall, F1-score and MAE among others.
    For evaluation Mean Absolute Error (MAE) was used.

    Results: Summarize the performance of the model and any conclusions that can be drawn from the results.
    The MAE of the ARIMA model was XXX, this means the model's prediction from the actual sales in the test was off by XXX on average. 


    Deployment: Describe how the model will be deployed and used in production, including any considerations for scaling, monitoring, and maintenance.
    Once the model is deployed, it is important to monitor its performance. This can be done by tracking key performance indicators such as mean absolute error (MAE to ensure that the model is performing as expected.


    Code: Keep the code organized and well-documented, with clear explanations of the functions, variables and methods.

    Version Control: Use version control tools such as Git to track changes to the code and documentation over time.

    Collaboration: Use collaborative tools such as Jupyter Notebook or Google Colab to share the work with others and receive feedback.

By following these best practices, you can ensure that your machine learning models are well-documented and easy to understand, both for yourself and for others who may need to use or build upon your work in the future.
