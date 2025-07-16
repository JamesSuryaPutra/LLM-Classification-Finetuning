# LLM Classification Finetuning

# Overview
This competition challenges you to predict which responses users will prefer in a head-to-head battle between chatbots powered by large language models (LLMs). You'll be given a dataset of conversations from the Chatbot Arena, where different LLMs generate answers to user prompts. By developing a winning machine learning model, you'll help improve how chatbots interact with humans and ensure they better align with human preferences.

# Description
Large language models (LLMs) are rapidly entering our lives, but ensuring their responses resonate with users is critical for successful interaction. This competition presents a unique opportunity to tackle this challenge with real-world data and help us bridge the gap between LLM capability and human preference.

We utilized a large dataset collected from Chatbot Arena, where users chat with two anonymous LLMs and choose the answer they prefer. Your task in this competition is to predict which response a user will prefer in these head-to-head battles.

This challenge aligns with the concept of "reward models" or "preference models" in reinforcement learning from human feedback (RLHF). Previous research has identified limitations in directly prompting an existing LLM for preference predictions. These limitations often stem from biases such as favoring responses presented first (position bias), being overly verbose (verbosity bias), or exhibiting self-promotion (self-enhancement bias).

We encourage you to explore various machine-learning techniques to build a model that can effectively predict user preferences. Your work will be instrumental in developing LLMs that can tailor responses to individual user preferences, ultimately leading to more user-friendly and widely accepted AI-powered conversation systems.

This competition challenges you to predict which responses users will prefer in a head-to-head battle between chatbots powered by large language models (LLMs).

# How Kaggle's Competition Work
## 1. Join the Competition
Read about the challenge description (see Code Requirements for more details), accept the Competition Rules and gain access to the competition dataset.
## 2. Get to Work
Create a Kaggle Notebook, import the competition data, build models, and generate a prediction file.
## 3. Make a Submission
Submit your notebook to the competition!
## 4. Check the Leaderboard
See how your model ranks against other Kagglers on our leaderboard.
## 5. Improve Your Score
Check out the discussion forum to find lots of tutorials and insights from other competitors.

# Evaluation
Submissions are evaluated on the log loss between the predicted probabilities and the ground truth values (with "eps=auto").

# Submission File
For each id in the test set, you must predict the probability for each target class. The file should contain a header and have the following format:

id,winner_model_a,winner_model_b,winner_tie
 136060,0.33,0,33,0.33
 211333,0.33,0,33,0.33
 1233961,0.33,0,33,0.33
 etc
