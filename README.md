# NBA Lineup Prediction

## Overview
This project focuses on predicting the outcome of an NBA match based on the selected lineup of players. Using feature engineering and neural networks, we generated embeddings for each player to capture complex, non-linear relationships based on the home and away team statistics. These embeddings were then used to classify match outcomes using a Random Forest classifier.

### Problem Statement
The problem is divided into two key predictions:
1. **Match Outcome Prediction**: Given 5 home players and 5 away players, predict the outcome of the match (win or lose for the home team).
2. **Best 5th Player Prediction**: Given 5 home players and 4 away players, predict the best suitable 5th player for the away team lineup to increase its likelihood of winning.

### Approach
1. **Feature Engineering**: We first performed detailed feature engineering to extract relevant statistics from each player, capturing both individual and team performance metrics.
2. **Player Embeddings**: To capture the non-linear relationships in player data, we used neural networks to generate player embeddings that reflect player characteristics, form, and past performance.
3. **Modeling**: 
   - **Random Forest Classifier**: We used Random Forest to classify the outcome as either a win or a loss for the home team based on the generated player embeddings.
   - For the second problem, we predicted the most suitable 5th player for the away team by analyzing the player embeddings to match the characteristics of the players already in the lineup.
   
### Libraries & Tools Used
- **Python**
- **Pandas**: For data manipulation and cleaning
- **NumPy**: For numerical operations
- **Scikit-learn**: For implementing the Random Forest classifier
- **TensorFlow/Keras**: For generating player embeddings using neural networks
- **Matplotlib/Seaborn**: For data visualization

### Dataset
The dataset used contains historical performance data for NBA players, including individual and team-level statistics. This data was preprocessed and cleaned to create features that would aid in predicting the match outcome and the best player lineup.

### Results
The model demonstrates the ability to predict match outcomes with a high degree of accuracy, as well as to suggest the most impactful 5th player for an away team lineup. Further improvements could include integrating player injury data and other advanced statistics to enhance the model's predictive power.
