**Deep Learning Model Report for Alphabet Soup**

### **Overview of the Analysis**
The purpose of this analysis is to develop and evaluate a deep learning model to predict the success of charity funding applicants for the Alphabet Soup foundation. By leveraging a dataset containing applicant information and funding outcomes, the model aims to identify patterns that determine successful funding applications. This can help the foundation allocate resources more effectively.

---

### **Results**

#### **Data Preprocessing**

The target variable for the model is `IS_SUCCESSFUL`, which indicates whether a charity application was successful. The features used in the model include variables like Application Type, Affiliation, Classification, Use Case, Organization, Income Amount, Special Considerations, Ask Amount, and other relevant encoded categorical variables. Variables such as `EIN` and `NAME` were removed from the input data because they are identifiers or complex strings that don't help the model predict outcomes effectively.

#### **Compiling, Training, and Evaluating the Model**

The first neural network model included two hidden layers with 8 neurons in the first layer and 5 neurons in the second layer. The ReLU activation function was used for the hidden layers, and the sigmoid activation function was applied to the output layer for binary classification. These choices were made to keep the model simple but effective. The initial model achieved an accuracy of 73%, which was below the desired performance target, which is 75%. I  tried adjusting the number of neurons and experimenting with additional hidden layers, but all 3 attempts failed and would not go any higher than 73%.

---

### **Summary**

The deep learning model for Alphabet Soup showed moderate performance with an accuracy of 73%. While this is a good start, it didn’t meet the desired accuracy for predicting successful charity applications. To improve the model, beginners could try simple adjustments like adding or removing features to see if the model performs better. They could also test a few different models, like logistic regression, which could be easier to understand and work well for classification. Cleaning up the data, such as making sure there are no missing values and standardizing numeric features, might also help. Finally, splitting the data into training and testing sets more carefully could give better insights into the model’s performance.
