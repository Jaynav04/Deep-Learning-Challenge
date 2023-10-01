# Deep-Learning-Challenge
Developing a binary classifier that can predict whether applicants will be successful if funded by a non-profit.


## Report
#### Overview:
The aim of this analysis is to identify a machine learning model with the highest level of accuracy for predicting the funding risk of future selected applicants. This prediction is based on historical data gathered from more than 34,000 organizations
#### Results:
- Data Preprocessing
    - I opted to designate the "IS_SUCCESSFUL" column in the dataset as the target variable during the model creation process. In this column, a value of 0 indicates a successful funding outcome for the applicant, while a value of 1 indicates an unsuccessful one.
    - Following the exclusion of the "IS_SUCCESSFUL" column from the original dataset, I employed all the remaining columns as features, with the exception of the two columns detailed below.. 
    - I eliminated two columns from the input data as they appeared unrelated to the desired outcome: "EIN" and "NAME.

- Compiling, Training, and Evaluating the Mode
    - During my initial attempt at constructing a model, I selected six neurons distributed across two hidden layers, employing the ReLu activation function for both layers. This choice was made with the intention of enhancing the processing speed of my model.
    - My initial model did not meet the desired 75% accuracy target; instead, it achieved approximately 72% accuracy on both my test and training datasets, with a loss rate of around 0.55 
    - In my second model iteration, I managed to make slight improvements in accuracy, reaching approximately 73% on both my test and training datasets. This was achieved by introducing an additional layer to my neural network, increasing the node count to 12, and expanding the bins in the "CLASSIFICATION" and "APPLICATION_TYPE" columns within my dataset.

#### Summary:
- In summary, the outcomes of this deep learning model are generally better than average but still fall short of the desired model performance. In future models, I may explore alternative techniques for improvement, such as incorporating different activation functions like Leaky ReLu or Tanh. These changes have the potential to transform input values and, in turn, enhance overall accuracy.