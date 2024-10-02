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
</ul>
