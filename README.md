# Neural-Machine-Translation--English-to-French
Neural Machine Translation is the use of deep neural network for the problem of machine translation. Here in encoder, a RNN layer is used. It processes the input sequence and returns its own internal state. Another RNN layer is used as decoder. It is trained to predict the next characters of the target sequence, given the previous characters of the target sequence. 
The summary of the process includes: 
1. The english sentences have to be converted in a 3D array of shape (number_of_pairs, max_english_sentence_length, number_english_characters) which is basically a one-hot vectorization. 
2. Decoder input data is also a 3D array of shape (number_of_pairs, max_french_sentence_length, max_french_characters). 
3. Decoder target data is same as decoder input data but offset by one timestamp. 
4. We have to train a RNN-LSTM to convert english language into french language. 

# Reference: 
1. https://blog.keras.io/a-ten-minute-introduction-to-sequence-to-sequence-learning-in-keras.html
