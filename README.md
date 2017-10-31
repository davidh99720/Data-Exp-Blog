# Data-Exp-Blog
My path to handle Data Problems

Capstone Proposal

My proposed project is "Healthy Yummy Recommender".

People will eat out very frequently. They may feel confused about what to eat next.
Giving them a suggestion of well-rated restaurant will be appreciated.
But there are still a lot of options that make them hard to make a decision.
My innovative idea here is healthy! We will give them a list of healthy eat-out suggestions
and detailed healthy eating analysis as a reference.

Based on the Yelp 2017 Challenge Database, we first group businesses in different cities and order the cities
by descending aggregated total reviews so that we can see that there are 963 different cities and which city is most yelp-active.
Then our analysis will start from the top 10 cites which each has at least 100,000 reviews for open businesses.

First, using collaborative filtering algorithm, based on reviews and ratings from all customers who have tried the restaurant and the review and ratings from the customer who need a recommendation,
we can give a high rating recommendation list of restaurant that this customer would like to appreciate.

Then, from the high rating recommendation list, we use the other personal data and review data
on yelp (and other info we could crawl from the internet) for this customer to analyze his healthy condition
and decide what kind of food this customer need to eat to make his/her diet balanced and make him/her healthier.
This may sound very challenging to analyze on the following problems:
1) Define what is a healthy/balanced diet plan.
2) Identify the eating habits and health condition of a given customer
3) Identify healthy food for a given customer in a given restaurant.

Solutions for the hard problems above:
1) This can be done in several views, including nutrition facts of food, oil amount used in food, the category of ingredients in food, etc..
2) For eating habits, we can use yelp review data (by keywords filtering) and pictures data in the yelp database of the customer,
  (as well as his/her Facebook data that we can find on the internet if it is available).
  This process of picture data will involve picture recognition
  and we can use neural network model trained by pictures data in internet and picture data in yelp database.
3) Compare the above two results for a healthy diet and this person's eating habit,
   with control factors determined by the health condition of the customer (including age, gender, review history etc.),
   to determine the suggested category of food for this customer.
   Then match this category data with available high rating restaurant (including its menu and review data) nearby to give recommendations.

