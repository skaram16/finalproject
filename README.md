# Kaggle Titanic

![Titanic](https://github.com/skaram16/finalproject/blob/main/Images/Titanic.jpeg)

For our final project, the <b>goal</b> is to perform a 2-label <b>classification problem</b>: to predict which <b>passengers survived</b> the tragedy. <br> [Kaggle](https://www.kaggle.com) offers two datasets. One training (the labels are known) and one testing (the labels are unknown). The goal is to submit a file with our predicted labels saying who survived or not. <br>

We had access to several types of features (numerical, text, categorical). The <b>big challenge</b> with this dataset was the size of the data we have. The <b>training set</b> is composed of only <b>891 samples</b>. The testing set is composed of 418 samples. <br>Therefore, the main issue is to design an algorithm which generalizes enough in order to avoid <b>over-fitting</b>. To do so, a bunch of features were generated. Then, an modeling method with the usage of random tree classifier is used in order to get the most generalized model.<br><br>


This is a multi-label classification, with 2 labels:

- 0: passenger did not survive/passed away
- 1: passenger survived

For this type of feature, we can observe the average survival of passengers within each categories. The observed features are: 

- PClass
- Sex
- Embarked
- SibSp
- Parch

Conclusion:

- Pclass and Sex has a great correlation with the survival of people -> Keep directly them as features
- SibSp & Parch have a sort of correlation but feature engineering is required: We can sum the two and then know:
	- if the passenger was alone 
	- if the passenger was with a big or a small family
- Embarked: 3 labels with no assumed order -> one-hot encoding 

### Numerical Features

For this type of feature, we can observe the distribution of the passengers given the survival. The observed features are: 

- Age
- Fare
- Gender

<u>Conclusion:</u>
- Younger and older people survived.
- The middle age (20-40) people did not survive. 
- We should consider that the passengers age is a predictor
- Age is skewed and Fare is highly skewed



### Resource Sites for Presentation:

Tableau - https://public.tableau.com/app/profile/sabrina6697/viz/Final_Project_Titanic/AgeHistogram?publish=yes
Google Slides - https://docs.google.com/presentation/d/1IFVcrnvRRrImdb5s6TLPkYXL-65yKagD_-F9EQwRS48/edit?usp=sharing
