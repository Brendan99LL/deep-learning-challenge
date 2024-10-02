# deep-learning-challenge
<p>Columbia University Bootcamp Module 21 Challenge</p>
<p>Alphabet Soup Charity</p>

**Background**
<p>The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.</p>
<p>From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:
<ul>
  <li>EIN and NAME—Identification columns</li>
  <li>APPLICATION_TYPE—Alphabet Soup application type</li>
  <li>AFFILIATION—Affiliated sector of industry</li>
  <li>CLASSIFICATION—Government organization classification</li>
  <li>USE_CASE—Use case for funding</li>
  <li>ORGANIZATION—Organization type</li>
  <li>STATUS—Active status</li>
  <li>INCOME_AMT—Income classification</li>
  <li>SPECIAL_CONSIDERATIONS—Special considerations for application</li>
  <li>ASK_AMT—Funding amount requested</li>
  <li>IS_SUCCESSFUL—Was the money used effectively</li>
</ul>
</p>

**Instructions**

_**Step 1: Preprocess the Data**_
<p>Using your knowledge of Pandas and scikit-learn’s StandardScaler(), you’ll need to preprocess the dataset. This step prepares you for Step 2, where you'll compile, train, and evaluate the neural network model.</p>
<p>Start by uploading the starter file to Google Colab, then using the information we provided in the Challenge files, follow the instructions to complete the preprocessing steps.</p>
<ol>
  <li>Read in the charity_data.csv to a Pandas DataFrame, and be sure to identify the following in your dataset:</li>
  <ul>
    <li>What variable(s) are the target(s) for your model?</li>
    <li>What variable(s) are the feature(s) for your model?</li>
  </ul>
  <li>Drop the EIN and NAME columns.</li>
  <li>Determine the number of unique values for each column.</li>
  <li>For columns that have more than 10 unique values, determine the number of data points for each unique value.</li>
  <li>Use the number of data points for each unique value to pick a cutoff point to combine "rare" categorical variables together in a new value, Other, and then check if the replacement was successful.</li>
  <li>Use pd.get_dummies() to encode categorical variables.</li>
  <li>Split the preprocessed data into a features array, X, and a target array, y. Use these arrays and the train_test_split function to split the data into training and testing datasets.</li>
  <li>Scale the training and testing features datasets by creating a StandardScaler instance, fitting it to the training data, then using the transform function.</li>
</ol>

_**Step 2: Compile, Train, and Evaluate the Model**_
<p>Using your knowledge of TensorFlow, you’ll design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup-funded organization will be successful based on the features in the dataset. You’ll need to think about how many inputs there are before determining the number of neurons and layers in your model. Once you’ve completed that step, you’ll compile, train, and evaluate your binary classification model to calculate the model’s loss and accuracy.</p>
<ol>
  <li>Continue using the file in Google Colab in which you performed the preprocessing steps from Step 1.</li>
  <li>Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.</li>
  <li>Create the first hidden layer and choose an appropriate activation function.</li>
  <li>If necessary, add a second hidden layer with an appropriate activation function.</li>
  <li>Create an output layer with an appropriate activation function.</li>
  <li>Check the structure of the model.</li>
  <li>Compile and train the model.</li>
  <li>Create a callback that saves the model's weights every five epochs.</li>
  <li>Evaluate the model using the test data to determine the loss and accuracy.</li>
  <li>Save and export your results to an HDF5 file. Name the file AlphabetSoupCharity.h5.</li>
</ol>
