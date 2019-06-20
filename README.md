# dl-final-project-jenny-joy
This git repo contains work for Findal Project of MSDS631 Deep Learning with Pytorch 

# Teammates
Jenny Kong, Joy Qi

# Project: Quora Insincere Question Classification  
Detect toxic content to improve online conversations

# Objectives
For Quora, the goal to put up this competition is to help them detect toxic content on Quora.com platform and improve the quality of online conversation environment. For the project, the goal is to predict whether a question asked on Quora is insincere or not. Quora also provide definition of insincere in the competition description. An insincere question is defined as a question intended to make a statement rather than look for helpful answers. Some characteristics that can signify that a question is insincere:

- Has a non-neutraltone
  - Has an exaggerated tone to underscorea point about a group of people
  - Is rhetorical and meant to imply a statement about a group of people
- Is disparaging or inflammatory
  - Suggests a discriminatory idea against a protected class of people, or seeks confirmation of a stereotype
  - Makes disparaging attacks/insults against a specific person or group of people
  - Basedonanoutlandishpremiseaboutagroupofpeople
  - Disparages against a characteristic that is not fixable and not measurable
- Isn'tgroundedinreality
  - Based on false information,or contains absurd assumptions
- Uses sexual content (incest, bestiality, pedophilia) for shock value, and not to seek genuine answers

# Data
The data comes from a Kaggle dataset provided by Quora. The features are the text from the questions and the labels will reflect whether it is insincere or not. To date, Quora has employed both machine learning and manual review to address this problem.  

The training data includes the question that was asked, and whether it was identified as insincere (`target = 1`). The ground-truth labels contain some amount of noise: they are not guaranteed to be perfect.   

Note that the distribution of questions in the dataset should not be taken to be representative of the distribution of questions asked on Quora. This is, in part, because of the combination of sampling procedures and sanitization measures that have been applied to the final dataset.  

# Approach
## First Model: [LSTM-CNN](https://github.com/DeepLearningWithPytorch/dl-final-project-jenny-joy/blob/master/1_LSTM.ipynb)
Our first model, we used LSTM

