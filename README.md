# Neural_Network_Charity_Analysis

## Overview of Project
Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

I am going to exercise my knowledge of machine learning and neural networks by using features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.


## Results

### Data Preprocessing
- What variable(s) are considered the target(s) for your model?  
  The 'IS_SUCCESSFUL' column is the variable that is targeted for my model. 
  
- What variable(s) are considered to be the features for your model?  
  ![image](https://user-images.githubusercontent.com/86776606/199859460-52b2f7ef-b9eb-412c-9de2-181c060b9d57.png)  
  All of the variables listed in the picture above are the variables being considered formy model.
  
- What variable(s) are neither targets nor features, and should be removed from the input data?  
 ![image](https://user-images.githubusercontent.com/86776606/199859293-2ce19776-23f6-4155-88f8-adce7f0c4725.png)  
  'EIN' and 'NAME' are the variables that are removed from the input data.

### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?  
![image](https://user-images.githubusercontent.com/86776606/199859862-9b6ef2cd-8ce4-4574-b32c-82947829d389.png)  
  There is a total of three hidden layers in my neural network model. The first layer has 100 neurons, the second has 30, and the third has 10. The first layer uses the ReLU activation function and the other two layers use the Sigmoid activation function. ReLU was used for the first layer in order to create simple and efficient training of my model. Sigmoid was used for the other two layers to help produce non-linear boundaries and provide a greater sense of accuracy.
  
- Were you able to achieve the target model performance?  
  ![image](https://user-images.githubusercontent.com/86776606/199861855-2a0560a5-5bfa-41af-b36d-7b1428cebeee.png)  
  Yes. My model was able to achieve a model accuracy of 78% which is 3% over the target model.
  
- What steps did you take to try and increase model performance?  
  I included the 'NAME' column by converting the column into a set of data points to be included in the model. This provided a substantial bump in efficiency. I also added the third hidden layer with the sigmoid activation function. My model was also ran through the RandomForestClassifer which helped with improving predictive accuracy.  

## Summary
The model achieved an accuracy of 78% which is 3% over the target model. The ability to create more viable data points is crucial in being able to achieve the highest predictive accuracy possible. The RandomForestClassifer would be recommended in helping solve classification problems. It is an excellent algorithm typically used for classification, regression, and other tasks.
