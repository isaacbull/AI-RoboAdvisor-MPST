# IA-applied-to-finance-RoboAdvisor

Robotic advisors create and manage investment portfolios through automated processes. The objective is to create a personalized investment portfolio for each client, which takes into account the preferences of each user, their knowledge, their experience, their objectives and other issues that determine their risk profile, in order to separate them from the assembly process. of your investment portfolio and its rebalancing over time. These strategies used by RoboAdvisors are usually classified as Passive strategies, which do not have the objective of trying to obtain a higher yield than the market, but rather to replicate it through indices.
This project aims to create an initial model of Robo Advisor in order to demonstrate its operation on a smaller scale.


# How does it work?
For this project, we proceeded to build 3 possible risk profiles for the user, classified as "Conservative", "Moderate" and "Aggressive". It is determined by answering 5 questions from the user, to determine the degree of risk aversion of him. Once this is obtained, the RoboAdvisor proceeds to recommend one of three possible portfolios created

# How is the portfolio selection made?
With respect to the method used for the selection of portfolios, the one proposed by Harry Markowitz known as "Modern Portfolio Selection Theory" was obtained. The reason for its choice lies in a survey that indicates that 40% of the systems of this type in the world use it, placing it as the main option.
For portfolio selection, 10.000 portfolios were created with random weights, each with a certain return and volatility. Subsequently, the 3 portfolios that presented a higher return for a given level of volatility were selected, by using the Sharpe index.

# What ML algorithm is used?
In the first instance, a comparison was made between 3 classification models, known as "Decision Tree", "Support Vector Machine" and "Linear Discrimination" to determine which presented the best results obtained through the Confusion Matrix. Both Decision Tree and Vector Support Machine presented 100% precision, recall and accuracy in their results, but the former was chosen because it was more robust and easier to interpret its results to a public not immersed in the topic.It was trained with a fictitious database composed of 500 users.