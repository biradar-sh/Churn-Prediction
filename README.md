
# Predicting Customer Churn for Telecom Company

This repository contains a deep learning model for predicting customer churn in a telecom company. The model utilizes a deep neural network approach, specifically focusing on an autoencoder with two layers, with additional handling of class imbalance using class weights.






## Project Overview:

The primary objective of this project is to predict whether customers are likely to churn using various deep learning models, evaluate their performance, and select the best-performing model. The performance is measured using F1 Score as the key metric due to the class imbalance problem.
## Key Features:

- Deep Neural Network: Built and fine-tuned multiple DNN models, including an autoencoder model, to predict churn.
- Class Imbalance Handling: Used class weights to tackle the imbalance between the churn and non-churn customer classes.
- Performance Metrics: Evaluated models using various metrics, including accuracy, recall, precision, and F1 score.




## Best Model:

The best-performing model is a 2-layer autoencoder with class weights for handling the class imbalance, achieving the most reliable performance in predicting churn.

### Models Tested

| Model                                        | Train Accuracy | Train Recall | Train Precision | Train F1 Score | Test Accuracy | Test Recall | Test Precision | Test F1 Score |
| :------------------------------------------- | :------------: | :----------: | :-------------: | :------------: | :-----------: | :---------: | :------------: | :-----------: |
| 1 layer model                                | 0.808          | 0.528        | 0.677           | 0.593          | 0.808         | 0.532       | 0.677          | 0.596         |
| 2 layer model - experiment 1                 | 0.800          | 0.588        | 0.633           | 0.610          | 0803          | 0.602       | 0.636          | 0.618         |
| 2 layer model - experiment 2                 | 0.818          | 0.523        | 0.713           | 0.603          | 0.796         | 0.484       | 0.658          | 0.558         |
| 2 layer model with dropout                   | 0.809          | 0.548        | 0.672           | 0.604          | 0.793         | 0.508       | 0.640          | 0.566         |
| 2 layer model with dropout and L2 regularizer| 0.810          | 0.498        | 0.700           | 0.582          | 0.802         | 0.476       | 0.682          | 0.561         |
| 2 layer model with dropout and class weights | 0.731          | 0.850        | 0.496           | 0.626          | 0.731         | 0.837       | 0.496          | 0.623         |
| 2 layer model with dropout and L1 regularizer| 0.691          | 0.882        | 0.457           | 0.602          | 0.689         | 0.896       | 0.456          | 0.605         |
| Autoencoder with 2-layer model               | 0.804          | 0.599        | 0.639           | 0.618          | 0.792         | 0.575       | 0.616          | 0.595         |
| Autoencoder with 2-layer model with class weights | 0.737     | 0.845        | 0.502           | 0.630          | 0.730         | 0.845       | 0.495          | 0.625         |







## Key Dependencies

- `Tensorflow`  for building and training deep neural network models.

- `Imbalanced-learn` for handling class imbalance.


## Future Improvements
- Experiment with other regularization techniques such as  Dropout for further improving model performance.

- Fine-tune hyperparameters for enhanced metrics.
