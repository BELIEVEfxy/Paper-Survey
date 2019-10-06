# Paper Survey

## 1 Transformer and its Variants
### 1.1 Structure
#### 1.1.1 *Attention is all you need*
proposed an encoder-decoder architecture which achieved to capture long term dependencies by taking long sequences as inputs and explicitly compute the relations between every token via a mechanism called the “self-attention” layer.

#### 1.1.2 *Transformer-XL*
  proposed a new architecture called Transformer-XL (meaning extra long). Instead of computing the hidden states from scratch for each new segment like traditional Transformer, this model can reuse the hidden states obtained in previous segments to resolve the problem of context fragmentation and make training faster.

#### 1.1.3 *Star-Transformer*
  proposed a new lightweight model named “Star- Transformer” which aims to sparsify the architecture by moving the fully-connected topology into a star-shaped structure, avoiding two limitations of Transformer-be quadratic to a sequence length and not efficient when there is no pre-training.

#### 1.1.4 *Improving the Transformer Translation Model with Document-Level Context*
  proposed to extend the Transformer model to take advantage of document-level context by using multi-head self-attention (Vaswani et al., 2017) to compute the representation of document-level context, which is then incorporated into the encoder and decoder using multi-head attention.

#### 1.1.5 *Area Attention*
  proposed area attention, as a general mechanism for the model to attend to a group of items in the memory that are structurally adjacent and because each of these areas can aggregate a varying number of items, the granularity of attention is learned from the data rather than predetermined.

#### 1.1.6 *Adaptive Attention Span in Transformers*
  proposed an alternative to the self-attention layer reduce the computational burden of a Transformer. The new layer learns its optimal context size, resulting in a network where each attention layer gathers information on their own context.

#### 1.1.7 *Input Combination Strategies for Multi-Source Transformer Decoder*
  proposed four different input combination strategies for the encoder-decoder attention in the Transformer architecture-serial, parallel, flat, and hierarchical, in order to solve multi-source sequence-to-sequence tasks better.

#### 1.1.8 *Scheduled Sampling for Transformers*
  proposed a new strategy for using scheduled sampling in Transformer models by making two passes through the decoder in training time.

#### 1.1.9 *Character-Level Language Modeling with Deeper Self-Attention*
  showed that a non-recurrent model can achieve strong results on character-level language model- ing. Specifically, the model uses a deep network of transformer self-attention layers (Vaswani et al. 2017) with causal (backward-looking) attention to process fixed-length inputs and predict upcoming characters.


## 2 Recommendation
### 2.1 Traditional Sequential Recommendation
#### 2.1.1 *Session-Based Recommendations with Recurrent Neural Networks*
  argued that RNNs can be applied to session-based recommendation with remarkable results, dealt with the issues that arise when modeling such sparse sequential data and also adapted the RNN models to the recommender setting by introducing a new ranking loss function suited to the task of training these models.

#### 2.1.2 *Recurrent neural networks with top-k gains for session-based recommendations*
  gave an improved version of GRU4Rec, which adopts a different loss function and sampling strategy, and shows significant performance gains on Top- N recommendation.



### 2.2 Transformer-based Recommendation

#### 2.2.1 *Self-Attentive Sequential Recommendation*
  proposed a Self-Attention based Sequential Recommendation model (SASRec) that is able to draw context from all actions in the past (like RNNs) and frame predictions in terms of just a small number of actions (like MCs).

#### 2.2.2 *Behavior Sequence Transformer for E-commerce Recommendation in Alibaba*
applied the self-attention mechanism to learn a better representation for each item in a user’s behavior sequence by considering the sequential information in embedding stage, and then feed them into MLPs to predict users’ responses to candidate items.

#### 2.2.3 *BERT4Rec: Sequential Recommendation with Bidirectional Encoder Representations from Transformer*
proposed a model called BERT4Rec which employs the deep bidirectional self-attention to model user behavior sequences through Cloze task.

#### 2.2.4 *Deep Session Interest Network for Click-Through Rate Prediction*
 proposed a novel CTR model named Deep Session Interest Network (DSIN) that leverages users’ multiple historical sessions in their behavior sequences. (1)Using **self-attention** mechanism with bias ****encoding to extract users’ interests in each session**.(2)Applying **Bi-LSTM** to model how users’ interests evolve and interact among sessions. (3)Employing the local activation unit to learn the influences of various session interests on the target item.

### 2.3 Repeat Consumption
#### 2.3.1 *Modeling Item-Specific Temporal Dynamics of Repeat Consumption for Recommender Systems*
  firstly analyzed repeat consumption and temporal dynamics on the datasets and proposed a holistic model that can recommend both novel and consumed items simultaneously, called SLRC(Short-Term and Life-Time Repeat Consumption model). It combines collaborative filtering (CF) which helps to better capture users’ preferences and explore novel items and Hawkes Process which utilizes patterns of repeat consumption to properly rank consumed items higher at specific time.

#### 2.3.2 *RepeatNet: A Repeat Aware Neural Recommendation Machine for Session-based Recommendation*
  investigated repeat consumption by incorporating a repeat-explore mechanism into neural networks and proposed a new model called RepeatNet with an encoder-decoder structure. Specially, the decoder includes two modes-repeat mode and explore mode, aiming to recommend old and new items respectively.

#### 2.3.3 *The Dynamics of Repeat Consumption*
  developed a hybrid model that predicts user choice based on a combination of recency and quality of consumptions.

#### 2.3.4 *Incorporating Copying Mechanism in Sequence-to-Sequence Learning*
  incorporated copying into neural network-based Seq2Seq learning and proposed a new model called COPYNET with encoder-decoder structure which can choose subsequences in the input sequence and put them at proper places in the output sequence.

#### 2.3.5 *Pointer Networks*
  proposed a new architecture-Pointer Net, which deals with the fundamental problem of representing variable length dictionaries by using a softmax probability distribution as a “pointer”.

### 2.4 New-item Recommendation

#### 2.4.1 *New Item Consumption Prediction Using Deep Learning*
proposed PISA(Purchase Intent Session-bAsed), a content-based purchase prediction method for cold start session-based recommendations. Two phases: (1)using the item descriptions and categories to create word embeddings that model the relationships among items (2)using these embeddings to model the items in each session and predict the likelihood of a purchase.

#### 2.4.1 *Fashion Retail: Forecasting Demand for New Items*
 applied deep learning and tree based machine learning algorithms to get point estimates in forecasting demand for items which were not present in the catalog earlier (new or unseen items).
