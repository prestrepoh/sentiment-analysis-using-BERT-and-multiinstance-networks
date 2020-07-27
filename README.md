# Opinion Lab Group 1.4

### Presentation Timetable

|        | 1st      | 2nd      | 3rd      | 4th      | 5th      | 6th      | Final    |
|--------|----------|----------|----------|----------|----------|----------|----------|
| Slot 1 | 27\.04\. | 11\.05\. | 25\.05\. | 08\.06\. | 22\.06\. | 06\.07\. | 20\.07\. |

### Description:
For the first topic about media agenda setting, a better sentiment analysis model is necessary. The idea of this project is to develop such a domain specific sentiment analysis model to predict sentence-level sentiment on social media comments on organic food products. Therefore, a small neural network is pre-trained on BERT sentence features and fine-tuned on our own Annotated Organic Dataset.

### Action items:
Apply the Milnet approach on sentences instead of discourse units. You can take the provided code or make your own from scratch.
As data take Amazon product reviews containing the keyword "organic" from the following categories (do your own random train/val/test splits):

 - Grocery and Gourmet Food 
 - Health and Personal Care 
 - Beauty

As features take BERT CLS embeddings on sentences.
As performance metrics, provide accuracy, micro and macro F1 scores per category and data split.
Eventually fine-tune the model on the Annotated Organic Dataset. Only take these sentences which only have one aspect-based sentiment annotated. Predict only sentiment, nothing else.

### Resources:
- [Paper: Multiple Instance Learning Networks for Fine-Grained Sentiment Analysis](https://gitlab.lrz.de/nlp-lab-course-ss2020/opinion-mining/overview/-/wikis/uploads/22749a9c3cad52972f0d782aac43e4e3/1711.09645.pdf)
- [Pre-trained multi-lingual Google BERT](https://github.com/google-research/bert)
- [Annotated Organic Dataset](https://gitlab.lrz.de/social-rom/organic-dataset/annotated-dataset/-/tree/master/annotated_3rd_round/processed/train_test_validation%20V0.3)
- [Amazon product reviews](http://jmcauley.ucsd.edu/data/amazon/links.html)
- [Sentiment analysis baseline](https://nlpforhackers.io/sentiment-analysis-intro/)
