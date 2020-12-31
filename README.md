# Drug's Mechanism of action prediction
Predicting the mechanism of action of drugs using gene expression and cell viability data from a publicly available dataset (https://www.kaggle.com/c/lish-moa).

# CS50 final project - Drug's Mechanism of action prediction
## In short
Predicting the mechanism of action of drugs using gene expression and cell viability data from a [publicly available dataset](https://www.kaggle.com/c/lish-moa).

## Personal background and knowledge used
My name is Simona Kolarova, I am recent PhD graduate from King's College London and my area of expertise is physical chemistry. For this project, I drew upon my understanding of chemical and biological data and my newly developed passion for data analysis and machine learning. I utilised much of the understanding developed troughout CS50 (specifically, my knowledge of Python, HTML and CSS, data structures and algorithms) and some of the techniques I learned during completion of the CS50 AI course (e.g., neural networks). 

## Project background and aim
Understanding the mechanism of action (MoA) of drug candidates is becoming increasingly important in the process of drug discovery. To determine the MoA of newly-developed therapeutics, cell-based assays that measure gene expression and cell viability upon drug exposure are commonly employed in combination with large databases of known drug/cellular responses/MoA correlations. Predicting the MoA of drug candidates from such data requires robust data analysis and machine learning approaches.

In search of such approaches, the Laboratory for Innovation Science at Harvard (LISH), Connectivity Map (a project within the Broad Institute of MIT and Harvard) and the NIH Common Funds Library of Integrated Network-Based Cellular Signatures (LINCS) recently made a [large multi-label dataset of cellular responses and MoA](https://www.kaggle.com/c/lish-moa) publicly available.

To contribute to this important task, I explored and visualised important aspects of the provided dataset, constructed a neural network model in Python and described my project in detail in an HTML file.

## Repositories
- [Project github repository (data exploration)](https://github.com/SimonaKolarova/Drug-s-Mechanism-of-action)
- [Kaggle repository (machine learning)](https://www.kaggle.com/simonakolarova/moa-predictions)
- [Kaggle repository (features importance)](https://www.kaggle.com/simonakolarova/moa-feature-importance)
- [HTML interactive project description](https://simonakolarova.github.io/mechanism_of_action.html) - please let page fully load before examining

## Dataset - understanding and visualisation
First, I focused on understanding the different features (i.e., experimental conditions, gene expressions, cell viabilities) and the target (i.e., mechanisms of action) in the dataset. For the purpose I visualised their distributions and calculated their cross-correlations in this [Jupiter Notebook](https://github.com/SimonaKolarova/Drug-s-Mechanism-of-action/blob/main/Data%20-%20understanding%20and%20visualisation.ipynb). More information is available in the [HTML project description ('Dataset - understanding and cisualtisation' section)](https://simonakolarova.github.io/mechanism_of_action.html#item-2).

## Exploratory data analysis
Next, I examined the relationships between the different features (e.g., whether experimental conditions affect the gene expression and cell viability distributions) and the relationships between the features and the targets (e.g., whether increased loss of cell viability is correlated with a drug having multiple mechanisms of action). 
Again, I compiled a [Jupiter Notebook](https://github.com/SimonaKolarova/Drug-s-Mechanism-of-action/blob/main/Exploratory%20data%20analysis.ipynb) of all the data handling and visualisation and have provided much more information about the observed relationships in the [HTML project description ('Exploratory data analysis')](https://simonakolarova.github.io/mechanism_of_action.html#item-3).

## Principal component analysis
As relatively high cross-correlations between some of the gene expression and cell viability features was recorded during the initial data analysis, a principal component analysis was performed to extract important features and reduce these cross-correlations. Again, the work is described in a [Jupiter Notebook](https://github.com/SimonaKolarova/Drug-s-Mechanism-of-action/blob/main/Principal%20component%20analysis.ipynb) with the most importantant observations detailed in the [HTML project description ('Principal component analysis')](https://simonakolarova.github.io/mechanism_of_action.html#item-4).

## Predictive modelling
Lastly, the knowledge obtained in the previous sections was used to preprocess the dataset and construct a neural network machine learning algorithm for the prediction of the probability of a drug having a specific mechanism of action. The log loss for the training data set was ~0.012 and for the external validation dataset ~0.019. For comparison, the log loss of the [winning submissions for the external validation dataset on Kaggle](https://www.kaggle.com/c/lish-moa/leaderboard) is ~0.016. Please find my [Kaggle machine learning notebook](https://www.kaggle.com/simonakolarova/moa-predictions) and more imformation about the model tranining and evalutation in the [HTML project description ('Predictive modelling')](https://simonakolarova.github.io/mechanism_of_action.html#item-5).
Additionally, please find brief analysis of the importance of the different variables for the predictive model in my [Kaggel feature importance notebook](https://www.kaggle.com/simonakolarova/moa-feature-importance) and discussion of these results in the [HTML project description ('Predictive modelling')](https://simonakolarova.github.io/mechanism_of_action.html#item-5-3).


## Thank you for the great course!

