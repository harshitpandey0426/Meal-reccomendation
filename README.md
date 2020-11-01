# Meal-reccomendation

PROBLEM STATEMENT:

Meal Recommender System: Based on historical purchases of a buyer and/or his
personal information (age, gender, health conditions etc.), define buyer persona.
When the buyer prepares his current cart, the meal recommendation wizard
could provide him with food choices, i.e. the meal this buyer is most likely to
prepare. And then accordingly he can either directly add the prepared meal to his
cart or add the missing ingredients to his cart.

PROPOSED SOLUTION:-

Part 1: 
Define user persona.
Find similar users based on their historical purchases and personal choices.

• User-Item collaborative filtering can be used to find similarity between users
based on similarity of items purchased by them.

• Personal data like age, gender, location, personal choices (favorite cuisines,
taste buds, allergies, etc.) can be collected from users by user’s consent to
define user persona more efficiently.

• Clustering algorithm can be used to cluster users as per their persona.

• Essential idea behind using user persona is similar users will get similar
recommendations. For this we will use collaborative filtering.

Part 2: Predict item user most likely to buy next

• User-Item matrix as explained above can be used to predict items user most
likely to buy next using deep learning methods.

• Associative rule learning can be used to incorporate more personalized
suggestions.

• Clusters of user personas defined in part 1 will be used to train different deep
learning and/or associative rule learning models so that similar users will get
similar recommendations.

Part 3: Meal recommendation
• Using predicted items user most likely to buy next and current cart items,
recommend most suitable meal using database query using below priority
order.
• Common items > Current cart items > Predicted items
• Suggestion to buy missing ingredients if particular meal is selected by the
user.

TO run execute the following command

python3 run.py
