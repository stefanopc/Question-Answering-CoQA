# Question-Answering-CoQA

Question Answering tasks with Transformers on the CoQA Conversational Question Answering dataset

<<<<<<< HEAD
Question Answering (QA) is the task of retrievingthe correct answers to questions based on somegiven context or knowledge (e.g. from a giventext in documents). 

A common approach to solvethe problem is based on Transformers, like in thisassignment, where two different QA tasks havebeen performed on the CoQA dataset. 

The CoQA dataset contains about 127k QA pairs, 8k conversationsin 7 diverse domains. In the first task, given atext passage P and a question Q as input, a modelshould output the correct answer. In the secondtask, a model should answer a question given a textpassage P, a question Q and a dialogue history H,i.e. the dialogue from which the question belongs,meaning the sequence of questions and answerspreviously seen by the model in the same text passage.For these purposes, two Seq2Seq (sequence-to-sequence) models were used, consisting of anencoder-decoder pair. In particular, the two definedand trained models were DistilRoBERTa andBERT-tiny which then have been fine-tuned onthree different seeds for three epochs. They areboth variants of pre-trained language models developedby HuggingFace, but differ in terms of their architecture, 
size, and performance. BERT-tinyis a smaller version of the original BERT model,designed to be faster and more lightweight thanthe full-size BERT model. DistilRoBERTa, onthe other hand, is a smaller and faster versionof RoBERTa. DistilRoBERTa has only half thenumber of layers and parameters of the originalRoBERTa model, while keeping most of its performance.
In the end, the evaluation was performedusing the SQuAD F1-score and the results showedthat the model initialized with DistilRoBERTa’sweights has a better performance with respect tothe one with BERT-tiny’s ones.
=======
Question Answering (QA) is the task of retrieving
the correct answers to questions based on some
given context or knowledge (e.g. from a given
text in documents). A common approach to solve
the problem is based on Transformers, like in this
assignment, where two different QA tasks have
been performed on the CoQA dataset. The CoQA
dataset contains about 127k QA pairs, 8k conversations
in 7 diverse domains. In the first task, given a
text passage P and a question Q as input, a model
should output the correct answer. In the second
task, a model should answer a question given a text
passage P, a question Q and a dialogue history H,
i.e. the dialogue from which the question belongs,
meaning the sequence of questions and answers
previously seen by the model in the same text passage.
For these purposes, two Seq2Seq (sequenceto-
sequence) models were used, consisting of an
encoder-decoder pair. In particular, the two defined
and trained models were DistilRoBERTa and
BERT-tiny which then have been fine-tuned on
three different seeds for three epochs. They are
both variants of pre-trained language models developed
by HuggingFace, but differ in terms of their architecture, 
size, and performance. BERT-tiny
is a smaller version of the original BERT model,
designed to be faster and more lightweight than
the full-size BERT model. DistilRoBERTa, on
the other hand, is a smaller and faster version
of RoBERTa. DistilRoBERTa has only half the
number of layers and parameters of the original
RoBERTa model, while keeping most of its performance.
In the end, the evaluation was performed
using the SQuAD F1-score and the results showed
that the model initialized with DistilRoBERTa’s
weights has a better performance with respect to
the one with BERT-tiny’s ones.
>>>>>>> d1da041e06655dd6ba9d56618f3d3e318a34b85c
