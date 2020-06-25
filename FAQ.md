# Frequently Asked Questions (FAQ)

## Circulating Supply

### How do you calculate circulating supply and why do some of them have a question mark?

Circulating supply is a tricky question in the cryptoworld and since it is used to generate market cap it also is very important.

Most ranking sites just take the number of block and the coins block reward schedule to determine circulating supply.  

This is highly inaccurate because it doesn’t include transaction fees, superblocks (for masternode coins) or other special block rewards.

Xplorenow pulls most circulating supplies from CoinGecko, but if a coin has a more accurate API for circulating supply, we use that.

If the circulating supply is question mark, then we can’t find any data for the circulating supply.  This also means their market cap cannot be determined.

If you know of a more accurate API for circulating supply for a cryptocurrency please open an issue: https://github.com/clockuniverse/xplorenow/issues

## Circulating Supply and Lost Coins

### What about circulating supply and lost coins?

Lost coins can be caused for a variety of reasons such as lost computers, lost passwords, or burn coins.

Most cryptocurrencies have no way to accurately determine the number of lost coins.  A cryptocurrency team could discount old unused address as “lost,” but there is no way to know if this is true.

Lost coins are not considered for circulating supply on Xplorenow unless they are shown burnt on the cryptocurrencies blockchain.

## Market Cap

### How do you calculate market cap?

Market Capitalization or better known as market cap is found by multiplying the circulating supply and the price.

If the circulating supply is unavailable, then the market cap shows as “Market Cap Unavailable.”

## No Volume in 24 Hours

### What does No Volume in 24 hours mean related to the price?

This means there is no volume in the past 24 hours and the last price is the last price where there was volume.  This could mean it was in the past couple of days or months old.

## Price

### How is the price calculated?

Price calculation is an important part of xplorenow because we want to have the most accurate pricing of any coin ranking site.

Price is averaged but weighted by volume.  The more volume a pairing has the more weight that price is given to the overall average.

The reason we are using a weighted price by volume is because outlier prices can highly distort the actual price of a coin.

Anyone can find a dead pairing and sell to themselves to manipulate the coin price but with a weighted price by volume they would have to spend much more money to do that.

If you find price anomalies please open an issue here: https://github.com/clockuniverse/xplorenow/issues

## Price Unavailable

### What does price unavailable mean?

Price unavailable means there has never been a trade on that pairing on that exchange.  We want to make sure everyone is aware of all the pairings that a cryptocurrency is trading on, so we have included pairings that currently have never had a trade.  We think this will improve arbitrage and tradability for all cryptocurrencies.

## Quality Items

### What are quality items?

Quality items are a way to show the "quality" of a coin.  These items cannot be opinion items but must have a link or proof of existing.  This will give a better understanding of the "quality" of a coin.

Each quality item is usually a linkable infrastructure item for the coin, number of pairs, or market cap.

Some of the items, such as website is something that every coin should have, while other items such as hardware wallet are more difficult for a coin to have.

All quality items are weighted by a point value.  This point value can be changed in the future as we balance the weight of each quality item to best rank a coin.

Most quality items are a yes or no question with a link meaning yes.  For example, in the list below, Website is the question, “Does the coin have a website?”  If the answer is yes, a link is required to prove this.

You can look at each coin’s quality items and their weight on the coins home page.

Current quality items are:
* Age of coin (generated from first block on current blockchain)
* Market Cap of coin (though only slightly weighted)
* Website (Link)
* Open Source (Link)
* Block Explorer (Link)
* Number of pairs (generated automatically by xplorenow API calls)
* CoreWallet – Linux (Link)
* CoreWallet – Windows (Link)
* CoreWallet – MacOS (Link)
* Mobile Wallet – Android (Link)
* Mobile Wallet – iOS (Link)
* Paper Wallet (Link)
* Multicoin Wallet (Link) 
* Hardware Wallet (Link)
* Public Team (Link.  This link can be the same as the coin’s homepage)
* Decentralized Governance (Link)
* Public Team Spending (Link?)

Additional quality items will be added in the future.  If you have quality item suggestions feel free to contact us or put in an issue here: https://github.com/clockuniverse/xplorenow/issues
