# tri_training
This git explores the paper "Tri-Training: Exploiting Unlabeled Data Using Three Classifiers" by Zhou and Li (2005).  http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.487.2431&rep=rep1&type=pdf

Tri-Training is a means to use unlabeled data when training a supervised model. It addresses the case when only a small amount of labeled data is available, but there's lots of unlabeled data. This technique allows you to use the unlabeled data to train a model using a supervised learning algorithm.

The procedure is summarized as follows:  Three models are trained using the labeled data. They then make predictions on the unlabeled data, and where the predictions agree those samples are added to the labeled set. You thus have a larger labeled dataset.  You then re-train and repeat the process.

Tri-Training is an example of Co-Training. Co-training is more generally categorized as Semi-Supervised learning.

An example of use was at Amazon.  Researchers there applied (or at least researched the application of) for the Wake-Word.  This was presented at ICASSP 2019.  https://s3.us-east-2.amazonaws.com/alexapapers/SemiSupervisedAcousticEventDetectionBasedOnTriTraining.pdf

The git incldes:
an overview presentation (.ppt)
video walk-through of above presentation

The git does NOT include:
an experiment and/or library applying the technique including Python code.
