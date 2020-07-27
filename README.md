# Multimodal Multiparty Emotion Recognition System in Conversation (Text-Mode Only)



Multimodal EmotionLines Dataset (MELD) has been created by enhancing and extending EmotionLines dataset. 
MELD contains the same dialogue instances available in EmotionLines, but it also encompasses audio and visual modality along with text. 
MELD has more than 1400 dialogues and 13000 utterances from Friends TV series. 
Multiple speakers participated in the dialogues. 
Each utterance in a dialogue has been labeled by any of these seven emotions -- Anger, Disgust, Sadness, Joy, Neutral, Surprise and Fear. 
MELD also has sentiment (positive, negative and neutral) annotation for each utterance.


A Multimodal Multi-Party Dataset for Emotion Recognition in Conversation has been accepted as a full paper at ACL 2019. 
The updated paper can be found here - https://arxiv.org/pdf/1810.02508.pdf


## Files
- /data/MELD/train_sent_emo.csv - contains the utterances in the training set along with Sentiment and Emotion labels.
- /data/MELD/dev_sent_emo.csv - contains the utterances in the dev set along with Sentiment and Emotion labels.
- /data/MELD/test_sent_emo.csv - contains the utterances in the test set along with Sentiment and Emotion labels.




## Labeling
For experimentation, all the labels are represented as one-hot encodings, the indices for which are as follows:

- **Emotion** - {'neutral': 0, 'surprise': 1, 'fear': 2, 'sadness': 3, 'joy': 4, 'disgust': 5, 'anger': 6}. Therefore, the label corresponding to the emotion 'joy' would be [0., 0., 0., 0., 1., 0., 0.]
- **Sentiment** - {'neutral': 0, 'positive': 1, 'negative': 2}. Therefore, the label corresponding to the sentiment 'positive' would be [0., 1., 0.]
