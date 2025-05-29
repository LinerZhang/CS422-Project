### A Comparative Study and Ensemble of Multiple Models for Imbalanced Multiclass Medical Diagnosis

**Liner Zhang**

#### Abstract
This project focuses on the challenge of imbalanced multi-class classification in medical diagnosis by building and comparing multiple data mining models. Using a cleaned dataset containing 394 samples and 23 symptom-related features, five classification models were constructed: __Decision Tree__, __K-Nearest Neighbors (KNN)__, __Naive Bayes__, __Random Forest__, and __AdaBoost__. To address the issue of class imbalance, oversampling techniques were applied during training.

Experimental results showed that the KNN model outperformed others across most metrics, particularly in accuracy and F1-score. Additionally, a __Stacking ensemble model__ was developed using Logistic Regression as the meta-learner to integrate the five base models. This ensemble approach improved overall prediction stability, although its final performance was still slightly below that of the KNN model.

Future work may explore more advanced ensemble methods, refine feature engineering strategies, or leverage larger and more balanced datasets to enhance diagnostic accuracy and model generalizability.

#### Rationale
__Migraine__ is a common neurological disorder affecting approximately 10% to 15% of the global population, with the prevalence in women being more than three times higher than in men (Lipton et al., 2001). In China, epidemiological studies indicate that there are about 90 million migraine sufferers, over 70% of whom are women (Li et al., 2018). As someone who has been long troubled by migraines, I deeply understand the differences in symptoms and treatment among various migraine types. Accurately and quickly identifying migraine types based on patients’ specific symptoms can greatly improve targeted medication precision, reducing the pain and time wasted on ineffective treatments. Therefore, this project is not only driven by my personal urgent need but also aims to leverage data mining techniques to provide migraine sufferers with a convenient and efficient auxiliary diagnostic tool, achieving truly personalized treatment and improving diagnostic efficiency and patient quality of life.

#### Research Question
This project aims to answer which data mining model performs best in the imbalanced multi-class classification problem of migraine medical diagnosis. Additionally, it explores whether combining multiple models (such as Stacking ensembles) can further improve diagnostic accuracy and stability. The goal is to develop an efficient and reliable __auxiliary diagnostic tool__ to help clinicians or patients quickly and accurately identify different types of migraines, enabling precise treatment and improving patients’ quality of life.

#### Data Sources
This project uses a dataset sourced from the __Kaggle platform__, available at: https://www.kaggle.com/datasets/gzdekzlkaya/migraine-symptom-dataset-for-classification. The dataset contains 400 records and includes 24 migraine symptom features, making it suitable for multi-class medical diagnosis research. 

#### Methodology
This study models the imbalanced multi-class migraine diagnosis problem using various data mining models, including Decision Tree, K-Nearest Neighbors (KNN), Naive Bayes, Random Forest, and AdaBoost classifiers. To tackle class imbalance, oversampling techniques (SMOTE) were applied for data balancing. Finally, model fusion (Stacking) was implemented using Logistic Regression to improve diagnostic accuracy and model stability. Evaluation metrics included __accuracy__, __precision__, __recall__, __F1 score__, and the area under the __ROC curve (AUC)__.

#### Results
Experiments showed that the KNN model performed best across multiple metrics, especially excelling in accuracy and F1 score compared to other individual models. The Stacking ensemble model, by integrating five base models, further improved prediction stability, although its overall performance was slightly lower than KNN. Oversampling techniques effectively alleviated the impact of class imbalance on model performance.

#### Next steps
Future research can explore more types of ensemble methods (such as Boosting variants, Bagging, etc.), optimize the feature engineering process, or collect larger and more balanced datasets to enhance model generalization. Additionally, exploring deep learning models for this task may elevate the intelligence level of diagnosis.

#### Conclusion
This project successfully built a multi-model diagnostic framework, validating the importance of model fusion in improving diagnostic stability. While KNN performed best on the current dataset, the ensemble model offered more robust results. It is recommended to combine multiple model predictions in clinical practice to achieve more precise migraine classification and improve patient treatment outcomes.

### Bibliography 
[1] R. B. Lipton et al., “Prevalence and burden of migraine in the United States: data from the American Migraine Study II,” Headache, vol. 41, no. 7, pp. 646-657, 2001.

[2] X. Li et al., “Epidemiology of migraine in China: A nationwide population-based study,” Journal of Neurology, vol. 265, no. 3, pp. 659-666, 2018.

[3] J. R. Quinlan, “Induction of decision trees,” Machine Learning, vol. 1, no. 1, pp. 81-106, 1986.

[4] T. Cover and P. Hart, “Nearest neighbor pattern classification,” IEEE Transactions on Information Theory, vol. 13, no. 1, pp. 21-27, 1967.

[5] G. H. John and P. Langley, “Estimating continuous distributions in Bayesian classifiers,” Proceedings of the Eleventh Conference on Uncertainty in Artificial Intelligence, pp. 338-345, 1995.

[6] L. Breiman, “Random forests,” Machine Learning, vol. 45, no. 1, pp. 5-32, 2001.

[7] Y. Freund and R. E. Schapire, “A decision-theoretic generalization of on-line learning and an application to boosting,” Journal of Computer and System Sciences, vol. 55, no. 1, pp. 119-139, 1997.

[8] D. H. Wolpert, “Stacked generalization,” Neural Networks, vol. 5, no. 2, pp. 241-259, 1992.

##### Contact and Further Information
For any questions or collaborations related to this project, please contact:

Name: Liner Zhang

Email: Zhangliner0105@hotmail.com
