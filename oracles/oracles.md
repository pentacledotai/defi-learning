https://blog.makerdao.com/introducing-oracles-v2-and-defi-feeds/

## SoK: Oracles from the Ground Truth to Market Manipulation

https://arxiv.org/abs/2106.00667

> An oracle is a bridge or gateway that connects the off-chain real world knowledge and the on-chain blockchain network. The ‘oracle problem’ [22] describes the limitation with which the types of applications that can execute solely within a fully decentralized, adversarial environment like Ethereum.

![](images/use-cases-categories.png)

![](images/oracle-workflow-stages.png)

Data Sources are defined here as passive entities that store and measure the representation of the ground truth. Common types of data sources include 
 - databases 
 - sensors
 - humans
 - smart contracts
 - or a combination of them

  Depending on how data sources gather and retrieve the ground truth, and where a representation of that value relies upon, there can be different attack types.
  
  ...
  
  > For instance, in Maker V2 oracle [74], the selection of the data feeders is done through a decentralized governance process [54]. MKR4 token holders vote on the number of authorized data feeders and who these data feeders can be [28].
  > Note that sometimes voting processes can provide the illusion of decentralization while not being much different than a centralized process in practice. To illustrate, consider a project with a governance token, in which most tokens are held by a few individuals where the project leaders advocate for their preferences and there is no established venue for dissenting opinions. If voters only inform themselves from one source of information, that source becomes a de facto centralized decision maker.

> The stake, can be both in token value and reputation of the data feeder. As an example, in Chainlink [41] protocol has a reputation contract that keeps track of the accuracy of data reporting of different feeders. Therefore, the combination of a loss of reputation, penalty fees, and the reduced (or eliminated) income from all future jobs provides the incentive for selected data feeders to act honestly. The module then forms a leaderboard, based on collateral and reputation, to select data feeders from all available data providers.

> In any case, incentives under staking are much closer to being endogenous than in the alternatives. 
> Decentralized selection is done by the holders of some scarce token, typically a governance token specific to the oracle service. The simplest decentralized mechanism to hold a vote amongst token holders, who are indirectly incentivized (we call this an exogenous incentive) cast informed votes since they hold a token tied to the success of the system (e.g., TruthCoin [96]). In a staking system, token holders are directly incentivized (a endogenous incentive) to vote ‘correctly’ (this remains to be defined but assume for now it means they vote in a way that will not be disputed) by posting some amount of their tokens as a fidelity bond. Stakers stand to be rewarded with new tokens and/or penalized (collateral slashed) depending on the performance of the data feeders they vote for.


### Evaluation Framework on the selection of data feeders

 - No trusted third party
 - Low latency
 - Resilient to Sybil Attacks
 - Resilient to Targeted Denial of Service Attacks
 - Incentives are Endogeneous


### Aggregation of Data Feeds
> To improve the quality of simple statistics such as the median and the mode, weights can be applied in the calculation. For instance, to mitigate manipulation of price data, one can choose to use time-weighted average price (TWAP) [102], or liquidity volume, or both [2]. Typically, the liquidity and trading volume of a market correlates with the quality of the price data. To illustrate, Uniswap V2 uses TWAP over several blocks (e.g., mean price in the last 10 blocks) to reduce the possibility of market manipulation in a single block (e.g., via flash loans [88]). In Uniswap V3, TWAP is optimized for more detailed queries including the liquidity volume and allowing users to compute the geometric mean TWAP [2].


### Dispute
TODO
  
  ![](images/oracle-classification-talbe.png)
  
  
  ## Other linkies
  
  https://oracles.club/
  
  [Blockchain Oracle Design Patterns](https://arxiv.org/abs/2106.09349)
  
  