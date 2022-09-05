# Political-Content-Identifier
Classifying us centric political posts on reddit.

#### Motivation
Annoyed by US centric news/political posts on reddit.

#### How was dataset generated:
* Mine data using PushShift, Reddit API and BigQuery and merge them.
* Label posts based on the subreddit.
* Extract keywords using TextRank and generate a frequency table.
* Train models using relative frequencies of extracted keywords.
* A simple logistic regression on relative word frequencies is giving ~94% accuracy in classification.


#### How to use
Included a logistic regression model.  
Example: 
```
from classifier import Classifier
Classifier.predict(text)
```
#### TODO
Make a browser plugin.
