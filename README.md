# deep-learning-challenge
Module 21 Challenge

# Background
Alphabet Soup, a non-profit foundation, is seeking a tool that can facilitate the selection of the most promising applicants for funding, thereby ensuring the highest probability of success in their ventures. The organization intends to utilize machine learning and neural networks in the provided dataset to create a binary classifier to achieve this. The classifier will be used to predict whether applicants will achieve success if funded by Alphabet Soup. The proposed analysis aims to optimize the process of selecting funding recipients through advanced computing methodologies.

# Results
- Data Preprocessing:
  - The target variable to determine the effectiveness of the funds disbursed is "IS_SUCCESSFUL". This variable reflects whether the financial aid has been utilized efficiently or not.
  - The following variables are classified as feature variables: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
  - EIN and NAME were removed because they are neither targets nor features.
 
- Compiling, Training, and Evaluating the Model:
  - According to [`AlphabetSoupCharity.ipynb`](https://github.com/lakigit/deep-learning-challenge/blob/main/Starter_Code/AlphabetSoupCharity.ipynb)
    - The number of input features is directly proportional to the length of X_train. The model architecture comprises two hidden layers with 80 and 30 neurons, respectively. The rectified linear unit (ReLU) activation function is employed for both hidden layers, while the sigmoid activation function is used for the output layer.
![image](https://github.com/lakigit/deep-learning-challenge/assets/138610916/034b0566-39f2-4a26-ac00-76a27e469365)
    - Evaluate the model using the test data
      
      `268/268 - 0s - loss: 0.5553 - accuracy: 0.7245 - 466ms/epoch - 2ms/step`\
      `Loss: 0.5552864670753479, Accuracy: 0.7245481014251709`

      1. **Epochs and Timing**:
        - It looks like the training process involves 268 epochs.
        - The training time for each epoch is 466 milliseconds, and the time taken for each step (or batch) is 2 milliseconds.

      2. **Model Performance**:
        - The loss after training is 0.5553.
        - The accuracy achieved on the dataset is 72.45%.
      
      3. **Conclusion**:
        - The model's accuracy is approximately 72.45%, suggesting that it correctly predicted the target outcome for about 72.45% of the instances in the dataset.
        - The loss value (0.5553) is a measure of how well the model is performing, with lower values indicating better performance. This loss value is used to optimize the model during training.
     
  - According to [`AlphabetSoupCharity_Optimisation.ipynb`](https://github.com/lakigit/deep-learning-challenge/blob/main/Starter_Code/AlphabetSoupCharity_Optimisation.ipynb)
