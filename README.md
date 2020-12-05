# Seq2Seq-chatbot-with-attention

## Introduction

This Chatbot is a TensorFlow implementation of Seq2Seq Mode. It makes use of an attention-based seq2seq RNN model.

Encoder architecture: Stacked Bidirection LSTM with 400 nodes

Decoder architecture: LSTM with 400*2 nodes
	
### Results :
| Train Accuracy | Test Accuracy |
|:---:|:---:|
| 83.72%  |  78.40%|

The overall architecture of the model using model.summary() :
<img src = 'model_plot4a.png' >
