
<h3 align="center">All development has been moved to <a href="https://github.com/thewaifuproject">@thewaifuproject</a></h3>

<h1 align="center">
  <br>
  <img src="https://raw.githubusercontent.com/corollari/waifuchain/master/webextension/promo/icon.png" width="200"></a>
  <br>
  WaifuChain
  <br>
</h1>

<h4 align="center">Tradeable blockchain waifus</h4>

<p align="center">
  <a href="#install">Install</a> •
  <a href="#build">Build</a> •
  <a href="#why">Why?</a> •
  <a href="#credits">Credits</a> •
  <a href="#license">License</a>
</p>

![screenshot](https://raw.githubusercontent.com/corollari/waifuchain/master/.github/screenshot.png)

## Install
- [**Chrome** extension](https://chrome.google.com/webstore/detail/waifuchain/injlalemmnakihphncnhbdckncjbcaac) [<img valign="middle" src="https://img.shields.io/chrome-web-store/v/injlalemmnakihphncnhbdckncjbcaac.svg?label=%20">](https://chrome.google.com/webstore/detail/waifuchain/injlalemmnakihphncnhbdckncjbcaac)
- [**Firefox** add-on](https://addons.mozilla.org/en-US/firefox/addon/waifuchain/) [<img valign="middle" src="https://img.shields.io/amo/v/waifuchain.svg?label=%20">](https://addons.mozilla.org/en-US/firefox/addon/waifuchain/)

## Build

### Clone repository
```bash
git clone --recursive https://github.com/corollari/waifuchain.git
```

### Build browser extension
```bash
cd webextension
npm install -g browserify #Install browserify
npm install #Install dependencies
npm run build #Build extension
```

### Collect/scrap waifu data
```bash
cd scrapper
pip install -r requirements.txt
python scrapper.py
python normalize.py
```

### Set up the database
```bash
#An SQL database must be installed
cd scrapper
pip install -r requirements.txt
python waifuselect.py
python createdb.py
```

### Run server (main website & API)
```bash
cd server
php -S localhost:8000 #The database must have been set up (see previous section) in order for the server to work properly
```

### Build and deploy contract
We are currently using [Remix](https://remix.ethereum.org/).

## Why
> Your scientists were so preoccupied with whether or not they could, they didn't start to think if they should.
<p align="right">- Dr. Malcolm</p>

## Credits
The following external resources have been included as part of the project:
- Ethereum Foundation's Web3.js 
- The icon used in the extension is an image of Zero Two, one of the main characters of the series DARLING in the FRANXX.

## License
The Unlicense
