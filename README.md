# AY22/23 SEM1 CS3244 Project Title: Human Activity Recognition

## Project Description

Every year, an estimated 684,000 deaths occur globally due to [falls](https://www.who.int/news-room/fact-sheets/detail/falls). Hence, the motivation behind this project is to detect falls through postural changes.

Our approach to this problem is to focus on detecting 2 postural changes, **SIT_TO_LIE** and **STAND_TO_LIE**, as accurately as possible. We want to maximize accuracy and **minimize False Negatives** for both classes.

Machine Learning Techniques used:
1. Exploratory Data Analysis
2. Feature Engineering
3. Support Vector Machine
4. Logistic Regression
5. Decision Tree Classifier
6. Random Forest Classifiers
7. Artificial Neural Networks (ANN)
8. Long short-term Memory (LSTM)
9. Convolutional Neural Network (CNN)
10. Convolutional-LSTM Neural Netowrk (CNNLSTM)

## Evaluation of Models
| **Models** | **Accuracy** | **Recall** | **Precision** | **F1** |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| SVM | 95.0%  | 88.0%  | 88.0%  | 88.0%  |
| Logistic Regression | 94.0%  | 83.0%  | 87.0%  | 85.0%  |
| RFC | 92.0%  | 82.0%  | 82.0%  | 83.0%  |
| ANN | 90.0% | 79.0%  | 82.0%  | 80.0% |
| CNN | 88.0% | 79.0%  | 81.0%  | 79.0% |
| RNN | 81.0% | 75.0%  | 78.0%  | 76.0% |
| CNNLSTM | 91.4% | 91.2% | 92.0% | 91.0% |

## Final CNNLSTM Model Architecture
![Screenshot 2022-12-05 225923](https://user-images.githubusercontent.com/101163864/205669061-4d0fd0ee-11fd-43a4-877f-908cff5c6020.png)

## Final Model
We **did not** choose the SVM or Logistic Regression model as the best classifiers because they were trained on features that have been engineered (using their statistics eg: mean, standard deviation, interquartile range etc.), which meant that the performance was **very specific to this particular experimental setting**. To generalize to a more practical use case, we relied on the raw signals. Hence, the CNNLSTM model was the best performing model on raw signals. However, although it was the best performing, it had a **higher False Negative rate**. Therefore, more work has to be done on this model for this specific problem setting. Nevertheless, it is still **effective and competent** in detecting human activities in general and can be used for other applications.

## Team Contributers
1. [Choo Wei Jie, Darren](https://github.com/dchoo99)
2. [Han Jiaxu](https://github.com/itsmejx)
3. Daryl Ang
4. Sarah Tan
5. Teo Zhi Hao
6. Kelvin Foo

## Mentor
Tian Fang

## Referenced Work:
1. 
2.
3.
4.
5.
6.
7.
8.
9.
10.
