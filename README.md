# DL-Assignment-2
1. Translation
For this sequence-to-sequence model built using LSTM layers, we assume an input embedding size 𝑚=256m=256, hidden state size 𝑘=256k=256 for both the encoder and decoder, sequence length 𝑇=15T=15, and vocabulary size 𝑉=60V=60. The model does not use attention and relies on greedy decoding during inference. The total number of computations is calculated using the formula 𝑇×[8𝑘(𝑚+𝑘)+𝑘𝑉]T×[8k(m+k)+kV]. Substituting the values gives 
 15×[8×256×(256+256)+256×60]=15×(1048576+15360)=15×1063936=15,959,04015×[8×256×(256+256)+256×60]=15×(1048576+15360)=15×1063936=15,959,040. Hence, the total number of computations is approximately 15.96 million operations.

The total number of parameters in the model is computed using the formula 2𝑉𝑚+8𝑘(𝑚+𝑘+1)+𝑘𝑉+𝑉2Vm+8k(m+k+1)+kV+V. Plugging in the values, we get 2×60×256+8×256×(256+256+1)+256×60+60=30,720+1,050,624+15,360+60=1,096,7642×60×256+8×256×(256+256+1)+256×60+60=30,720+1,050,624+15,360+60=1,096,764. Therefore, the total number of parameters in the network is approximately 1.10 million.
