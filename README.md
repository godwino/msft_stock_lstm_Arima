# msft_stock_lstm_Arima
Microsoft stock prediction

Microsoft Stock Price Forecasting

                        Introduction
In the domain of quantitative finance, accurate predictions of stock prices constitute a pivotal challenge. This project aims to forecast the future stock prices of Microsoft Corporation (NASDAQ: MSFT) by implementing and juxtaposing two distinct time-series models: LSTM (Long Short-Term Memory) and ARIMA (AutoRegressive Integrated Moving Average). Through rigorous analysis and application of these models, we seek to identify patterns in historical price movements to forecast future values.
with a focus on model optimization through hyperparameter tuning for enhanced predictive performance.


                          Repository Structure
src/: Source code for LSTM and ARIMA models, including preprocessing and tuning scripts.
data/: Historical stock price data used for training and testing the models.
notebooks/: Jupyter notebooks containing exploratory data analysis and initial model development.
models/: Serialized final models and configuration files.
requirements.txt: List of dependencies for replicating the analysis environment.
LICENSE: Terms of distribution and use for the project.

                            Dataset
The dataset includes daily stock prices of Microsoft Corporation from march 13,1986 to the current date sourced from Yahoo Finance, with the following features:

Date
Open
High
Low
Close
Adjusted Close
Volume

                            Hyperparameter Tuning

Hyperparameter tuning is a critical step in optimizing machine learning models for better performance. For the LSTM model, we utilized a grid search approach to iterate over a predefined range of hyperparameters, including:
Number of layers
Number of neurons per layer
Learning rate
Dropout rate
For the ARIMA model, we conducted a stepwise search to determine  the optimal values of p (order of the autoregressive part), d (degree of differencing), and q (order of the moving average part).
The hyperparameter tuning process is automated with scripts located in src/tuning, which can be run to replicate our results or to seek further improvements.

                           Model Improvement

Continuous improvement of the models is achieved by:
Regularly retraining the models with new data.
Incorporating additional features such as trading volume and sentiment analysis from news articles.
Ensemble methods that combine the predictions from both LSTM and ARIMA models.
We encourage experimentation with different model architectures, feature sets, and tuning strategies to enhance the model's predictive capabilities.

                             Evaluation
Models are evaluated using RMSE,for lstm was 5.92 why Arima was 9.46,This project show LSTM performs better than Arima. alongside visual comparison of predictions with actual stock prices. Detailed evaluation results are provided for both pre- and post-tuning performance.

                            Contributions
We value contributions and encourage the community to propose enhancements, report bugs, or submit pull requests. Please read through CONTRIBUTING.md for guidelines on the contribution.

Contact
Project Maintainer: [GODWIN OSAYAMWEN] - [godwinosayamwen@gmail.com]
Project Link: https://github.com/Godwino/msft_stock_lstm_Arima
