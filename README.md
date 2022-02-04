# Seq2Seq-chatbot-with-attention

## Introduction

This Chatbot is a TensorFlow implementation of Seq2Seq Mode. It makes use of an attention-based seq2seq RNN model.

The classical architecture for the seq2seq model uses an "encoder" to encode the input sentence into a hidden
vector and then uses a "decoder" to generate the output. However, putting all
information into a single vector makes the encoder prune to forget something. Furthermore, different parts of the input
can be more valuable at each generation step, yet the decoder sees only one source representation. Using an attention
mechanism can resolve this issue. The main idea is that a model can
learn which input parts are more important at each step. In this setting, the encoder will not compress the whole input
into a single vector, but it outputs as many hidden state vectors as the number of instances in the input sequence.


Encoder architecture: Stacked Bidirection LSTM with 400 nodes

Decoder architecture: LSTM with 400*2 nodes
	
### Results :
| Train Accuracy | Test Accuracy |
|:---:|:---:|
| 83.72%  |  78.40%|

The overall architecture of the model using model.summary() :
<img src = 'model_plot4a.png' >
