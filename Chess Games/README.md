# Chess Games

## Overview
In this project, I analyzed a chess dataset that I found on Kaggle. This was my first project on Kaggle and I used this dataset as a way to test my skills in conducting data analysis, visualization, and even a small attempt at a classification model as well. Please feel free to look at the code, get inspired by it, criticize it, and suggest more things that I can do in terms of analysis.

### Links
* Dataset: [Online Chess Games](https://www.kaggle.com/datasets/ulrikthygepedersen/online-chess-games)
* This notebook on Kaggle: [Chess Data Analysis](https://www.kaggle.com/code/anaqiamir/chess-data-analysis#Conclusion)
* My Kaggle profile: [Anaqi Amir](https://www.kaggle.com/anaqiamir)

## Findings/Results

### EDA
Here are some of the results that we've discovered in the EDA:

* Most games are rated
* Average white rating: 1597
* Average black rating: 1589
* The top 3 openings (all with 1000+ occurences unlike the rest of the openings) are:
  * Sicilian Defense: 2632
  * French Defense: 1412
  * Queen's Pawn Opening: 1233
* result_by_skill:
  * There are more definitive games at the beginner level
  * There are more drawn games at the expert level
  * The player with the white pieces are slightly more likely to win the game compared to the player with the black pieces

### Classification
Furthermore, here is the conclusion on the classification model:

With the Decision Tree model, we managed to create a model that can predict the outcomes of a game at a 63% accuracy should we provide the model with the necessary predictor features.

As mentioned before, though a 63% accuracy may not seem as much, I believe that it is quite high for a chess game predicion model as chess games are highly dependent on the players themselves and how they play which can change from game to game.

## Credits
The dataset belongs to ULRIK THYGE PEDERSEN on Kaggle and can be found [here](https://www.kaggle.com/datasets/ulrikthygepedersen/online-chess-games).
