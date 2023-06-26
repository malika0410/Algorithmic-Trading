# Algorithmic-Trading

## Machine Learning Trading Bot
In this Challenge, you’ll assume the role of a financial advisor at one of the top five financial advisory firms in the world. Your firm constantly competes with the other major firms to manage and automatically trade assets in a highly dynamic environment. In recent years, your firm has heavily profited by using computer algorithms that can buy and sell faster than human traders.

The speed of these transactions gave your firm a competitive advantage early on. But, people still need to specifically program these systems, which limits their ability to adapt to new data. You’re thus planning to improve the existing algorithmic trading systems and maintain the firm’s competitive advantage in the market. To do so, you’ll enhance the existing trading signals with machine learning algorithms that can adapt to new data.

## Instructions:
Use the starter code file to complete the steps that the instructions outline. The steps for this Challenge are divided into the following sections:

- Establish a Baseline Performance

- Tune the Baseline Trading Algorithm

- Evaluate a New Machine Learning Classifier

- Create an Evaluation Report

## Technologies
In this challenge, you’ll use Jupyter Lab and the following python version 3.8.5 libraries:

- pandas
- Numpy
- hvPlot
- [Matplotlib]https://matplotlib.org/)
- scikit-learn
   - scikit metrics
   - imbalanced-learn
   - linear model 
   - train test split
   - Standard Scaler
   - OneHotEncoder

## Installation Guide
### To check that scikit-learn and hvPlot are installed in your Conda dev environment, complete the following steps:
### 1. Activate your Conda dev environment (if it isn’t already) by running the following in your terminal:
`conda activate dev`

### 2. When the environment is active, run the following in your terminal to check if the scikit-learn, itensorflow and keras libraries are installed on your machine:
`conda list scikit-learn`

### If you see scikit-learn, itensorflow and keras listed in the terminal, you’re all set!
### 1. Install scikit-learn
`pip install -U scikit-learn`

## Usage
To use this application, simply clone the repository and open jupyter lab from git bash by running the following command:

`jupyter lab`

## After tuning the data 
- Here I have tune the training algorithm by adjusting the size of the training dataset as 6 months instead of 3 months. Compared it with the original 3 month dataset
 ![image](https://github.com/malika0410/Algorithmic-Trading/blob/main/images/6month.PNG)

- Also I have tune the trading algorithm by adjusting the SMA input features.Short window = 50 and long window = 200
  ![image](https://github.com/malika0410/Algorithmic-Trading/blob/main/images/window50_200.PNG)
 

- Finally compared the cumpulative reutn plot of trading algorithm before and after tuning the dataset.
  Actual returns versus Strategy returns
 ![image](https://github.com/malika0410/Algorithmic-Trading/blob/main/images/returns.png)
 ![image](https://github.com/malika0410/Algorithmic-Trading/blob/main/images/6monthsreturn.PNG)




## Questions to Answer -
1) What impact resulted from increasing or decreasing the training window?
Ans. Notice that our SVM model when the traing window was 3 month performed well from the end of 2017 period until early in 2019. That’s when the actual and predicted returns start to greatly differ.When the training window changed to 6 months there is no significant change can be seen just a slight differ in 6 month data after 2020.

2) What impact resulted from increasing or decreasing either or both of the SMA windows?
Ans. When the training window set to period 50 and 200 there is a drastically increase or decrease in returns. Model did not perform well and actual return and strategy returns are different.

![image](https://github.com/malika0410/Algorithmic-Trading/blob/main/images/window.PNG)






