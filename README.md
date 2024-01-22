# Health_Insurance_Cross_Sell_Prediction-By_Classification
* Our client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.
# Business Context:
Our client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company. An insurance policy is an arrangement by which a company undertakes to provide a guarantee of compensation for specified loss, damage, illness, or death in return for the payment of a specified premium. A premium is a sum of money that the customer needs to pay regularly to an insurance company for this guarantee. For example, you may pay a premium of Rs. 5000 each year for a health insurance cover of Rs. 200,000/- so that if, God forbid, you fall ill and need to be hospitalised in that year, the insurance provider company will bear the cost of hospitalisation etc. for upto Rs. 200,000. Now if you are wondering how can company bear such high hospitalisation cost when it charges a premium of only Rs. 5000/-, that is where the concept of probabilities comes in picture. For example, like you, there may be 100 customers who would be paying a premium of Rs. 5000 every year, but only a few of them (say 2-3) would get hospitalised that year and not everyone. This way everyone shares the risk of everyone else.

Just like medical insurance, there is vehicle insurance where every year customer needs to pay a premium of certain amount to insurance provider company so that in case of unfortunate accident by the vehicle, the insurance provider company will provide a compensation (called ‘sum assured’) to the customer.

Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

Now, in order to predict, whether the customer would be interested in Vehicle insurance, you have information about demographics (gender, age, region code type), Vehicles (Vehicle Age, Damage), Policy (Premium, sourcing channel) etc.

# Dataset Description :
* Id : Unique ID for customer

* Age : Age of the customer

* Driving_License : Customer has DL or not

* Region_Code : Unique code for the region of the customer

* Previously_Insured  : Customer already has Vehicle Insurance or not

* Vehicle_Age : Age of the Vehicle

* Vehicle_Damage  : Past damages present or not

* Annual_Premium : The amount customer needs to pay as premium

* PolicySalesChannel : Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.

* Vintage : Number of Days, Customer has been associated with the company

* Response : Customer is interested or not
# Main Libraries to be Used:
* Pandas for data manipulation, aggregation
* Matplotlib and Seaborn for visualization and behavior with respect to the target variable
* NumPy for computationally efficient operations
* Scikit Learn for model training, model optimization, and metrics calculation
# Project Objective?
* Efficient EDA
* Understanding of how to prep the data and make it ready for training.
* Understanding the target feature and its distribution
* Assessing target features for class imbalance.
* Modeling - which algorithm to use?
* Evaluation while keeping class imbalance in mind.
* Feature Importance and Conclusion
* Understanding how your project is useful to client
# Prediction Models:
To predict the stock's closing price, I developed Seven models: Logitcal Regression, Decision Tree, Random Forest, Gradient Boost , XGBoos, KNN and LightBGM With GridsearchCV. These models were trained using historical data and various features. The Decision Tree and Random Forest model performed exceptionally well both on training and test datasets.
# Evaluation Metrics:
* Precision : Precision is the ratio of true positive predictions to the total number of positive predictions.

* Recall : Recall is the ratio of true positive predictions to the total number of actual positive cases.

* F1-Score : F1-Score is the harmonic mean of precision and recall.

* Support : The support is the number of samples of the true response that lie in that class.

* Confusion Matrix : The confusion matrix shows the number of true positive, false positive, true negative, and false negative predictions made by the model.

* ROC Curve  :A receiver operating characteristic curve, or ROC curve, is a graphical plot that illustrates the diagnostic ability of a binary classifier system as its discrimination threshold is varied. The ROC curve is created by plotting the true positive rate (TPR) against the false positive rate (FPR) at various threshold settings. The true-positive rate is also known as sensitivity, recall or probability of detection in machine learning. The false-positive rate is also known as probability of false alarm and can be calculated as (1 − specificity).

* Classification Report : The classification report visualizer displays the precision, recall, F1, and support scores for the model. In order to support easier interpretation and problem detection, the report integrates numerical scores with a color-coded heatmap. All heatmaps are in the range (0.0, 1.0) to facilitate easy comparison of classification models across different classification reports.
# Conclusion:
* The gender variable in the dataset is spread nearly evenly. The male category is marginally larger than the female category, and the likelihood of purchasing insurance is also slightly higher. The response rate of those who are not interested in purchasing vehicle insurance is higher than that of those who are interested in buying vehicle insurance.Only 12.3% people are interested in buying vehicle insurance and 87.7% are not interested in buying vehicle insurance. So people who own the bike may already have vehicle insurance, or people might not be aware of insurance policy and pricing factors, which means the firm needs to come up with good marketing techniques and a pricing strategy to create awareness and offer an affordable price to the customers in order to reach out to more customers to generate more leads.

* The response rate of those who are not interested in purchasing vehicle insurance is higher than that of those who are not interested in buying vehicle insurance. 99.8% of customers have DL, whereas 0.2% do not have DL. Only a small percentage of people who have a DL (12.2%) are interested in purchasing vehicle insurance. So almost all the people who own vehicles have DL because it's mandatory when you have a bike, and only a small percentage of people are interested in buying vehicle insurance. The possible reason might be that people who own the bike may already have vehicle insurance or insurance might be expired.

* 45.8% of people are insured previously, in that 12.2% of people interested to buy the vehicle insurance again, Which means people are aware of insurance policy and ready to pay a premium amount, for better off taking actions to avoid certain risks or reduce risk. So buying insurance makes the most sense when the potential loss is great and there is a significant probability of loss.

* Around 4.2% of vehicles are more than two years old, 52.6% are between one and two years old, and 43.2% are under one year old. 1.2% are interested in purchasing vehicle insurance for vehicles older than 2 years, 9.1% are interested in purchasing insurance for vehicles between 1 and 2 years old, and 1.9% are interested in purchasing insurance for vehicles older than 1 year. As vehicle age increases most of the people are aware of insurance and interested to buy the insurance for reducing the risk.

* 50.5% of the vehicles have past damage.12.0% of people who have had a damaged vehicle in the past want to acquire vehicle insurance. So 50 percent of vehicles are damaged and 50 percent are not damaged, which means people with damaged vehicles (12%) are interested in buying insurance and are aware of vehicle insurance policies and its benefits, while the rest of the people might already have purchased insurance and do not need to purchase again.

* Around 4.2% of vehicles are more than two years old, 52.6% are between one and two years old, and 43.2% are under one year old. 1.2% are interested in purchasing vehicle insurance for vehicles older than 2 years, 9.1% are interested in purchasing insurance for vehicles between 1 and 2 years old, and 1.9% are interested in purchasing insurance for vehicles older than 1 year. As vehicle age increases most of the people are aware of insurance and interested to buy the insurance for reducing the risk.

* The dataset has more individuals with an age of 24. 40 to 60-year-olds had a higher likelihood of purchasing vehicle insurance. 9.3% of people in their middle age are interested in purchasing insurance. Almost 47% of middle-aged individuals have a driver's licence. About 21.9% of people in their teens have health insurance. Around 21.9% of persons in their teens have had insurance previously. So most teenagers have insurance and are aware of their policy. So the target audience might be middle-aged people and teenagers to generate more leads for insurance companies.

## Happy Learning
