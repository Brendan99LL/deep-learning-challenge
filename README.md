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

_**Step 3: Optimize the Model**_
<p>Using your knowledge of TensorFlow, optimize your model to achieve a target predictive accuracy higher than 75%.</p>
<p>Use any or all of the following methods to optimize your model:</p>
<ul>
  <li>Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:</li>
  <ul>
    <li>Dropping more or fewer columns.</li>
    <li>Creating more bins for rare occurrences in columns.</li>
    <li>Increasing or decreasing the number of values for each bin.</li>
    <li>Add more neurons to a hidden layer.</li>
    <li>Add more hidden layers.</li>
    <li>Use different activation functions for the hidden layers.</li>
    <li>Add or reduce the number of epochs to the training regimen.</li>
  </ul>
</ul>
<p>Note: If you make at least three attempts at optimizing your model, you will not lose points if your model does not achieve target performance.</p>
<ol>
  <li>Create a new Google Colab file and name it AlphabetSoupCharity_Optimization.ipynb.</li>
  <li>Import your dependencies and read in the charity_data.csv to a Pandas DataFrame.</li>
  <li>Preprocess the dataset as you did in Step 1. Be sure to adjust for any modifications that came out of optimizing the model.</li>
  <li>Design a neural network model, and be sure to adjust for modifications that will optimize the model to achieve higher than 75% accuracy.</li>
  <li>Save and export your results to an HDF5 file. Name the file AlphabetSoupCharity_Optimization.h5.</li>
</ol>

_**Step 4: Write a Report on the Neural Network Model**_
<p>For this part of the assignment, you’ll write a report on the performance of the deep learning model you created for Alphabet Soup.</p>
<p>The report should contain the following:</p>
<ol>
  <li>Overview of the analysis: Explain the purpose of this analysis.</li>
  <li>Results: Using bulleted lists and images to support your answers, address the following questions:</li>
    <ul>
      <li>Data Processing</li>
        <ul>
          <li>What variable(s) are the target(s) for your model?</li>
          <li>What variable(s) are the features for your model?</li>
          <li>What variable(s) should be removed from the input data because they are neither targets nor features?</li>
        </ul>
      <li>Compiling, Training, and Evaluating the Model</li>
        <ul>
          <li>How many neurons, layers, and activation functions did you select for your neural network model, and why?</li>
          <li>Were you able to achieve the target model performance?</li>
          <li>What steps did you take in your attempts to increase model performance?</li>
        </ul>
    </ul>
  <li>Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.</li>
</ol>

_**Step 5: Copy Files Into Your Repository**_
<p>Now that you're finished with your analysis in Google Colab, you need to get your files into your repository for final submission.</p>
<ol>
  <li>Download your Colab notebooks to your computer.</li>
  <li>Move them into your Deep Learning Challenge directory in your local repository.</li>
  <li>Push the added files to GitHub.</li>
</ol>


