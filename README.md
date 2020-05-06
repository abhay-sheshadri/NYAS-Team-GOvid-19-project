# Team GOvid-19's Project

This is our implementation of the solution we described in our presentation and summary.  You can read more about the way our project there.  Make sure you are on Ubuntu 18.04 and have Python 3.6 or later.  The main directory contains all of our Rest API, Telegram, and IBM Watson code.  The code for the FactBase can be found in the oracle directory and the code for the Auto-Summarizer can be found in the summarizer directory.
  
## Installation  

Clone our repository onto your computer.  With your terminal, navigate into the directory and do

```
pip3 install -r requirements.txt 
```

to install all the packages neccessary to run our code.  It is recomended that you do this in a virtual environment.

## Running our code

Before starting up the chatbot, go into the `config.py` file and update the variables with the neccessary information.  You can follow this tutorial to get an IBM Watson API key and Assistant ID.

https://developer.ibm.com/tutorials/crisis-communication-chatbot-watson-assistant-webhook-integration-discovery-covid-data/

After doing that, make sure you get a Telegram Bot Token.  Search for BotFather on Telegram and enter the command `/newbot` .  This should guide you through the process of creating a Telegram Bot.  Also, obtain the filepath to the responses.db file in the oracle directory.  Add all of this information to the relevant fields in `config.py` .

Finally, in order to run the chatbot, enter 

```
python3 app.py
```

in your terminal in the main directory.  You will then be able to initiate contact with your Telegram Chabot either from your computer or from a mobile device.  In order to run the Auto-Summarizer code, enter the following commands in your terminal.

```
cd summarizer
python3 summarizer.py
```


