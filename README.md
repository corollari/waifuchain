
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

![screenshot](https://raw.githubusercontent.com/corollari/waifuchain/master/webextension/promo/screenshot.png)

## Install
The extension can be installed through [Chrome's Web Store](https://chrome.google.com/webstore/detail/waspline-reader/ndlnnojbbcbdpkccfmcgbopalpbmhbhm) or [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/waspline-reader/)

## Build

### Clone repository
```bash
git clone --recursive https://github.com/corollari/waifuchain.git
```

### Build browser extension
```bash
cd webextension
npm install
# Run the following command to update the version of Web3.js being used. Given that non-backwards compatible releases are common for Web3.js, this may break the extension.
# npm run updateWeb3
npm run build
```

### Collect/scrap waifu data
```bash
cd scrapper
pip install -r requirements.txt
python scrapper.py
```

### Run server (main website & API)
```bash
cd server
php -S localhost:8000
```

### Build and deploy contract
We are currently using [Remix](https://remix.ethereum.org/).

## Why
> Your scientists were so preoccupied with whether or not they could, they didn't start to think if they should.
<p align="right">- Dr. Malcolm</p>

## Credits
The following external resources have been included as part of the project:
- Ethereum Foundation's Web3.js 
- The [wasp icon](https://icons8.com/icon/6558/wasp) used in the extension comes from Icons8's Free License icon collection

## License
The Unlicense
