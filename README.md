
## High-performance sniping bot 

# Table of contents
* [Important Notes](#IMPORTANT-NOTES-BEFORE-RUNNING-THE-BOT)
* [Advanced Bot](#NOW-LAUNCH-ADVANCED-BOT)
* [Setup](#HOW-TO-RUN)
* [TroubleShoot](#TROUBLESHOOT)

### Bot supports Kucoin as well as MATIC

## IMPORTANT NOTES BEFORE RUNNING THE BOT


### What's the feature
1 ) Buy
2 ) Sell
3 ) Sell with target profit & custom amount
4 ) Approval/Confirmation
5 ) Snipe before liquidity added 
6 ) Custom slippage, gwei , gas limit
7 ) Some mini customizations
8 ) Spam Buy
9 ) Degen Scanner : https://t.me/degenScanner
10 ) All trx using BNB instead WBNB
11 ) support unicrypt and dxsale
12 ) support matic network


## HOW TO RUN
1. clone this repository
2. $ npm install
3. copy your <code>.env.example</code> to <code>.env</code>
4. set up your <code>.env</code> to with this explanation : 

```
WBNB_CONTRACT=0xbb4cdb9cbd36b01bd1cbaebf2de08d9173bc095c
~ WBNB contract for buy the token

FACTORY=0xcA143Ce32Fe78f1f7019d7d551a6402fC5350c73
~ Pancake Factory contract to get function of buy

ROUTER=0x10ED43C718714eb63d5aA57B78B54704E256024E
~ Pancake Factory contract to process function of buy

YOUR_ADDRESS=
~ Your BSC (BEP20) address from trustwallet or another wallet.

SLIPPAGE=1
~ Customize your slippage here, cannot decimal. (eg : 1, 5, 10). if you buy early token recommended 30+ Slippage

GWEI=5
~ Customize your GWEI (gas fee) here, cannot decimal. (eg : 5, 10, 25). if you buy early token recommended 15+ GWEI

GAS_LIMIT=345684
~ Minimul limit is 210000, more much more better.

MIN_LIQUIDITY_ADDED=3
~ Set how much minimum liquidity added in pair address that you want to buy. set in BNB. (eg : 2, 4, 7).
  2 mean 2 BNB liquidity added.

YOUR_MNEMONIC=
~ Input your private Key here, that you get from your wallet privacy.

AMOUNT_OF_WBNB=0.002
~ Amount how much you want buy the token in WBNB.

TO_PURCHASE=0xe9e7cea3dedca5984780bafc599bd69add087d56
~ Token address that you want to buy.


```
5. Approve your WBNB in pancake like this
   <img src="./assets/img.png">

6. run with <code>npm run snipe </code>.

7. Wait the bot do his job, if success, you will see like this picture. <br>
   <img src="./assets/botimg.PNG">
   
8. Close bot with <code>ctrl + C</code>.

## WARNING
All this bot feature are free, I'm never sell this bot, and I'm never share my TG account. Please be careful and DWYOR!. Only this bot is free, not advanced bot.

## TROUBLESHOOT
* there are some reason if your tx failed :
- you haven't approve your WBNB
- your gas price are to small
- your GWEI are to small (use 15+ for early token)
- your slippage are to small (use 30+ for early token)

* Error with node :
  
 <img src="./assets/wss-error.png">
  
For now <code>wss://bsc-ws-node.nariox.org:443</code> it won't be able to use again forever. for that you can use private node or build your own node. it more faster than public node.
there is my recommend for private node : 
  1. https://getblock.io/en/
  2. https://www.quicknode.com/
  3. https://www.ankr.com/ <br>
   
We also rent a full node with cheapest and also faster speed, you will get installation guide and maintenance for that just for $70/month, you can compare with private node that I recommend. The different full node with private node is, full node build in our own vps, so we can manage the speed and performance. 
