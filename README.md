# RNN_Story_Generator_Char_Level

This piece of code uses PyTorch for training a character level RNN using LSTM to output a story in the style of the author Anna Karenina. It has been trained on text of 1985223 characters. It can take a starting character as input and output the subsequent characters in a way that the resultant bunch of characters will resemble a story written by Anna Karenina.
anna.txt is the file that has the dataset

Dependencies are - PyTorch, numpy, python
I used CUDA/GPU for training so if you want it to train faster make sure you have access to a GPU. If not the code still works on a GPU.

# Architecture
It has 2 LSTM layers followed by a fully connected layer (256 -> 83) with softmax at the end. Used Adam Optimizer with a learning rate = 0.001 and trained for 20 epochs. Loss function is cross entropy loss
