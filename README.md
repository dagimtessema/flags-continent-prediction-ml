#  🎯 Flag continent Prediction with Decision Trees
A machine learning project that predicts the continental location of a given flag using decision tree modeling. The model combines 'Zone', 'Area', 'Population', 'Language',
'Religion', 'Bars', 'Stripes', 'Colors', 'Red', 'Green', 'Blue', 'Gold','White', 'Black', 'Orange', 'Circles', 'Crosses', 'Saltires','Quarters', 'Sunstars', 'Crescent', 
'Triangle', 'Icon', 'Animate','Text' variables to determine flag continental location with Score = 0.692 on test data.

## 📊 Overview
This project demonstrates a complete data science workflow using a University of California Irvine Machine Learning dataset that can be foudn at: https://archive.ics.uci.edu/dataset/40/flags  

      Predicts: Continent of flags 
      Features: 'Zone', 'Area', 'Population', 'Language','Religion', 'Bars', 'Stripes', 'Colors', 'Red', 'Green', 'Blue', 'Gold','White', 'Black', 'Orange', 
                'Circles', 'Crosses', 'Saltires','Quarters', 'Sunstars', 'Crescent', 'Triangle', 'Icon', 'Animate','Text' 
      Model: Decision trees with feature engineering and parameter fine-tuning  
      Performance: Score= 0.692 on test data  
      Dataset: University of California Irvine Machine Learning dataset
   
## 🛠️ Methodology

    Data Loading: Processed CSV file with pandas  
    Feature Engineering: created models with different sets of features to assess prediction power  
    Paramete fine-tuning: used a range of tree depths and corss-validation to determine optimal tree size
    Model Training: decision trees with 25 engineered features
    Evaluation: scores, scatter plots, and loops

## 📈 Key Results

    Training score: 0.968
    Testing score:  0.692
    Best tree depth: 6
    Model Performance: model did fairly well after determining optimal tree depth

## 🧠 Technologies Used

    Python Libraries: pandas, scikit-learn, matplotlib, numpy
    Development Environment: Jupyter Notebook
    Data Format: CSV 
    Version Control: Git 

## 🚀 Getting Started
### Prerequisites

Make sure you have Python and Jupyter Notebook installed:
``` bash
 python --version
jupyter --version
```

### Installation
  1. Clone the repository:
 ``` bash
 git clone https://github.com/dagimtessema/flags-continent-prediction-ml.git
 cd flags-continent-prediction-ml
```
 2. Install required packages:
``` bash
pip install -r requirements.txt
```
 3. Launch Jupyter Notebook:
``` bash
jupyter notebook car-price-prediction-ml.ipynb
```

## 📁 File Structure
├── flags-continent-prediction-ml.ipynb # Main analysis notebook  
├── README.md # Project documentation  
├── requirements.txt # Python dependencies    
└── data/       
&emsp; └── flags.csv   

## 📊 Key Findings  
    Model Limitations: decision trees are intrinsically greedy classifiers and hence we cannot know we have the best categorical splitting. Also, a smaller tree depth could
                       risk underfitting the data when model is applied to other unseen test datasets.

## 🎯 How It Works
The model takes multiple features as input and predicts the expected flag's continental location:

    Input: 'Zone', 'Area', 'Population', 'Language','Religion', 'Bars', 'Stripes', 'Colors', 'Red', 'Green', 'Blue', 'Gold','White', 'Black', 'Orange', 
            'Circles', 'Crosses', 'Saltires','Quarters', 'Sunstars', 'Crescent', 'Triangle', 'Icon', 'Animate','Text' 
    Output: Predicted continental location
    Use Case: could be used as teaching project or in the rare case; to design an apporpriate flag
## 🚧 Future Improvements
    Implement ensemble methods (Random Forest, XGBoost)
    
## 📈 Model Performance
The maximum the score we were are able to achieve was 0.692, which is better than a random guess, that would have an accuracy of 1/6.
