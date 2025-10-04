AI-Powered Digital Marketing LLM

An end-to-end project that uses Twitter API + Google Gemini AI + Flask to analyze tweets, generate optimized content, and predict engagement.
This system helps brands, startups, and influencers maximize their reach with data-driven, AI-optimized tweets.

Problem Statement
Social media engagement is unpredictable.
Current tools only show metrics (likes, retweets, impressions) without insights.
A/B testing requires posting multiple tweets publicly, wasting time.
Manual analysis of sentiment and engagement is slow and inconsistent.
No system exists to predict Marketing Post  performance before posting.

  ✅ Solution
  Our solution is an AI-powered Twitter Engagement Optimizer that:
  Fetches and analyzes tweets using Tweepy + Gemini AI.
  Performs sentiment & keyword analysis for deeper insights.
  Identifies top 5 performing tweets by engagement type.
  Generates new AI-based tweets inspired by top performers.  
  Runs virtual A/B testing (Tweet A vs Tweet B) without publishing.
  Predicts which tweet will perform better with explanation.
  Exposes everything via a Flask API with a simple index.html interface.

⚙️ Tech Stack
Python 🐍
Tweepy → Fetch tweets from Twitter API
Google Gemini AI → Sentiment analysis, tweet generation, prediction
Pandas → Data analysis & filtering
Flask → REST API for tweet generation & comparison
HTML + JS (index.html) → Simple frontend for demo
JSON → Store and exchange tweet data

📂 Project Structure
├── extract_tweets.py       # Fetch tweets from Twitter API and save to extracted_tweets.json  
├── extracted_tweets.json   # Raw tweets fetched from Twitter  
├── run_prompt.py           # Gemini AI helper functions (analysis, tweet creation, prediction)  
├── sentiment_tweets.py     # Analyzes tweets with Gemini (sentiment, engagement, keywords) → analyzed_tweets.json  
├── analyzed_tweets.json    # Processed tweet data with AI insights  
├── createtweets.py         # Selects top tweets, generates new AI tweets, compares A vs B  
├── api.py                  # Flask API exposing /generate endpoint  
├── index.html              # Simple frontend for interacting with Flask API  
└── README.md               # Project documentation  


🔄 Workflow
 Fetch Tweets (extract_tweets.py)

 Uses Tweepy to fetch tweets from a given user.

 Stores them in extracted_tweets.json.

 Analyze Tweets (sentiment_tweets.py)

Sends tweets + metrics to Gemini AI.

Extracts sentiment, keywords, target audience, engagement score.

Saves results in analyzed_tweets.json.

Select Top Tweets & Generate New Ones (createtweets.py)

Identifies top 5 tweets based on engagement.

AI generates two new candidate tweets (Tweet A & Tweet B).

Compares them against best-performing tweets.

Prediction & Comparison

AI decides which tweet will perform better.

Provides explanation (tone, structure, relativeness).

Flask API (api.py)

Endpoint: /generate?prompt=YourText

Returns Tweet A, Tweet B, comparison, prediction, and explanation.

Frontend (index.html)
A simple UI to interact with the Flask API.
Users can enter prompts and see AI-generated results.



🔮 Future Enhancements
  Real-time analytics dashboard with charts.
  Multi-platform support (Instagram, LinkedIn).
  Multilingual tweet generation.
  Advanced trend detection using live feeds.

  Contributors 
  1. Raghav Devgan 
  2. Ansh gill
  3. kanan 
  4. Prithvi Raj Singh Chouhan
  5. Manbir Singh
