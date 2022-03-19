# mememachine
A telegram bot that sends memes, jokes and other fun things from reddit. the bot deletes messages it sends after some time in order to prevent cluttering the group. A logger group is required where the bot sends log messages, updates and errors when encountered, it also prevents the deletion handler thread from being closed.

uses 
Praw - to retrieve content from reddit
psycopg2 - to store information of each message sent out and all command messages received so they can be deleted later on
datetime - to keep track of time and delete messages sent after some time
threading - to have two threads- one to handle deleting older messages, another to handle commands and messages
telegram - to handle bot messages 
random - to randomly select memes abd jokes to send
time - to sleep the deletor thread

the bot code is currently hosted by me on heroku, with the username @simpmachinebot on telegram.

# setup 

the extra files are created to host it on heroku, other services file requirements may vary. 

1 - add all the tokens in the tokens.py file. the API_KEY is the api key of your telegram bot as given by botfather, the ID is chat id of your logget group.
2 - create a heroku account and connet the repo to it
3 - run and enjoy
