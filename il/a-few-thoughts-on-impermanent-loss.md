![[Pasted image 20211203154948.png]]
The screenshot above is from a [Medium post](https://medium.com/@pintail/uniswap-a-good-deal-for-liquidity-providers-104c0b6816f2) that the [official Uniswap *V2* docs](https://docs.uniswap.org/protocol/V2/concepts/advanced-topics/understanding-returns) refers the reader to in order to explain the risks and returns associated when *providing liquidity* on their platform. I personally much prefer the term **divergence loss** myself, but for one reason or another, the original **impermanent loss**, or **IL** for short, stuck around.

To cut it short, this has always been strange to me, since both the docs and the article demonstrate that there is (most often) nothing impermanent about the loss. There have been many articles, twitter threads, and academic publications written to explain this phenomenon of IL to various people with different backgrounds. 

Money, narratives, and hot topics move fast in our Brave New World of crypto, but here I will attempt to write yet another. One that I wish I could have read when I read the docs and medium posts in the summer of 2020. My aim is clarity and brevity, but I may diverge onto other terms and topics, perhaps to expand on in later writings. Please bear with me.

![[Pasted image 20211203164239.png]]
*Total Value Locked (TVL) of Uniswap protocol, courtesy of [DefiLlama](https://defillama.com/protocol/uniswap/all/USD) **TODO UPDATE SCREENSHOT***

To start, there are a few other terms that I had never heard about before I got into DeFi which are inseparably linked to IL, and there is similarly a great body of texts explaining what they all mean in various ways. I learnt about them from crypto circles, mostly in the form of short, separated articles, not quite grokking how it all fit together. *Liquidity. Decentralized exchange. Automated Market Making. xy=k.* What does it all mean? Why should I care? Is it really the future of finance? I suppose I should start with a short description of the past and present of finance, and the various tangential but inseparable terms.

If you are like me, and don't have a background in finance or economics, [*liquidity*](https://en.wikipedia.org/wiki/Market_liquidity) is likely not something you've needed to know about or something you've encountered in your life. It is a feature of a market, or an asset (in our case, this means various crypto tokens) that is traded. **The more liquid something is, the harder it is to move its price.** When you go to the store to buy groceries, you don't need to think about liquidity, because the owner of the shop (the market maker) bought enough for everyone to get theirs from the shelf. The shop provides ample liquidty for all its customers on a day-by-day basis, so when you buy something, its price stays the same for other customers.

![[Pasted image 20211206125102.png]]
*Candlestick chart and CLOB snapshot of the [ETH/USD market on FTX](https://ftx.com/trade/ETH/USD)*

![[Pasted image 20211206125332.png]]
*Liquidity pool mechanism figure from the [official Uniswap V2 docs](https://docs.uniswap.org/protocol/V2/concepts/core-concepts/pools)*

