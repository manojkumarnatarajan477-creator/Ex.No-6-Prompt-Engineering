Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

Aim:  

Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools.

Explanation:

Develop a python code that integrates multiple AI tool by interacting with their APIs.
Compare outputs from different APIs.
Analyze the response and the Output.

The aim is to understand how to request help from AI tools for tasks like writing Python code, integrating with APIs, comparing outputs, and generating actionable insights.

Program:

```python
POSITIVE ANALYSIS
from nltk.sentiment import SentimentIntensityAnalyzer
import nltk

nltk.download('vader_lexicon')

# Simulated AI-generated text
generated_text = "This smartphone offers outstanding battery life and an intelligent AI camera that captures stunning photos. i want this into negative statement"

print("Generated Review:\n")
print(generated_text)

# Sentiment analysis
sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)

print("\nSentiment Analysis:")
print(sentiment)

# Insight generation
if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")
```
```python
NEGATIVE ANALYSIS 

from nltk.sentiment import SentimentIntensityAnalyzer
import nltk

nltk.download('vader_lexicon')

# Simulated AI-generated text
generated_text = "This smartphone does not offer outstanding battery life and does not have an intelligent AI camera that captures stunning photos."

print("Generated Review:\n")
print(generated_text)

# Sentiment analysis
sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)

print("\nSentiment Analysis:")
print(sentiment)

# Insight generation
if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")

```
Result:


Positive:
<img width="1779" height="441" alt="POSITIVE REVIEW" src="https://github.com/user-attachments/assets/b519d86a-d74d-417f-afeb-42740bb4ebcb" />
Negative:
<img width="1664" height="348" alt="NEGATIVE REVIEW" src="https://github.com/user-attachments/assets/3bed4120-b888-4162-a14a-bf99d1e1c79f" />


