# Udacity data science nanodegree course
## _Introduction to data science end of module project_

## Theme

This project was run based on the data from tennis ATP games results. On top of games players, results or scores, the dataset used provides the betting odds that are used to understand if a simple gambling strategy can be used to ensure or maximize benefits.

## Methodology

The initial question I was wanting to find an answer to was, plainly, if there was a simple way to have a beneficial betting strategy on tennis matches.

To try and find an answer to this question, I got data from this website: http://tennis-data.co.uk/alldata.php, that provides interesting information regarding tennis matches since 2001, and notably the betting odds coming from different gambling platforms. There is also an average value for the odds.

I made the choice to focus on the last 2 years. Some rows were not useful for the analysis and were removed, mainly those were one of the players' ATP rank was missing.

First step was to analyze the reliability of the odds by checking which proportion of matches ended according to the pre-match odds (lowest value wins). As Grand Slam tournaments were identified as the most reliable, a focus was performed on those to analyse each round.

Next step was to try a very simple and naive modelling to predict the odds by using only the rankings of both players. As expected, this proved too simple and a more complex model was needed. This more complex model was assumed to be needing additional features that were not included in the original data. This original data was therefore enriched by computing new columns with the number of wins in last 5 and 10 matches for both players. This allowed to get better results, but still quite far from satisfcatory.

However it provides a reasonable confidence in the fact that adding new features to the model would lead to better results (but that's for next time).

## Contents

The project is composed of a 4 jupyter notebook files. All comments are provided in it but, in a nutshell:

- Analysis: Imports the data downloaded from the original file, check how reliable are the odds (is the player with the lowest value always winning ? hint: no), study the correlation between the level of reliability of the odds and the type of tournament, analyze a gambling strategy for the four biggest tournaments (Grand Slams)
- TooSimplePrediction: tries a naive approach of predicting the odds by using only the rankings of both players
- Enrichment: computes some additional data to use as features in the hope of getting a better model (number of wins in last 5 and 10 matches)
- SimplePrediction: tries to predict the odds using the newly computed features

## Installation

Nothing special here, you just need a jupyter notebook instance running.

## More information needed?

Go there: https://medium.com/@leosartorius/betting-on-tennis-matches-how-simple-is-that-d70b60c4593

## License

MIT

**Free Software, Hell Yeah!**

