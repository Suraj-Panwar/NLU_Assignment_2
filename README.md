# NLU_Assignment_2
Natural Language Understanding Assignment 2 
The repository contains following files with mentioned applications as required in NLU assignment2 for class of 2018:

## 1. Kneser_ney_perplexity.py
This program generates perplexity for the Kneser Ney based Trigram model as produced in the first assignment. The corpus used is     gutenberg corpus, and running the script produces the perplexity. No input is required as the corpus is loaded from the Sklearn files.

## 2. LSTM_char_perplexity.py
This program creates a character level LSTM model for language modelling and computes the character perplexity based on the Gutenberg corpus. The LSTM parameters can be changed by the user and have been mentioned in the program. The model is trained on a 60% split of the gutenberg corpus and the test perplexity is carried out on the 20% split og gutenberg corpus. The random.seed() is same in all files allowing same splits on all of them.

## 3. LSTM_word_perplexity.py
This program creates a word level LSTM model for language modelling and computes the word perplexity based on the Gutenberg corpus. The LSTM parameters can be changed by the user and have been mentioned in the program. The model is trained on a 60% split of the gutenberg corpus and the test perplexity is carried out on the 20% split og gutenberg corpus. The random.seed() is same in all files allowing same splits on all of them. The vocabulary size used in this program is almost 34000 and thus takes a lot of time to compute per epoc.

## 4. LSTM_char_sent_trainer.py
This programs creates a sentence generation model for creating a random sentence of desired sequence length which can be changed by the user. The program is based on the character level LSTM model implementation of the gutenberg corpus and gives a sentences generated entirely of characters used in gutenberg corpus. The generator also outputs a weights file which can be reused by the model for generating the sentence without actual training the model every time. The model is trained on top 1 million words and can be changed by the user based on the computation resources avaliable.

## 5. LSTM_char_sent_generator.py
The model uses the weights created by the LSTM_char_sent_trainer.py and uses them to compute the random sentence to be generated from the corpus. The generated sequence length can be altered by the user and the starting seed word although taken random in this case can be altered by the user to generate a sentence starting from a specific seed word.
