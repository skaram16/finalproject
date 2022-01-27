# Kaggle Titanic

For our final project, the <b>goal</b> is to perform a 2-label <b>classification problem</b>: to predict which <b>passengers survived</b> the tragedy. <br> [Kaggle](https://www.kaggle.com) offers two datasets. One training (the labels are known) and one testing (the labels are unknown). The goal is to submit a file with our predicted labels saying who survived or not. <br>

We had access to several types of features (numerical, text, categorical). The <b>big challenge</b> with this dataset was the size of the data we have. The <b>training set</b> is composed of only <b>891 samples</b>. The testing set is composed of 418 samples. <br>Therefore, the main issue is to design an algorithm which generalizes enough in order to avoid <b>over-fitting</b>. To do so, a bunch of features were generated. Then, an modeling method with the usage of random tree classifier is used in order to get the most generalized model.<br><br>


This is a multi-label classification, with 2 labels:

- 0: passenger did not survive/passed away
- 1: passenger survived










Tableau - https://public.tableau.com/app/profile/sabrina6697/viz/Final_Project_Titanic/AgeHistogram?publish=yes
