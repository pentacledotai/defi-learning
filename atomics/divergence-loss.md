## What is it?

The loss produced by providing tokens as liquidity to an AMM instead of just holding them, if the tokens diverge in
price.

Divergence loss is the difference between the value of an LP position vs the same account holding fixed amounts of those
same tokens.

## Rewards

Protocols typically give out rewards/yield to counterbalance the risk, which often, but not always makes up for the
divergence loss suffered.

## Risk implications

Divergence loss is a risk that one is exposed to when providing liquidity on an AMM.

## Further / Optional detailed

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