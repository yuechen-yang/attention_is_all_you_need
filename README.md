# Attention Is All You Need
This is the paper presentation repo for "Attention Is All You Need".


## Overview

1. The paper proposes a new network architecture, the Transformer, based solyely on attention mechanisms. The Transformer is more parallelizable and require less time to train (WMT).
2. The Transformer contains Encoder and Decoder parts. Each of them contaions 6 identical layers.
3. For Encoder, each layer has 2 sub-layers. The first is a multi-head self-attention mechanism, and the second is a simple, position-wise fully connected feed forward network.
4. The Decorder is also composed of 6 identical layers. In addition to the two sub-layers in each encoder layer, the decoder inserts a third sub-layer, which performs multi-head attion over the output of the encorder stack.
5. An attention function can be described as mapping a query and a set of key-value pairs to an output, where the query, keys, values, and output are all vectors. The Transformer model in this paper uses the "Scaled Dot-Product Attention".


### The picture in this paper

<div align=center><img src="img/1.png" style="zoom:50%" />  
<p></p>
<img src="img/2.png" style="zoom:50%" />
<p></p>
<img src="img/3.png" style="zoom:50%" />
</div>


## Discussion Topic 1

Why they use mask?

## Discussion Topic 2



## Discussion Topic 3




## Critical Analysis

1. The paper poposed a new mdoel architecture and it is only foced on translation.



## Resource links

1. Original Article: https://arxiv.org/abs/1706.03762v5
2. Code and trained PFNs are released at https://github.com/tensorflow/tensor2tensor


## Code demonstration

The code has not yet been made availalbe.

## Video Recording

Link to video recording.
