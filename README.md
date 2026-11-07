# CDC Diabetes Health indicators
Problem Statement
To identify if a person has diabetes or pre-diabetic/healthy


Dataset Description
The Diabetes Health Indicators Dataset contains healthcare statistics and lifestyle survey information about people in general along with their diagnosis of   diabetes.The target variable for classification is whether a patient has diabetes, is pre-diabetic, or healthy.

Dataset Characteristics
Tabular, Multivariate

Subject Area
Health and Medicine

Associated Tasks
Classification

Feature Type
Categorical, Integer

No of Features: 21
No of Instances: 10000

GitHub Link: https://github.com/sriramvuser79-gittest/mltest/blob/main/

Models Used

| ML Algorithm           │   Accuracy │   AUC Score │   Precision │    Recall │   F1 Score │      MCC │

│ Logistic Regression    │   0.835667 │    0.803649 │    0.472727 │ 0.161157  │   0.24037  │ 0.20423  │

│ Decision Tree          │   0.763    │    0.600062 │    0.302609 │ 0.359504  │   0.328612 │ 0.18702  │

│ KNN                    │   0.830667 │    0.703062 │    0.45     │ 0.22314   │   0.298343 │ 0.231415 │

│ Naive Bayes            │   0.750667 │    0.768603 │    0.335821 │ 0.557851  │   0.419255 │ 0.287025 │

│ Support Vector Machine │   0.840333 │    0.712232 │    0.52809  │ 0.0971074 │   0.164049 │ 0.174339 │

Observations on Model Performance

|ML Model Name          | Observation about Model performance                                                                                                  |

| Logistic Regression   | Logistic Regression achieves the highest AUC score (0.803) across all models, meaning its internal probability scores rank diabetic  |  |                       | patients very well relative to non-diabetic patients. Recall value is lower resulting in missing more cases.                         |

| Decision Tree         | Decision Tree has lowest AUC score (0.600) and weak F1 score (0.328) indicating high variance and overfitting on the diabetic class. |

| KNN                   | KNN achieves moderate precision (45.0%) and a decent MCC (0.231), but its recall (22.3%) is still far too low for reliable diagnostic|                          | use.                                                                                                                                 |
| Naive Bayes           | Naive Bayes achieves the highest Recall (55.7%), the highest F1 Score (0.419), and the highest MCC (0.287). Naive Bayes catches over |  |                       | half of the actual diabetic patients—more than double the rate of any other model tested.                                            |

| Support Vector Machine| SVM detects less than 10% of true diabetic cases (Recall = 9.7%) .. Have high accuracy but this is misleading.SVM predicts more      |  |                       | non-diabetic making them unsafe for clinical trials.                                                                                 |

| Overall Winner for the| Despite having the lowest raw accuracy (75.1%), Naive Bayes is clearly the most effective baseline model for diabetes detection. It  |  | dataset               | achieves the highest Recall (55.8%), the highest F1 Score (0.419), and the highest MCC (0.287).                                      |
|                       | Medical Takeaway: Naive Bayes catches over half of the actual diabetic patients—more than double the rate of any other model tested. |

              
