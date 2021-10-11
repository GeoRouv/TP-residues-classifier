# TP-residues-classifier
Classifying residues of transmembrane proteins using a custom Seq2Seq model.

## Intro

The implementation of a neural network for tackling structural bioinformatics problems is not a novel approach, but the implementation of a sequence-to-sequence model for the detection of transmembrane amino acids certainly is. Below we expand on how our neural network model was designed and constructed, and discuss further preprocessing that is particularly significant for the performance of our model.

## Design

We approached the problem of classifying residues as a sequence-to-sequence problem, since an aminoacid sequence would be handed in as input, and the classification of each aminoacid-transmembrane/ non-transmembrane- would be the outputted as a sequence as well, a sequence of zeros and ones. 

As such, no structural properties of the proteins were taken into account for model training or amino acid classification, and the proposed prediction algorithm consists a purely sequence-based approach. 

For the neural network approach, an encoder-decoder model was constructed. Encoder-decoder models are an alternative way of structuring Recurrent Neural Networks (RNNs) for sequence-to-sequence prediction problems.

<img src="./images/aaa.png" alt="drawing" width="400"/>
