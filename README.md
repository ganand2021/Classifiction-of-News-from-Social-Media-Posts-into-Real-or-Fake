
# Classifiction of News from Social Media Posts into Real or Fake

CIS 522 - Final Project

## Description

In the age of the internet, information is freely and easily accessible.
However, it comes with its own share of benefits and risks. One major
bane is misinformation. Misinformation is prevalent on every social media
platform like Facebook, TikTok, Snapchat, Reddit, Whatsapp, Instagram,
Twitter, etc. These pose extreme risks right from affecting elections to
posing grave health risks as we observed during the COVID-19 pandemic
and in certain cases might also lead to fatalities. A major source of this is
fake news. Most people are usually led to believe that news structured in
a formal way should ideally be from a reliable news source, but it is often
not. We aim to address this issue of identifying fake news so that such
content can be flagged and removed before it causes any disturbance. The
rapid advancements in NLP help us tackle this problem and identify news
as either real or fake. In this project, we use the publicly available Kaggle
News dataset that contains news data from reputed and trustable news
sources as our training set and news scraped from social media platforms
like Reddit and Twitter forms our test set. The data is trained on multiple
models starting from simple Machine Learning models to the state of
the art Transformer models. The trained models were then used for the
classification task and the results obtained display high accuracy values
and F1 scores in identifying fake news irrespective of the distribution of
news data and where it was posted.
## Team Members

* [Gopik Anand](https://github.com/ganand2021) 
* [Arvind Balaji Narayan](https://github.com/narvind24/)
* [Vasanth Kolli]()
## Repo Content Explanation

The **Datasets** folder consists of the text content that is used to train the models. They should be in the working directory of the Jupyter Notebooks for the code to execute as expected.

The **Models** consists of the independent jupyter notebooks for each model we trained for this project which can be executed as a whole as long as the data exists in the working directory.
Depending upon the data used as the training set and the test set, the models are stored in the following directories:

- *Train Kaggle Test Reddit*
- *Train Kaggle Test Twitter*
- *Train Kaggle Test Reddit+Twitter*

## Results

#### Train: Kaggle, Test: Reddit
| *Model Name*     | *Validation Accuracy* | *F1 Score*     |
| :---            |    :----:           |          ---:|
| Naive Bayes            |  0.3559         |          0.3559|
| SVM            |    0.4613           |          0.4613|
| BiLSTM            |    0.4412           |          0.4412|
| TextCNN            |    0.4469           |         0.276|
| RoBERTa            |    0.7968590659           |          0.7968590659|
| AlBERT            |    0.5135631246           |          0.6786147419|
| DistilBERT            |    0.821537834           |          0.821537834|
| Canine            |    0.794207628           |          0.8853018074|
| GPT-2           |    0.7829900061           |          0.8782887211|
| DeBERTa            |    0.8019579849           |          0.8900962083|
| Electra            |    0.8256169692           |          0.8256169692|
| XLM-RoBERTa            |    0.8025698552           |          0.8025698552|
| XLNet            |    0.8168468285           |          0.8168468285|
| BERT            |    0.8221497043           |          0.8221497043|
|LinkBERT  |        0.8127676932       |       0.8967146715         |



#### Train: Kaggle, Test: Twitter

| *Model Name*     | *Validation Accuracy* | *F1 Score*     |
| :---            |    :----:           |          ---:|
| Naive Bayes            |  0.5048         |          0.5048|
| SVM            |    0.5111           |          0.5111|
| BiLSTM            |    0.5136           |          0.5136|
| TextCNN            |    0.5624           |         0.5694|
| RoBERTa            |   0.919          |          0.919|
| AlBERT            |    0.5941460132           |          0.5560053981|
| DistilBERT            |    0.8903          |          0.8903|
| Canine            |    0.8963777055           |          0.9018065887|
| GPT-2           |    0.8918918919           |          0.8953538862|
| DeBERTa            |    0.9126387799           |          0.9187610804|
| Electra            |    0.8865           |          0.8865|
| XLM-RoBERTa            |    0.9185          |          0.9185|
| XLNet            |    0.8995           |          0.8995|
| BERT            |    0.888           |          0.888|
|LinkBERT  |        0.920264663       |      0.9259297844         |


#### Train: Kaggle, Test: Reddit + Twitter

| *Model Name*     | *Validation Accuracy* | *F1 Score*     |
| :---            |    :----:           |          ---:|
| Naive Bayes            |  0.452        |          0.452|
| SVM            |    0.4934           |          0.4934|
| BiLSTM            |    0.4849           |          0.4849|
| TextCNN            |    0.5052           |         0.4916|
| RoBERTa            |   0.8869030391          |          0.8869030391|
| AlBERT            |    0.5655571635           |          0.6144361675|
| DistilBERT            |    0.8429088278         |          0.8429088278|
| Canine            |    0.860130246           |          0.8938320426|
| GPT-2           |    0.8532561505           |          0.8870446697|
| DeBERTa            |    0.8733719247           |          0.9050151976|
| Electra            |    0.8767727931           |          0.8767727931|
| XLM-RoBERTa            |    0.89328         |          0.92515|
| XLNet            |    0.8825615051           |          0.8825615051|
| BERT            |    0.8628075253           |          0.8628075253|
|LinkBERT  |        0.8821273517       |      0.9118840266         |
