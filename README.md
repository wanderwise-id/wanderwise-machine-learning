# wanderwise-machine-learning

This is the repository for machine learning models development of Wanderwise app. Wanderwise is a safety travel app that could automatically summarize & classify news from various sources to users to provide safety information regarding tourist destinations.

The flow of development: 
1. Data collection & labeling

First, we scrap online indonesian news from detik news, then we translate these news and fed them to chat gpt api to label these data (getting the summary & classification label). The dataset is saved into a collection in mongodb.

2. Model building

Here, we use the fine-tuning approach to build both the text-summarization and the text-classification model. For the text summarization model, we fine tune the t5-small model. While for the text classification model, we fine tune the distill-bert model. 


3. Saving model

Then, after we're done training the models, we upload them to huggingface hub. 
