## By Charles Alba, Drs. Lukasz Walasek, Mikhail Spektor


Cite as: Alba, C., Walasek, L., Spektor M. (2024) "Attention-driven imitation in consumer reviews". Decision (Special Issue on interface between ML, AI and JDM research)

### Abstract summary:
How do reviewers decide what to write about? How much do reviews written by others influence one’s own contribution. We predicted that reviews will be more semantically similar to the most successful, salient, and readily accessible reviews written by others. To investigate this hypothesis, we extracted over 3 million reviews from a ``STEAM``. We reversed-engineer and traced the reviews that were displayed at the time to each reviewer at the time each review was being composed. Using word embeddings from ``fast-text``, we quantified the ``cosine similarity`` between a given review and other reviews that were visible (or not) to a user. We found that reviewers imitate the most helpful reviews written by others, especially those that are visually salient. At the same time, reviewers avoid imitating content of the most recent (and not necessarily highly rated) reviews, even if these reviews are salient at the time when they compose their review. Our findings suggest that the default sorting and display format of reviews on online platforms will have a pronounced effect on the style and content of new reviews.


### Code works in the following sequential order:

#### 1. Data Scrapping

In this stage we scrapped the data from STEAM. Data was scrapped and gathered courtesy of STEAM API. Please refer and abide to their terms of use at all times. Refer to their terms of use here: https://steamcommunity.com/dev/apiterms

#### 2. Validation of review sorting algorithms

As mentioned in the abstract, we aimed to trace the reviews that would have been made visible to each gamer when he/she was writing his/her review. We do not know exactly how STEAMs algorithm decides what reviews at displayed to each gamer when they write their reviews, but we can reverse-engineer and hypothesize them. So we tested and validated our reversed-engineered hypothesized algorithm. 

#### 3. Data Wrangling

Having tested and validated our hypothesized algorithm, we then trace what each reviewer will have seen when writing his/her own review. 

#### 4. Text Mining

Here we perform text pre-processing, and implement fast-text embeddings with cosine-similarity matrices to determine how close each review is to the reviews that the reviewer will have seen. 

#### 5. Statistical Analysis

Performed statistical analysis to test our effect sizes. 







