# Slack-Bots
This repository contains various Slack Bots for various purposes and information sharing in DSC TIET-GS Slack Channel

## Current goals for the project are:

3 different chat bots to be developed,

    1. For Hacathons, primarily from telegram. 
    2. Medium/ technical articles
    3. Recruitment of Hacathon teams

3 stages for the Bots are:

    1. Scraping using metadata
    2. Using Regex
    3. Applying NLP

## Runtime Instructions 
### Telegram Bot

	1. 'Talk' to 'BotFather' in the Telegram app to create a new bot
	2. Use '/setprivacy' and 'Disable'. Now your bot can read all messages in the group
	3. Get your bot's token for BotFather using '/token' (eg: 888####:AA#############)
	4. Add you bot in the group chat and get chat id using the following steps:
		Assume the bot name is my_bot.

		1- Add the bot to the group.
		Go to the group, click on group name, click on Add members, in the searchbox search for your bot like this: @my_bot, select your bot and click add.

		2- Send a dummy message to the bot.
		You can use this example: /my_id @my_bot

		3- Go to following url: https://api.telegram.org/botXXX:YYYY/getUpdates
		replace XXX:YYYY with your bot token

		4- Look for "chat":{"id":-zzzzzzzzzz,
		-zzzzzzzzzz is your chat id (with the negative sign).
	5. Add your Chat ID and bot Token to Telegram/scrapper.py