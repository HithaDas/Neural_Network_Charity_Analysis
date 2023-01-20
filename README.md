# Neural_Network_Charity_Analysis
Module 20 Challenge 

# Background
Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

# Module Deliverable
Deliverable 1: Preprocessing Data for a Neural Network Model
Deliverable 2: Compile, Train, and Evaluate the Model
Deliverable 3: Optimize the Model
Deliverable 4: A Written Report on the Neural Network Model (README.md)

Purpose
A foundation, Alphabet Soup, wants to predict where to make investments. The goal is to use machine learning and neural networks to apply features on a provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. The initial file has 34,000 organizations and a number of columns that capture metadata about each organization from past successful fundings.

# Results

- What variable(s) are considered the target(s) for your model?
Checking to see if the target is marked as successful in the DataFrame, indicating that it has been successfully funded by AlphabetSoup.

- What variable(s) are considered to be the features for your model?
The IS_SUCCESSFUL column is the feature chosen for this dataset.

- What variable(s) are neither targets nor features, and should be removed from the input data?
The EIN and NAME columns will not increase the accuracy of the model and can be removed to improve code efficiency.

Compile, Train, and Evaluate the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
In the optimized model, layer 1 started with 120 neurons with a relu activation. For layer 2, it dropped to 80 neurons and continued with the relu activation. The sigmoid activation seemed to be the better fit for layers 3 (40 neurons) and layer 4 (20 neurons).

<img width="929" alt="Screen Shot 2023-01-19 at 9 41 46 PM" src="https://user-images.githubusercontent.com/110873947/213612922-621863ba-a276-47cf-b76f-e6cbd8aaf452.png">



- Were you able to achieve the target model performance?
The target for the model was 75%, but the best the model could produce was 46.68%.

<img width="687" alt="Screen Shot 2023-01-19 at 9 46 21 PM" src="https://user-images.githubusercontent.com/110873947/213613377-569e631d-7432-4b75-8d54-728e3bcad712.png">

- What steps did you take to try and increase model performance?
The STATUS and SPECIAL_CONSIDERATIONS columns were dropped as well as increasing the number of neurons and layers.

# Summary 
The original code yielded 71.69% accuracy whereas the optimization yielded lower accuracy of 46.68%. To investigate the accuracy further, we should try random forest classifier.

