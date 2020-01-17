# tri_training
This git explores the paper "Tri-Training: Exploiting Unlabeled Data Using Three Classifiers" by Zhou and Li (2005).  http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.487.2431&rep=rep1&type=pdf

Tri-Training is a means to use unlabeled data to train a supervised model. It addresses the case if you have some labeled data, but lots of unlabeled data. This technique allows you to take advantage of the unlabeled data while continuing to use supervised learning algorithm.

Tri-Training was recently presented by Amazon researchers at ICASSP 2019.  https://s3.us-east-2.amazonaws.com/alexapapers/SemiSupervisedAcousticEventDetectionBasedOnTriTraining.pdf

Tri-Training is an example of Co-Training.  And Co-training is more generally categorized as Semi-Supervised learning.

Essentially 3 models are trained using the labeled data.  They vote on the unlabeled data, and where the predictions agree those samples are added to the labeled set.  You then have a larger labeled dataset, re-train, and repeat the process.

The git incldes:
an overview presentation (.ppt)
video walk-through of above presentation

The git does NOT include:
an experiment and/or library applying the technique including Python code.
