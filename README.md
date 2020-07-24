# Abstractive-Text-Summarization(Seq2Seq) using GRU

Abstractive Text Summarization

First, we can form our problem as a sequence-to-sequence problem (a sequence prediction problem) at word-level where the input sequences are long english statement(s) and the output is a shorter-length, same-meaning, different-words summary.

In general, the input sequences and output sequences in sequence-to-sequence learning have different lengths (such as text summarization and machine translation) and the entire input sequence is required in order to start predicting the target.

In Keras, the process is done as follow:

    A RNN layer (Here, we will use GRU) acts as "Encoder": it processes the input sequence and returns its own internal state.
    Another RNN layer (GRU) acts as "Decoder": it is trained to predict the next words of the target sequence, given previous words of the target sequence.

Dataset

Amazon Fine Food reviews

Other Required Files

attention layer file.

Note: Keras has a built-in Attention class. Unfortunately, it is more suitable for CNNs than RNNs. Therefore, we will use a third-paty attention layer file.

References:

1- Sequence Models (Course 5 of the Deep Learning Specialization), Deeplearning.ai, Andrew Ng

https://www.youtube.com/playlist?list=PLkDaE6sCZn6F6wUI9tvS_Gw1vaFAx6rd6

2- Comprehensive Guide to Text Summarization using Deep Learning in Python, Aravind Pai

https://www.analyticsvidhya.com/blog/2019/06/comprehensive-guide-text-summarization-using-deep-learning-python/#comment-160299

3- A ten-minute introduction to sequence-to-sequence learning in Keras, Francois Chollet

https://blog.keras.io/a-ten-minute-introduction-to-sequence-to-sequence-learning-in-keras.html
