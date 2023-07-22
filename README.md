# Hope lexicon 🤞💚

This lexicon was built following the approach of Guerra et al<sup>1</sup>.
According to the Collins dictionary, “Hope is a feeling of desire and expectation that things will go well in the future.”, therefore something to be hopeful needs to be a subjective anticipation of a positive outcome. 
To identify words with these features, we utilized the [NRCLex library](https://pypi.org/project/NRCLex/) to cross-reference the dictionaries for the categories "anticipation," "positive," and "joy." We selected words that exhibited "anticipation," at least one of either "positive" or "joy," and were also considered subjective. To meet this third requirement, we utilized the [`textblob.subjectivity`](https://textblob.readthedocs.io/en/dev/api_reference.html#textblob.blob.TextBlob.subjectivity) function, which assigns a score ranging from 0 (not subjective) to 1 (very subjective), and we only selected words with a score higher than 0.5.
The resulting lexicon contains 221 words. 

To ease the integration of this lexicon with the other affect categories of the NRC EmoLex<sup>2</sup>, the file `hope.txt` is formatted as the files available at https://saifmohammad.com/WebPages/NRC-Emotion-Lexicon.htm.

## References
<sup>1</sup> A. Guerra and O. Karakus. Sentiment analysis for measuring hope and fear from Reddit posts during the 2022 Russo-Ukrainian conflict. Frontiers in Artificial Intelligence, 2023.

<sup>2</sup> Saif M. Mohammad and Peter D. Turney. Crowdsourcing a Word-Emotion Association Lexicon. Computational Intelligence, 2013.