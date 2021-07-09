## Summary
This was a project for the boot camp where I took the perspective of a consultant working for a food company. I used a reddit API to scrape data from r/vegan and r/Cooking, performed natural language processing, and compared the language in the two subreddits.

## Guide to the repo
- Requires nltk and spacy imports for natural language processing
- Do not run the first notebook
- Second and third notebooks run independently with the data in the saved_data folder

## Executive Summary/ Summary for customers

### Problem Statement

Your company has been a leader in the food industry for many years. However, the market for food products is changing, and your market share has been shrinking recently. You know that there is a growing demand for sustainable, organic, or ethically conscious food, and you want to meet it. But breaking into a new market is hard, and you suspect that you need to market these new products differently.


We are able to use new machine learning techniques to explore consumer behavior. You hired us to do this analysis for the behavior of consumers who are not entirely focused on taste and price.


To explore the interests of this new class of consumers, we performed natural language processing and modeling. We identified words that were used by one group of consumers that care about health and ethical values around food, vegans. There is a large and active reddit forum (subreddit) for vegans, r/vegan. We compared the words used in the reddit forum for vegans with the words used by other consumers who are interested in food and cooking. To acheive this, we analyzed the words used in the subreddit r/Cooking.


First, we lemmatized the text to condense various forms of the same word. We modeled the lemmatized text from the title of the posts and the body. To compare the words used in the two forums, we performed classification modeling to predict which of the subreddits the title or body text came from. After trying logistic regression and random forest modeling, we decided to focus on random forest modeling on the body text.


### Conclusions

We found that there were substantial differences in the language used in each forum. Two of the top words that could distinguish the forums were "animal" and "recipe". When exploring the r/vegan subreddit using count vectorizing to find the most commonly used words, we found that the top words in the title posts were value-laden, like "hate" and "peta". We compared the body text for both r/vegan and r/Cooking using count vectorizing. In r/Cooking, top words included "recipe", "sauce", and "chicken", and none of the words were connected to values and emotions. In r/vegan, top words reflected a more conceptual discussion and included "animal", "people", and "think". Considering these results, it is clear that r/vegan is focused on conversation about animal rights and values, and that r/Cooking is focused on conversation about recipes.


From these results, we recommend that you focus on value-laden words when marketing to this different group of consumers.
