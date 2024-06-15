## Twitter Joke Bot

This Python script posts a programmer joke to Twitter every week. It uses the Twitter API for authentication and posting, ensuring the jokes are posted sequentially without repeating until all jokes have been posted.



### Requirements
- Python 3
- 'requests-oauthlib' library


### Setup 

Step 1: Install the required packages:

    pip install requests requests-oauthlib

Step 2: Set up your Twitter Developer account and create an app to get your consumer_key and consumer_secret.

Step 3: Update the script with your consumer_key and consumer_secret
    
### Usage

#### Authentication

1. The script checks if twitter_tokens.json exists to reuse the saved tokens. If not, it initates the OAuth flow to the access tokens.
2. Follow the printed authorization URL, authorize the app, and input the provided PIN when prompted.
3. The tokens will be saved for future use.

#### Running the Bot

Simply run the script:
    
    python twitter-chatbot.py

The bot will run indefinitely, posting a new code joke every week.
