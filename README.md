# Ad-placement-optimization-RL
Ad placement in a particular website using reinforcement learning(Model-based and Model Free Methods)
Placement of ads on website is the primary problem for companies that operate on ad revenue. The position where the ad is placed plays pivotal role on whether or not the ad will be clicked. Here we have the following choices:

Place them randomly, or
Place the ad on the same position
The problem with placing the ad on the same position is the user, after a certain time, will start ignoring the space since he's used to seeing ad at the place, he will end up ignoring that particular position hereafter. Hence, this will reduce the number of clicks on ads. The problem with the former option, placing them randomly, is it wouldn't take optimal positions into consideration. For instance, text beside images are viewed higher number of times than those text which are placed at a distance. It is infeasible to go through every website and repeat the procedure.

Solution: Reinforcement Learning

Using Reinforcement Learning we can approximate the human behavior.

Why Reinforcement Learning?
We cannot use traditional Machine Learning here, since it requires:

Huge data
Features
Tuning of many hyperparameters
And we neither have huge data, nor features. The only data we have is the position of the banner/ad and whether or not it was clicked. We will use this dataset from Kaggle: https://www.kaggle.com/akram24/ads-ctr-optimisation. We will solve this problem using both model-based (Policy iteration) and model-free methods(Q-Learning & Monte-Carlo). We'll simplify some assumptions for model-based technique.

Notebook Layout
MDP environment - Understanding the dataset
Random Policy - placing the ads randomly on different webpages
Max policy - placing the ad where it is clicked maximum number of times
Model-based Method - Policy Iteration
Model-free Method - Q-learning & Monte Carlo
