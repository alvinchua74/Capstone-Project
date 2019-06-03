Real-Time Consumer Behaviour Prediction and Targeted Marketing Approach
Introduction
E-Commerce is a huge platform which is growing at an unprecedented rate all over the world. People regardless of age loves to shop from different e-stores. Online shopping provides more happiness as compared to physical shopping stores. The reason is simple as we have a lot of websites and apps focusing e-commerce, hence it has become simple to find anything on e-stores that you want to buy immediately. In the coming years, it is expected that thr growth of e-commerce will increase like never before with existing technologies. The rate of online shopping is increasing rapidly, and this is driving e-commerce owners crazy to keep their solid place in the online race. As per a survey, retail e-commerce sales will increase around 200% from 2014 to 2020.

According to a research, Turkish people paid 68.5 billion Turkish liras while shopping online in 2016, which is about 20 billion USD. Considering the internet usage in Turkey(about 60% of citizens use internet), it means each internet user in Turkey spends 450 USD on online shopping in 2016. Considering that the minimum wage is almost 450 USD/month, this is a relatively high amount.

Moving in a technology world, it is highly essential to keep an eye on statistical data. Knowing customers’ need, owners will able to make required changes in their e-commerce websites. With the help of real-time devices, consumer behavior and statistics can be tracked, which is present on the sites. It has been observed that a proper market analysis will always lead to huge profits and customer engagements. This will strategically drive business sales and will ultimately boost online businesses globally.

Hence, I wanted to build a model that predicts consumer behaviour in real-time. The predictions will then push appropriate marketing content to the correct target audience, in order to increase conversion rate and in turn, revenue.

Initial Dataset and Preliminary Modelling
Data of online shoppers' profiles were based on the sportswear website Columbia from Turkey, where data was donated to the UCI machine learning website.

The dataset consists of features belonging to 12,330 sessions. The dataset was formed so that each session would belong to a different user in a 1-year period to avoid any tendency to a specific campaign, special day, user profile, or period.

As this is a imbalanced class binary classification problem, upsampling was done to balance the classes before modelling. Simple models such as Logistic Regression (high interpretability and relatively computational inexpensive compared to other models, therefore easier to scale and quick to compute for deployment) and Random Forests (non-parametric since many of the features used probably would not be linear, reduced overfitting).

The evaluation metric I decided on was F1-score, recall and ROC AUC. Predicting the positive class correctly will aid in increasing revenue generated from consumers who have the intention to purchase. Revenue will be lost if the positive class is misclasiffied, and predicting the negative class correctly will also potentially increase the conversion rate, given that the consumers will be swayed by the marketing content displayed.

Limitations
Some features were masked, so it is not easy to understand the demographics, let alone the dateset being from Turkey. Some Google Analytics data were also aggregated, which makes the analysing a little challenging. The dataset also lies within only one year, hence more patterns may be captured if there are more data over a span of a few years.

Further Modelling
Various models were used for comparison of models' performance, from support vector machines, gradient boosting, and multilayer perceptron were used. XGBoost, with the best F1-score, recall and ROC AUC was chosen as the best model.