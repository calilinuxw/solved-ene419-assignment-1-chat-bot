Download Link: https://assignmentchef.com/product/solved-ene419-assignment-1-chat-bot
<br>
Programming Assignment (Application layer)

You will create a chat-bot program that can collect Bit Coin prices from major exchanges and notify a user. Your program should be named as ‘coin-studentid.py’. It consists of following parts:

<ol>

 <li>Requesting Bit Coin (BTC) prices every starting minute exactly (e.g., 13:01:00, 13:02:00, and so on) via http request api from cryptocompare.com or similar services that you can find on your own.</li>

 <li>Sending message to you from your telegram chat-bot.</li>

 <li>Receiving command from your telegram chat-bot.</li>

</ol>

**Part A. Request the following Bit Coin prices: Bitfinex in USD and EUR. Please refer to crytocompare api instruction for single or multi symbol(s) price: (if you want, you can use other similar api services, like Upbit or Bithumb for KRW price.)

https://min-api.cryptocompare.com/documentation




To request data, please refer to the following instruction:

http://docs.python-requests.org/en/master/user/quickstart/

Its request should be made every starting minute continuously. Please refer to the following instruction. You can find more APS scheduler examples on Google. Alternatively, you can use crontab or threading timer.

http://apscheduler.readthedocs.io/en/latest/userguide.html

The collected information should be stored to csv file. It is similar to the following:

$more price.csv

Date, BTC-USD, BTC-EUR

2021-08-30-00:00:00, 4567.8, 3000.0

2021-08-30-00:01:00, 4572.7, 3000.0

2021-08-30-00:02:00, 4582.7, 3000.0




…ß

**Part B. Send text message to your telegram using chat-bot. To do this, create your telegram chat-bot and send pricing up/down information every minute as well.

Telegram chat-bot instruction: (please refer to BotFather)

https://core.telegram.org/bots

Recommended chat-bot api:

http://telepot.readthedocs.io/en/latest/

You need to create ‘TOKEN’ in order to send a message. You can do this manually for now. Read these instructions carefully. And your telegram chat window should be similar to the following (please ignore ‘profit’ field in this example):




**Part C. Add a “/stop” command if you want to stop receiving these messages. You don’t need “/start” button (you can assume that you can receive these messages when starting your program). This means you should be able to type “/stop” command in your telegram window and your program must receive this and act correspondingly. We can discuss this in class.

NOTE:

<ol>

 <li>Python is recommended. If you are willing to use other programming languages, that’s fine too. But use it at your own risk.</li>

 <li>Any platform of your choice is fine, but I’d like to see many Linux as possible (e.g., Ubuntu).</li>

 <li>If you want, you can use Kakao Talk and others instead of telegram.</li>

</ol>