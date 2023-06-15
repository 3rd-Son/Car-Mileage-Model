<!DOCTYPE html>
<html>
<head>
 
</head>
<body>
  <h1>Auto-Mpg Linear Regression Model</h1>
  
  <h2>Introduction</h2>
  <p>
    This repository contains the code and data for a linear regression model that predicts the miles per gallon (mpg) of a car based on various features.
  </p>
  
  <h2>Data</h2>
  <p>
    The dataset used for training and evaluating the model is the <a href="https://archive.ics.uci.edu/ml/datasets/auto+mpg" target="_blank" rel="noopener noreferrer">Auto-Mpg Dataset</a> from the UCI Machine Learning Repository. It consists of 398 instances with 9 attributes, including the target attribute (mpg). The dataset contains both continuous and discrete features such as cylinders, displacement, horsepower, weight, acceleration, model year, origin, and car name. You find the data at <a href="https://www.kaggle.com/datasets/uciml/autompg-dataset">MPG-Dataset</a>

  </p>
  
  <h2>Exploratory Data Analysis (EDA)</h2>
  <p>
    Prior to building the model, an Exploratory Data Analysis (EDA) was performed on the dataset to gain insights and understand the relationships between the features and the target variable. Various visualizations and statistical analyses were conducted to identify patterns, correlations, and potential outliers in the data. See <a href="https://github.com/Vic3sax/Car-Mileage-Model/blob/main/notebooks/visualization.ipynb">EDA</a> for the Exploratory Data Analysis.
  </p>
  
  <h2>Model Training</h2>
  <p>
    The linear regression model was built using the scikit-learn library in Python. The features were preprocessed, including handling missing values in the "horsepower" attribute. The dataset was split into training and testing sets to evaluate the model's performance. Feature scaling and any necessary feature transformations were applied. <a href="https://github.com/Vic3sax/Car-Mileage-Model/blob/main/models/model.ipynb">Model.py</a> 
  </p>
  
  <h2>Model Evaluation</h2>
  <p>
    The trained linear regression model was evaluated using various performance metrics such as mean squared error (MSE), mean absolute error (MAE), and R-squared (coefficient of determination). The model's performance on the test set was assessed to measure its accuracy in predicting the miles per gallon of cars.
  </p>
  
  <h2>Usage</h2>
  <p>
    To use this model, follow the steps below:
    <ol>
      <li>Clone the repository: <code>git clone https://github.com/Vic3sax/Car-Mileage-Model.git</code></li>
      <li>Navigate to the project directory: <code>cd Car-Mileage-Model
</code></li>
      <li>Install the required dependencies: <code>pip install -r requirements.txt</code></li>
      <li>Run the prediction script: <code>python predict_mpg.py</code></li>
    </ol>
  </p>
  
  <h2>Contributing</h2>
  <p>
    Contributions to this project are welcome. If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.
  </p>
  
  <h2>License</h2>
  <p>
    This project is licensed under the MIT License. See the <a href="LICENSE" target="_blank" rel="noopener noreferrer">LICENSE</a> file for more details.
  </p>
  
  <h2>Acknowledgements</h2>
  <p>
    The Auto-Mpg Dataset used in this project is available from the UCI Machine Learning Repository. Special thanks to the original contributors and maintainers of the dataset.
  </p>
</body>
</html>

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
