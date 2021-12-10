# END-3.0-Assignment-7
Assignment 7 of the END 3.0 course of The School Of AI
## Precision, Recall, F1-Score

Precision, recall and F1-Score are used to judge the performance of our model in classification tasks. It is usually preferred over accuracy when we are provided a skewed dataset, or a multi-classification dataset. We can measure the performance of classification model by constructing a confusion matrix.<br /><br />

__Precision__ : It is the ratio of number of correctly labelled instances of a particular class to the total number of instances labelled as that particular class. Answers the question "How many of the examples predicted as Class X are correct ?"<br /><br />

__Recall__ : It is the ratio of number of correctly labelled instances of a particular class to the actual number of instances pertaining to that class. Answers the question "Out of all the examples actually in Class X, how many are predicted correctly ?"<br /><br />

__F1-Score__ : There is a trade-off between precision and recall in classification problems. So, in most instances, we use the harmonic mean of the precision and recall.<br />
F = 2PR/(P+R)

![Confusion Matrix](https://github.com/MohammedYaseen97/END-3.0-Assignment-7/blob/main/confusion_matrix.png)

## BLEU Score

BLEU Scores score the quality of language translation by judging how many words/groups of words that appear in the reference translation, also appear in the candidate translation. Hence, the formula is adjusted to score words that appear in candidate translation and which are also present in reference translation. We use a concept called n-grams, which basically means groups of words. <br /><br />

The one obvious disadvantage of BLEU score is that it makes its judgement solely based on the reproducibility of words. It scores a good translation poorly because they might not repeat the same words, while scoring highly for a sentence which has a lot of n-grams repeating without making any sense of the sentence.

![Bleu Score](https://github.com/MohammedYaseen97/END-3.0-Assignment-7/blob/main/BLEU4.png)

## Perplexity

When we are trying to model language, we need probability for the formation of a particular sequence. Ex : P("abcd"), P("abc") - trigram, P("cd") - bigram. But often when the sequence is long, the probabilities get very very small, and in extreme cases, might result in underflow. For that reason, we prefer perplexity where perplexity of a sequence is measured as the exponential average negative log likelihood of a sequence. For a sequence X = (x0, x1, x2, .... , xt), <br /><br />

PPL(X) = exp{-1/t Σlogp(xi/x<i)} <br /><br />

For long sequences, we can take the perplexity of fixed-length sequences like bi-gram, tri-gram. In code, usually we retrieve perplexity of sequences using exp(NLLLoss).

## BERT Score

BERTScore uses the pre-trained contextual embeddings from BERT and matches words in candidate and reference sentences by cosine similarity. Moreover, BERTScore computes precision, recall, and F1 measure, which can be useful for evaluating different language generation tasks.<br />
Below is an illustration of how BERT Score Recall works :

![BERT Score](https://github.com/MohammedYaseen97/END-3.0-Assignment-7/blob/main/bert_score.png)

Group 21 members : <br />

Mohammed Yaseen (47.yaseen@gmail.com)<br />
Mayank Singhal (singhal.mayank77@gmail.com)<br />
Ravi Vaishnav (ravivaishnav20@gmail.com)<br />
Sundeep Joshi<br />
