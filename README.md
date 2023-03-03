# Wordsplay

We have used PubMed RCT dataset.
We will be using PubMed_20k_RCT_numbers_replaced_with_at_sign.
Creating an NLP model to classify abstract sentences into objective, methods , results, etc. Its mainly for those research papers that do not have a structured abstracts.

Making a baseline (TF-IDF classifier)
Deep models with different combinations of: token embeddings, character embeddings, pretrained embeddings, positional embeddings.
Building a multimodal model.

Model 0: TF_IDF Multinomial Naive Bayes

We create Scikit-Learn pipeline which uses TfidfVectorizer class to convert our abstract sentences to numbers using the TF-IDF algo and then use MultinomialNB to classify the sentences.

Model 1: Conv1D with token embeddings



Model 2: Feature extraction with pre-trained token embeddings

Model 3: Conv1D with character embeddings

Model 4: Combining pre-trained token embeddings + character embeddings (hybrid embedding layer)

Model 5: Transfer Learning with pre-trained token embeddings + character embeddings + positional embeddings
