# fake-news
Simple binary classifier for fake news articles using fastai.

This uses the fake_or_real_news.csv file that was prepared by George McIntire in 2017 - see https://opendatascience.com/how-to-build-a-fake-news-classification-model/. The dataset has about 6,000 items, consisting of the headline and text of a news article and the label, FAKE or REAL.

I tried several variations on this model, including removing any records where ‘real’ was in the text and the label was REAL, or ‘fake’ was in the text and the label was FAKE, to avoid "data leakage". That took the dataset down to about 4,800 records. There was a little variability in losses and accuracy with the model and dataset variations, but it generally got around 98-99% accuracy, compared to McIntire's 91.7%.  So it looks to me like the fastai model works amazingly well at classifying McIntire’s dataset.
