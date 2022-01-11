## What is it?

Most prominent AMM formula, popularised by Uniswap.

$x \times y = K$ $x$ and $y$ are *amounts of* tokens in the Liquidity Pool, $K$ is the total liquidity product, and the
ratio that the UniV2 AMM keeps constant after each swap.

The ratio of the two assets in the pool is the exchange rate $P$:
$\frac{x}{y} = P$

![xyk-pricing-curve](images/xyk-pricing-curve.png)

![xyk-quoting-formula](images/xyk-quoting-formula.png)

It follows that the coin reserves of a Liquidity Pool can be expressed in terms of price $P$ and constant $K$:

$x = \sqrt{K \times P}$ $y = \sqrt{\frac{K}{P}}$

![definition-and-refs-from-paper](images/definition-and-refs-from-paper.png)

$DL = \sqrt{R} - \frac{R+1}{2}$ where $R$ is the ratio of the initial (at deposit) and new price $R = \frac{P_1}{P_0}$

## Rewards

Simple, permissionless DEX to open a market for trading and Providing Liquidity [link to LP] ~~shitcoins~~ cryptocurrencies.

## Risk implications

Divergence loss [link to DL]


## Links

https://www.desmos.com/calculator/nw4zrqrftx
https://twitter.com/danrobinson/status/1429972775511408651
