<h1>Neural Network Model Report</h1>

<h3>Optimization Attempts Summaries:</h3>
<ol>
  <li>Optimization Attempt # 1</li>
    <ul>
      <li>Activation Functions: Relu, Sigmoid, Relu, Sigmoid (output)</li>
      <li>Hidden Layer Units: 10, 9, 8, 1</li>
      <li>Epochs = 100</li>
      <li>Accuracy: 73.03%</li>
    </ul>
  <li>Optimization Attempt # 2</li>
    <ul>
      <li>Activation Functions: Relu, Sigmoid, Elu, Sigmoid (output)</li>
      <li>Hidden Layer Units: 20, 19, 18, 1</li>
      <li>Epochs = 100</li>
      <li>Accuracy: 72.93%</li>
    </ul>
  <li>Optimization Attempt # 3</li>
    <ul>
      <li>Activation Functions: Relu, Relu, Relu, Sigmoid (output)</li>
      <li>Hidden Layer Units: 80, 50, 25, 1</li>
      <li>Epochs = 100</li>
      <li>Accuracy: 73.20%</li>
    </ul>
  <li>Optimization Attempt # 4</li>
    <ul>
      <li>Activation Functions: Relu, Relu, Sigmoid (output)</li>
      <li>Hidden Layer Units: 10, 8, 1</li>
      <li>Epochs = 100</li>
      <li>Accuracy: 72.58%</li>
    </ul>
  <li>Optimization Attempt # 5</li>
    <ul>
      <li>Activation Functions: Relu, Sigmoid, Sigmoid (output)</li>
      <li>Hidden Layer Units: 16, 16, 1</li>
      <li>Epochs = 50</li>
      <li>Accuracy: 72.79%</li>
    </ul>
  <li>Optimization Attempt # 6</li>
    <ul>
      <li>Activation Functions: Relu, Relu, Sigmoid (output)</li>
      <li>Hidden Layer Units: 16, 16, 1</li>
      <li>Epochs = 50</li>
      <li>Accuracy: 72.47%</li>
    </ul>
  <li>Optimization Attempt # 7</li>
    <ul>
      <li>Activation Functions: Relu, Elu, Sigmoid (output)</li>
      <li>Hidden Layer Units: 16, 16, 1</li>
      <li>Epochs = 50</li>
      <li>Accuracy: 72.93%</li>
    </ul>
  <li>Optimization Attempt # 8</li>
    <ul>
      <li>Activation Functions: Relu, Relu, Elu, Sigmoid (output)</li>
      <li>Hidden Layer Units: 16, 16, 16, 1</li>
      <li>Epochs = 50</li>
      <li>Accuracy: 72.93%</li>
    </ul>
  <li>Optimization Attempt # 9</li>
    <ul>
      <li>Activation Functions: Relu, Relu, Relu, Sigmoid (output)</li>
      <li>Hidden Layer Units: 16, 16, 16, 1</li>
      <li>Epochs = 50</li>
      <li>Accuracy: 73.16%</li>
    </ul>
  <li>Optimization Attempt # 10</li>
    <ul>
      <li>Activation Functions: Relu, Sigmoid, Elu, Sigmoid (output)</li>
      <li>Hidden Layer Units: 16, 16, 16, 1</li>
      <li>Epochs = 50</li>
      <li>Accuracy: 73.04%</li>
    </ul>  
</ol>

<h3>Results</h3>
<ul>
  <li>Data Processing</li>
    <ul>
      <li>What variable(s) are the target(s) for your model?</li>
      <p>The variable target of the model is the "IS_SUCCESSFUL" column originally from the application_df.</p>
      <li>What variable(s) are the features for your model?</li>
      <p>The features of the model are the columns within application_df, except for the "IS_SUCCESSFUL" column.</p>
      <li>What variable(s) should be removed from the input data because they are neither targets nor features?</li>
      <p>The "EIN" and "Name" variables were removed from application_df because they are neither targets nor features to be used in the model.</p>
    </ul>
  <li>Compiling, Training, and Evaluating the Model</li>
    <ul>
      <li>How many neurons, layers, and activation functions did you select for your neural network model, and why?</li>
      <p>The amount of neurons, layers, and activiation functions varied throughout the ten attempts made to create a target model performance of at least 75%. 
 The maximum number of hidden layer units used through the attempts was three units, excluding the one output layer that is included in each model, and that is in attempts to have the model run effectively.  I started with 3 neuron layers to start the attempts to create a high optimization of the model, but I decreased it to 2 neurons to see the difference.  During my last few attempts, I went back to 3 neurons in hopes of giving the model potentially more clear outputs.  The actvation functions that were kept on rotation included Sigmoid, Relu, and Elu.  The point of switching between these activiation functions and the various amount of neurons in each model, was to potentially create a regression model that creates a high output value.  During the many attempts, the Sigmoid activation function was kept as the output, and the input layers would keep the Relu functions.  The Relu finction was kept in the attempts as it has the faster learning and simplified output compared to the other functions.  The amount of epochs did not exceed 100 since the model ran for about 3-4 minutes each time.  I switched to 50 epochs for my later attempts in hoping that the model would output values that would exceed 75% during this beginning half of the run.</p>
      <li>Were you able to achieve the target model performance?</li>
      <p>Unfortunately, with all the changes in the neural network model, the results were not able to acheive the target model performance.  The various edits to the model were meant to create an accurancy value of at least 75%, however the highest accuracy point the model attempts were able to acheive is 73.20%.</p>
      <li>What steps did you take in your attempts to increase model performance?</li>
      <p>There is not a clear way to know how the various number of neurons and activation functions, unless advanced mathematics is involved.  Throughout the attempts the number of layers and neurons would change to experiment if a higher or lower amount of units would lead to a higher accuracy value.  In theory, the attempts that had more units should have been able to examine more patterns within the data.  The Relu activation function was kept as the initial layer due to its faster learning and simplified output.  The middle layers were a trial and error of functions to see what would yield the optimal accuracy.  The output layer consistently stayed as the output layer since I thought it would help predict the probabilities.  When choosing the epochs, this was based on the change of accuracy as each epoch was run and how well my device was able to run them.  With 100 epochs, it took 3-4min to run all of them, and the accuracy still never reached 75%.  Even when decreasing the epochs to 50, the accuracy values never reached above 75%.  In this case, the epochs later became determined on how my device was able to run them since there was not much of a change in values and loss.</p>
    </ul>
</ul>

<h3>Summary</h3>
<p>The initial neural network model created an accuracy value of about 72.78%, and the optimization attempts were not successful in creating a value of greater than 75%.  My ten attempts to optimze the model were not able to perform effectively enough to create an accuacy value of 75% or greater.  Since the initial model is considered unsuccesful, my optimization models may fall in the same category since no attempt was able to go over 74%, however none of them went below the 72% mark.  In theory, maintaining the initial activation function as Relu and the output layer as Sigmoid should yeild optimal results, however attempts to change all the activation functions for all the layers may be the next step.  It can be argued that the models were successful in keeping a consistent accuracy value as within all the attempts the accuracy level never fell below 72% and never went above 74%.</p>


