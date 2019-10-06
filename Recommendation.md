# Recommendation
## Traditional Sequential Recommendation
- ### *Session-Based Recommendations with Recurrent Neural Networks*
  - argued that RNNs can be applied to session-based recommendation with remarkable results, dealt with the issues that arise when modeling such sparse sequential data and also adapted the RNN models to the recommender setting by introducing a new ranking loss function suited to the task of training these models.

- ### *Recurrent neural networks with top-k gains for session-based recommendations*
  - gave an improved version of GRU4Rec, which adopts a different loss function and sampling strategy, and shows significant performance gains on Top- N recommendation.



## Transformer-based Recommendation

- ### *Self-Attentive Sequential Recommendation*
    - proposed a Self-Attention based Sequential Recommendation model (SASRec) that is able to draw context from all actions in the past (like RNNs) and frame predictions in terms of just a small number of actions (like MCs).

- ### *Behavior Sequence Transformer for E-commerce Recommendation in Alibaba*
  - applied the self-attention mechanism to learn a better representation for each item in a user’s behavior sequence by considering the sequential information in embedding stage, and then feed them into MLPs to predict users’ responses to candidate items.

- ### *BERT4Rec: Sequential Recommendation with Bidirectional Encoder Representations from Transformer*
  - proposed a model called BERT4Rec which employs the deep bidirectional self-attention to model user behavior sequences through Cloze task.

- ### *Deep Session Interest Network for Click-Through Rate Prediction*
  - proposed a novel CTR model named Deep Session Interest Network (DSIN) that leverages users’ multiple historical sessions in their behavior sequences. (1)Using **self-attention** mechanism with bias ****encoding to extract users’ interests in each session**.(2)Applying **Bi-LSTM** to model how users’ interests evolve and interact among sessions. (3)Employing the local activation unit to learn the influences of various session interests on the target item.

## Repeat Consumption
- ### *Modeling Item-Specific Temporal Dynamics of Repeat Consumption for Recommender Systems*
  - firstly analyzed repeat consumption and temporal dynamics on the datasets and proposed a holistic model that can recommend both novel and consumed items simultaneously, called SLRC(Short-Term and Life-Time Repeat Consumption model). It combines collaborative filtering (CF) which helps to better capture users’ preferences and explore novel items and Hawkes Process which utilizes patterns of repeat consumption to properly rank consumed items higher at specific time.

- ### *RepeatNet: A Repeat Aware Neural Recommendation Machine for Session-based Recommendation*
  - investigated repeat consumption by incorporating a repeat-explore mechanism into neural networks and proposed a new model called RepeatNet with an encoder-decoder structure. Specially, the decoder includes two modes-repeat mode and explore mode, aiming to recommend old and new items respectively.

- ### *The Dynamics of Repeat Consumption*
  - developed a hybrid model that predicts user choice based on a combination of recency and quality of consumptions.

- ### *Incorporating Copying Mechanism in Sequence-to-Sequence Learning*
  - incorporated copying into neural network-based Seq2Seq learning and proposed a new model called COPYNET with encoder-decoder structure which can choose subsequences in the input sequence and put them at proper places in the output sequence.

- ### *Pointer Networks*
  - proposed a new architecture-Pointer Net, which deals with the fundamental problem of representing variable length dictionaries by using a softmax probability distribution as a “pointer”.

## New-item Recommendation

- ### *New Item Consumption Prediction Using Deep Learning*
  - proposed PISA(Purchase Intent Session-bAsed), a content-based purchase prediction method for cold start session-based recommendations. Two phases: (1)using the item descriptions and categories to create word embeddings that model the relationships among items (2)using these embeddings to model the items in each session and predict the likelihood of a purchase.

- ### *Fashion Retail: Forecasting Demand for New Items*
  - applied deep learning and tree based machine learning algorithms to get point estimates in forecasting demand for items which were not present in the catalog earlier (new or unseen items).
