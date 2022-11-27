HOW TO EXECUTE THE CODE:

it starts with the importing the drive to the colab notebook environment.
Accesing the files those reside in the drive.
Import the train split from the drive to train the data.
Preprocessing the data such as removing the punctuations etc.

TRAINING THE DATA:

This portion deals with the training the data. The data in training split will be divided into words by using the N-grames and includes the process of finding the probabilities.
This process includes the finding the probability of each sentence and finding the average probability of Train Split by divding the sum of probabilities of the each sentence to total number of sentences of the train split.
This process allows the two files in drive to update the probabilities and average probability of the train split.

DEV DATASET:

Importing the dev dataset allows to work on kneyser smoothing technique that would used to improve the performance of the language model.
kneyser smoothing technique would be implemented by using the equation which includes three terms

P(traigram) = Ckn + lamda*Pcontintution(Wi)

Ckn = max((frequency of triagram)-d,0)/frequency of bigram

lamda = d/C(wi-1)*|no of preceeding words|

C(wi-1) = frequency of semi final word

Pcont(wi) = count(final word)/len(sentences)

TESTING THE DATA:

Import the test data split
Preprocess the data
Divide the sentences using trigarm language model
calculating the probabilities of each sentence by using trigram
calculating average probability of the test split
performance analysis by perplxity equation: probability(total sentences)power(-1/N), where N represents the N grames
checking the probability of a sentence given by user.
Generates the two text files contains the probabilities of every sentence and average probability of the test split in drive


FINDING THE PROBABILITIES OF SENTENCE AND AVERAGE PROBABILITY OF DATASPLITS:

Probabilities of the sentences can be calculated by the N-grams those have been used in this language model.
Average Probability of a data split can be calculated by dividing the sum of probabilities of every sentence of split by total number of sentences.


