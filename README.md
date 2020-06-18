&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;[![Bitcoin](https://media.giphy.com/media/NW4hBBjqMJfOg/giphy.gif)](https://bitcoin.org/en/)

__This is a python script package, bitcoin price notification to get notified for the regular updates of bitcoin price on gmail,telegram,twitter,android sms and IFTTT app notifications. The aim is to push notifications when the price of bitcoin changes at certain time interval, user can specify the time interval. By default time interval and threshold are set to 5 in minutes and $10000 respectively. The user has option to choose out of which of the 5 application they want to recive the notification.__

# DESCRIPTION
__*Bitcoin price is a fickle thing. You never really know where it’s going to be at the end of the day. So, instead of constantly checking various sites for the latest updates, let’s make a Python app to do the work for you.*__

<ul>
  <li>We’re going to use the popular automation website IFTTT.</li>
  <li>We’re going to create 4 IFTTT applets and 1 gmail service:</li>
  <li>One for emergency notification when Bitcoin price falls under a certain threshold and the emergency notification plus normal price update will send to any app of the users choice out of the 5 option.</li>
  <li>These will be triggered by our Python app which will consume the data from the Coinmarketcap API.</li>
  <li>An IFTTT applet is composed of two parts: a trigger and an action.</li>
  <li>Trigger will be a webhook service provided by IFTTT.</li>
  <li>Our Python app will make an HTTP request to the webhook URL which will trigger an action. Now, this is the fun part—the action could be almost anything you want. IFTTT offers a multitude of actions like sending an email, updating a Google Spreadsheet and even calling your phone</li>
</ul>

## Prerequisite

Must have one of the following app installed and/or must join or follow one of the following accounts:
  - IFTTT App
  - Telegram App and must join this channel click on the image to join <a href="https://t.me/mybitcoinproject"> <img src="https://media2.giphy.com/media/1gdue30RkC7TPsefAP/giphy.gif" width="80"/></a> 
  - Twitter App and must follow this account click on the image to follow <a href="https://twitter.com/AtanuPa02151991"> <img src="https://media.giphy.com/media/M9O6ePwNJ58UMF1Rvq/giphy.gif" width="80" /></a> 
  - An email account
  - An contact number to recive sms
  
#### Github Link : https://github.com/Atanu-Paul-au6/bitcoin_price_alert_app/tree/v0.6
#### Pypi Link   : https://pypi.org/project/bitcoin-price-alert-app/0.6/

### Tech

Bitcoin price notifier was made use the follwing :

* python.org - as the core developing language
* github.com - for version control
* pypi.org - for distribution.
* ifttt.com - for notification automation services

### Installation

Bitcoin price alert application requires [Python 3](https://python.org/) v3+ to run.

Install all the following for running the app smoothly:

1 Installation for PIP on windows run the following command in your terminal
```sh
pip install
```
2 Then install the app dependency, this app only requires 1 dependency, to install it run the following commond in you terminal

```sh
pip install requests
```
3 Install bitcoin_price_alert_app package/module from PIP, to do that run the following command on terminal

```sh
pip install bitcoin-price-alert-app==0.6
```
__IF THE APP DOES NOT INSTALL OR RUN PROPERLY AFTER STEP 3 THEN GO TO [THIS LINK](https://github.com/Atanu-Paul-au6/bitcoin_price_alert_app/archive/v0.6.2.tar.gz) TO DOWNLOAD THE ZIP FILE.__

### ALTERNATE STEP TO RUN THE APP AFTER DOWNLOADING THE ZIP FILE

* UNZIP THE FILE 
* OPEN YOUR CMD OR TERMINAL 
* GO TO THE FOLDER PATH OF THE UNZIPPED FOLDER EXAMPLE 'C:\Users\Desktop\bitcoin_price_alert_app-0.5\bitcoin_price_alert_app'


TYPE THE FOLLOWING COMMAND TO SEE HELP MENU
```
python bitcoin_price_notifier.py --help
```
you will see a menu like this
```

Welcome To Bitcoin Price Alert App
usage: bitcoin_alert_prototype4.py [-h] [-a alert_amount] [-t time_interval] [-l log_lenght] -d destination_app

Bitcoin Price Alert App.

optional arguments:
  -h, --help            show this help message and exit
  -a alert_amount, --alert_amount alert_amount
                        The price of 1 bitcoin when an emergency alert will be sent. Default is 7,18,715 INR
  -t time_interval, --time_interval time_interval
                        The time interval in minutes after which the lastest value of bitcoin will be fetched. Defalut is 5 minutes
  -l log_lenght, --log_lenght log_lenght
                        The number of records/entries you want example 5 entries at 5 minutes interval. Default length is 2
  -d destination_app, --destination_app destination_app
                        The mobile application on which you want to recive alert. Destination app options are (1) IFTTT app, (2) Telegram
                        App, (3) Email, (4) Twitter, (5) SMS

This app gives the value of 1 BTC in INR. Destination (-d) must be provided. To recive notification on IFTTT install IFTTT mobile app. To
recive notification on Telegram install Telegram mobile app and join this channel https://t.me/mybitcoinproject . Prerequisite : MUST HAVE A
IFTTT APP AND TELEGRAM APP INSTALLED TO RECIVE NOTIFICATION ALSO MUST JOIN THE TELEGRAM Bit_Coin CHANNEL TO RECIVE MESSAGES. PRESS Ctrl+C to
terminate the app
```
to run the app type the following command
```
python bitcoin_price_notifier.py -a 5000 -t 3 -l 5 -d email
```
* -a : alert limt amount in INR
* -t : time interval in minutes
* -l : the number of records needed
* -d : the destination app like email or telegram etc __THIS MUST BE PROVIDED__

License
----

MIT

**Free Software, Hell Yeah!**

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;![thank_you](https://media.giphy.com/media/95P1vO6r7rsk0/200_d.gif)

##### Author: Atanu Paul.
