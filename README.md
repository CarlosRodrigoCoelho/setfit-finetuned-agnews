# setfit-finetuned-agnews

# How SetFit works
SetFit uses rich text embeddings which removes the need for prompts (which also means more reliability and less variability in the predicted results - solves bottleneck 2), and is a very efficient framework for few-shot learning tasks requiring a much-labeled training data compared to the existing methods for the same tasks.‍

The diagram below compares SetFit with the other methods for classification using few-shot learning. SetFit requires significantly less number of train samples and still achieves better accuracy compared to the other techniques for few-shot learning. ‍

SetFit using only 8 labeled examples per class on the Customer Reviews (CR) sentiment dataset gives results that are comparable to those of fine-tuning RoBERTa Large on the full training set of three thousand examples! It’s important to note that the fine-tuned RoBERTa is 3 times larger than the SetFit model used. Along with this, the uncertainty bands demonstrate better reliability (less uncertainty in terms of variability) in SetFit’s results. All of this with comparatively much smaller and cost-effective models!


# Compared to other few-shot learning methods, SetFit has several unique features:

🗣 No prompts or verbalisers: Current techniques for few-shot fine-tuning require handcrafted prompts or verbalisers to convert examples into a format that's suitable for the underlying language model. SetFit dispenses with prompts altogether by generating rich embeddings directly from a small number of labeled text examples.

🏎 Fast to train: SetFit doesn't require large-scale models like T0 or GPT-3 to achieve high accuracy. As a result, it is typically an order of magnitude (or more) faster to train and run inference with.

🌎 Multilingual support: SetFit can be used with any Sentence Transformer on the Hub, which means you can classify text in multiple languages by simply fine-tuning a multilingual checkpoint.

# Installing SetFit
Using Collab:

``` !pip install setfit``` 
