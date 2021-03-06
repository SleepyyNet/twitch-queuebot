# twitch-queuebot

## About

This is a simple bot for handling queues in twitch chat. Subs have priority over regulars in the queue.

The bot is coded and tested in Python 3.4

## Download

Just clone this git repo!

## Install

The bot depends on one Python dependency, namely the library called `irc` (https://bitbucket.org/jaraco/irc).

    [sudo] pip install irc
    
## Run

Before you run the bot, rename `config.example.ini` to `config.ini` and edit it with your preferred settings.

Once you have installed the dependencies and fixed the config file, run the bot by executing the following command:

`python main.py`

## Commands
Command                     | Description
--------------------------- | ----------------------
!queue join                 | join the queue (only if it's active)
!queue remove USERNAME      | Remove USERNAME from the queue
!queue add USERNAME         | Add USERNAME to the queue
!queue enable               | Start the queue
!queue disable              | Stop the queue
!queue clear                | Clear all participants from the queue
!queue list                 | List the first ~15 participants in the queue.
!queue winner               | Remove the person who's first in the queue and print his name.
!queue pos [USERNAME]       | Check the position of a user. If no username is given, check yourself.
