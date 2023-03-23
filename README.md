Apologies for contacting you this way - I could not see any means of reaching out to you otherwise.

We are planning to launch a new product under the name Norsk, which will have a significant open source element to it and we would love to be able to host this under github.com/norsk.  I see that you own that username, but the account appears to be dormant, the only (visible) activity being to fork this repo some years ago.

We would be very grateful if you would consider changing your username so that it could be picked up by a considerably more active account.

With kind regards,

Adrian Roe

# Cloud Telegram Bot

-1. Find @BotFather in Telegram and send them "/newbot" and name of your new bot after that

0. Remember token of your bot
1. Download this repo as ZIP
2. Unpack
3. Go inside "cloud-telegram-bot-master", select all files and folders inside and archive. 
It will help to avoid python package names limitations.
4. Go to https://my.selectel.ru -> Cloud Platform -> Functions, tap "Create function"
5. Upload ZIP file 
6. Set "Path to the file" to "bot/tele_bot"
7. Set "Function to execute" to "main"
8. Add item to "Environment variables", name it "TOKEN" and insert token of your bot as value.
9. Click "Save and deploy"
10. Mark "HTTP-request" as public
11. Find @SelectelServerless_bot in Telegram (it has exactly same code which you see in github)
12. To register webhook on your cloud function, send them `/setwebhook <you bot token> <public URL of your function>`
13. After that `/getwebhook <you bot token>`. Here you can see status of how Telegram connects with your cloud function

Done. Your bot will receive messages and answer to you.

P.S.: Send sticker to the bot to get a code to use in your bot.
