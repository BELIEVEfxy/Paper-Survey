# Transformer and its Variants
## Structure
- ### *Attention is all you need*
  - proposed an encoder-decoder architecture which achieved to capture long term dependencies by taking long sequences as inputs and explicitly compute the relations between every token via a mechanism called the “self-attention” layer.

- ### *Transformer-XL*
  - proposed a new architecture called Transformer-XL (meaning extra long). Instead of computing the hidden states from scratch for each new segment like traditional Transformer, this model can reuse the hidden states obtained in previous segments to resolve the problem of context fragmentation and make training faster.

- ### *Star-Transformer*
  - proposed a new lightweight model named “Star- Transformer” which aims to sparsify the architecture by moving the fully-connected topology into a star-shaped structure, avoiding two limitations of Transformer-be quadratic to a sequence length and not efficient when there is no pre-training.

- ### *Improving the Transformer Translation Model with Document-Level Context*
  - proposed to extend the Transformer model to take advantage of document-level context by using multi-head self-attention (Vaswani et al., 2017) to compute the representation of document-level context, which is then incorporated into the encoder and decoder using multi-head attention.

- ### *Area Attention*
  - proposed area attention, as a general mechanism for the model to attend to a group of items in the memory that are structurally adjacent and because each of these areas can aggregate a varying number of items, the granularity of attention is learned from the data rather than predetermined.

- ### *Adaptive Attention Span in Transformers*
  - proposed an alternative to the self-attention layer reduce the computational burden of a Transformer. The new layer learns its optimal context size, resulting in a network where each attention layer gathers information on their own context.

- ### *Input Combination Strategies for Multi-Source Transformer Decoder*
  - proposed four different input combination strategies for the encoder-decoder attention in the Transformer architecture-serial, parallel, flat, and hierarchical, in order to solve multi-source sequence-to-sequence tasks better.

- ### *Scheduled Sampling for Transformers*
  proposed a new strategy for using scheduled sampling in Transformer models by making two passes through the decoder in training time.

- ### *Character-Level Language Modeling with Deeper Self-Attention*
  showed that a non-recurrent model can achieve strong results on character-level language model- ing. Specifically, the model uses a deep network of transformer self-attention layers (Vaswani et al. 2017) with causal (backward-looking) attention to process fixed-length inputs and predict upcoming characters.
