# DiscordConvBot
Python-based bot for premade conversations in discord

Requirements:
Python >3.10;
requests;
windows-curses;

## Description

An application to send out discord messages in preset sequence as a dialogue. For anti-spam testing and server administration training.

## Installation and startup
1. Download python, most importantly include PATH variables when [installing](https://tutorial.djangogirls.org/en/python_installation/)
2. Download main.py and disSendClass.py from github and put them in the same folder.
3. If python is installed correctly, write commands "pip install windows-curses" and "pip install requests" in cmd.
4. Go to the bot folder via cmd and type "python main.py"

## Usage
- WARNING it is desirable to run cmd in full screen to avoid unnecessary errors.
- fill in the cfg file for each conversation according to the example, it is possible to specify the execution queue with a SPACE.
- use the up and down arrows to navigate between conversations


## CFG file example 
*(follow this specific order, save in .cfg format, make sure there are no spaces or other extra characters at the end of the lines)*

- txt file name     (text file name with its extension)

- token 1

- token 2

(Discord tokens are obtained by entering Discord via browser and following these instructions F12 -> Network -> F5 (wait for reboot) -> science -> Headers -> authorization copy the value, you can close the browser window)
                  
- chat_id           (ID of the chat in which the conversation will take place, go through your browser to Discord and to the desired chat, in the address line it is the last set of digits.)

- delay             (delay between messages in seconds, I advise you to set it to 30, the delay between messages in discord it will take into account itself.)

- reaction to chat stop (what the bot should do if chat is paused, any number = wait in seconds for the specified time; -1 = pause itself; leave blank = do nothing)
- number of mistakes per message (number of errors made in a message, ex. 1 = one error per message, 0-2 = zero to two errors per message.)

*(specify what to use after the end of sending the last message in the dialog with a comma, example: token 1, token 2.)*
