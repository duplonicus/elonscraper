# Info

This script was originally created to gain an advantage in crypto trading but can be used for other purposes. For example, logging all of an account's tweets in case of account deletion. It loops every 5 seconds and checks the last tweet of the specified account for keywords, photo changes, and banner changes. If a keyword is detected or an image changes, it plays a sound. It opens a new tab in the default browser to new tweets and images. Results are displayed in the console, sent to Discord, logged to twitter.log, and a PostgreSQL database (optional). Twitter API key not required.

# Setup for Windows

1. Install Python3

2. Run "pip install -r requirement.txt"

3. Rename new_secrets.py to secrets.py and fill in a Discord webhook URL

Complete the rest of the steps if a database is desired

4. Install PostgreSQL and create a database

5. Rename new_db.ini to db.ini and fill in the database connection info

# How to use

Run "python3 twitter.py" to scrape the default account set in the argument parser definition

Run "python3 twitter.py username" to scrape someone else.
Example: "python3 twitter.py michaeljburry"

The keywords can be modified within twitter.py and are seperated by the | symbol

Turn functionality on/off in the Options section

# Screenshots

![Screenshot](https://i.imgur.com/KvDBJRf.png)

![Screenshot](https://i.imgur.com/0SIqCVO.png)

![Screenshot](https://i.imgur.com/lvAWToB.png)