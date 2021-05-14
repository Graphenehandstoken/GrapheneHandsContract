
<p align="center">
   <img src="https://user-images.githubusercontent.com/84188628/118306891-fbb6ad00-b4b7-11eb-870b-2613666764fb.png" width="400" height="250">
</p>
  
## Not for Paper Hands. Not even for Diamond Hands, this is Graphene Hands


<!-- TABLE OF CONTENTS -->
- [About the Team](#about-the-team)
- [Token Concept](#token-concept)
- [Tokenomics](#tokenomics)
- [Fee Structure](#fee-structure)
- [Built in Contract Protections](#protections)

## About the Team
The team behind Graphene Hands is comprised of United States Army vets, business owners, and software engineers from some of the best engineering schools in the world. While this team provides an opportunity for investors to benefit from the rise in value from the Graphene Hands Token, investors will also be contributing to a Dev Wallet which will be used to advance Graphene related innovations around
- Tactile enabled Graphene Prosthetics and Gameplay wearables
- Rapid charge Graphene based batteries
- Wearable technologies leveraging Graphene conductivity

The Dev Wallet will be used to form strategic partnerships with industry to push forward Graphene centric efforts. Over time we would like to bring this development in house to start releasing our own Graphene based product lines starting with a line of smart wearables. The application of Graphene is a new and emerging field that takes a large amount of capital in order to make substantial progress. Million mile batteries from Tesla, rapid charge batteries from Samsung and ultra-lightweight tactile enabled prosthetic limbs are all paving the way toward broader adoption of Graphene, and we want to be part of the revolution! Don't believe us, here is the proof...

>_Chinese EV maker Guangzhou Automobile New Energy announced that it has developed a graphene-enhanced battery that can be charged up to 85 percent in 8 minutes. Guangzhou believes the battery can be available for mass production as early as the end of this year._
>
https://investingnews.com/daily/tech-investing/nanoscience-investing/graphene-investing/graphene-battery-tesla/

>_The researchers have shown how graphene and other related materials can be directly incorporated into fabrics to produce charge storage elements such as capacitors, paving the way to textile-based power supplies which are washable, flexible and comfortable to wear._
>
https://www.graphene-info.com/researchers-develop-washable-wearable-graphene-capacitors-can-be-woven-directly-clothes

>_Samsung may be in the race to develop a graphene-based alternative to lithium-ion batteries for its phones. Rumors are going around claiming that the Company hopes to have at least one phone with a graphene battery ready next year or by 2021.
The word is that these graphene-based batteries will be capable of a full charge in under a half-hour_
>
https://www.graphene-info.com/samsung

We have numerous opportunities in the works for application of Graphene Hands token in the world of graphene technologies including using tokens to
- Buy time on Graphene Printers
- Purchasing internally developed Graphene centric products such as smart wearables, biometric monitors and energy storing fabrics
- Having a vote in the product lines we intend to pursue

## Token Concept
Graphene Hands is an entirely new kind of token that takes advantage of the predictable nature of liquidity pools and cryptocurrency markets. Trading crypto is unlike traditional investing as the price of the token is not based on what the buyers and sellers are willing to pay. It is entirely based on the ratio of the trading pair in the liquidity pool. The price is set via a simple x*y=k equation which allows entry and exit of your position at predictable price levels. As can be seen in the below table, as the liquidity pool grows, the price impact of selling .2 BNB diminishes.  

![numbers](https://user-images.githubusercontent.com/84188628/118306768-d7f36700-b4b7-11eb-877d-d4d74023c4e0.PNG)

Taking advantage of this knowledge it is then possible to manage the stability and movement of the token value in a predictable fashion. In doing so, we are creating a new token that leverages deflationary burn and anti-sell mechanisms to push the value of the token to the moon! The below information regarding the contract is a technical deep dive that you will not see from other token providers. We are presenting the next evolution of a truly safe moon opportunity!
For transparency there are core concepts everyone should understand
- The development team will NOT initially renounce the contract. We need access to the contract to control fees and eventually enable automated swap and liquefy functions. 
- The development team manually manages the liquidity. All liquidity goes to the Graphene Hands wallet which will be controlled by the development team soley for the purpose of injecting liquidity back into the token. None of these funds will be returned to the dev team
- The development team will pay the high fees to sell just like everyone else, there are no exclusions to this rule 
- Early buyers will NOT be able to sell their positions until after the total fees + price slippage goes below the Pancakeswap limitation of 49%

### Tokenomics
As mentioned, the liquidity pool drives the price of the token using the simple formula X*Y=K where x and y are the token pairs and K is some constant. When the liquidity pool is created K is selected by the development team. As people buy and sell, the ratio of X*Y must always equal K, which is what causes the price to move. As you take out token Y, the value of token X goes up. Additionally, as the size of X and Y increases (ie the liquidity pool grows) the price impact of buying and selling diminishes. This is best illustrated from our friends at Uniswap | Pools

![liqdiagram](https://user-images.githubusercontent.com/84188628/118306982-1557f480-b4b8-11eb-833f-f4eae5e8c3cf.jpg)

https://uniswap.org/docs/v2/core-concepts/pools/

With this knowledge, how does Graphene Hands work? There are 4 key concepts
- Initial liquidity is small, this will drive the price up very quickly as the amount of BNB in the pool will increase while the amount of Graphene Hands in the pool decreases
- BOTS that bypass Pancakeswap will pay the hefty fees associated with the token. The 50% slippage limitation is a Pancakeswap limitation, not part of the core API used by Pancakeswap. For this reason, BOTs that use the APIs directly will move into and out of their positions paying hefty fees which adds to the liquidity pool. If you look at tokens such as SafeMoon you will see 100s of thousands of dollars being sold every couple minutes by bots that take advantage of reflection to create a nearly infinite supply for the money printer. Specifically for SafeMoon, if a 4% holder receives reflection on every transaction it is actually possible for the BOT to continually sell without losing any value. This is why we do not implement reflection and why we have created this BOT honeypot.
- In the early months buyers will NOT be able to sell their positions via Pancakeswap (due to slippage limitations) and if they bypass Pancakeswap they will be severely penalized with fees. The developers of Graphene Hands will manage the liquidity pool manually in order to create price stability prior to anyone attempting to exit their position. We will do this through the tokens we are retaining in our Deployer Wallet once Graphene Hands launches. Think of it this way, we are leveling the playing field for everyone by creating price stability so that EVERYONE benefits vs the elite few with big wallets. NONE of the liquidity contributions will be accessed by the development team.
-  As the liquidity fee drops below the Pancakeswap 49% limit big sells will simply not be possible. This is because the total slippage of the sell is the sum of fees + price change. Therefore a big sell will simply not work because the slippage will be too high and will not go through. This means that no one can dump their holdings and cash out.
To be clear, if you try to sell through Pancakeswap in the early months while fees are high the transaction WILL NOT go through. Once the fees+price impact drop below 49% it will only then be possible to sell. But by this time the development team behind Graphene Hands will have created a large liquidity pool to minimize price impacts of the sells that take place. We do not in any way financially benefit from these contributions to liquidity.

Other contracts that use liquidity fees will transfer the tokens to the contract as buyers and sellers move into and out of positions. Periodically, and at predictable times, the contract will swap out the tokens for BNB and add the pair to the liquidity pool. This is great because all of this information is on the public block chain. If you know when this trigger is (which you can pretty easily figure out) then you can easily trade around these events for profit. Yes, this is happening but no one publicizes it. Even worse, if you don't know what you're doing things like this happen: https://safefairmoon.medium.com/exposing-suspicious-transaction-activity-in-fairmoon-token-d989b5d019e7 . Be careful, some of these carbon copy tokens out there may be in for a BIG drop if the dev team doesn't understand how things actually work! 

We manage all of this differently by sending the liquidity tokens to a wallet that is managed by the developer team. We are being fully transparent about this, we the development team manage the liquidity fee pool. Manually managing the liquidity allows the price to run hot but then allows us to beef up the liquidity before anyone exits their position.

### Fee Structure
Buyers are welcome, paying 0% fees to enter their position. Sellers on the other hand are penalized for Paper Handing out. The below fee structure ONLY applies to sells of Graphene Hands. 

#### Promotion Wallet (.5%)
In order to encourage participation, the team implemented a promotion wallet that receives 1% of every sell transaction. These funds will transparently be used to promote the token and gain awareness through contests, running a giveaway or taking advantage of influencers. 

#### Dev Wallet (1%)
As previously mentioned, the dev team will use the 2% dev fee to further enhancements regarding application of Graphene technologies. We realize this is a broad and sweeping statement but the field is just emerging so we want to be strategic in how we use the dev wallet long term. The ultimate goal is to bring Graphene product development in house in order to usher in a new era of prosthetics and wearable gaming and fitness trackers.  

#### Burn Wallet (.5%)
If you are reading this we assume that you are interested in the nitty gritty details of how Graphene Hands works. With that said, we are going to deep dive how things actually work instead of just saying we "burn tokens". 
Burning tokens is a very misunderstood concept that many tokens do in order to check a checkbox. The first kind of burn is known as a developer burn, these are tokens that the developers burn before or after initial ICO. This burn does NOT directly affect the price of a token. It does however have the benefit of making buyers think the value of the token is going to go up. On the surface this is true, by burning the tokens the developers cannot sell their holdings and cash out which would drop the value of the token. But burning developer tokens that are NOT in the liquidity pool will not actually change the price of the token, it only changes the perception of the token. 
Tokens burned from the liquidity pool actually do change the price of the token. This is because the ratio of the pair in the liquidity pool is forever changed. For example, if you have 1 BNB = 100,000 Graphene Hands tokens in the liquidity pool and I take out 50,000 Graphene Hands tokens from the pool, each Graphene Token is now more valuable relative to the BNB, therefore the price goes up. Burning tokens from the liquidity pool as transactions occur WILL push the price up as those tokens are forever removed from the liquidity pool. When you add liquidity you must add the liquidity to the pool based on the ratio of the BNB to Graphene Hands, this will NOT change the price but will create price stability for new buyers/sellers. 
With this knowledge in hand (no pun intended) Graphene Hands will burn liquidity pool tokens which will push the price up. At some point in the future the Dev Team will burn their developer tokens but for the initial launch the team intends to keep these tokens on hand in order to stabilize liquidity as necessary. Since there will not be any sellers in the early months (except for BOTS) we will need to pull this liquidity from somewhere which is the developer account.

#### Liquidity (2% Base + 50% which decreases by .25% every day)
All buying and selling comes from what is known as a liquidity pool. Think of it like a bucket of water where all of the buying and selling takes place. When you place your buy or sell you are throwing a rock into the bucket of water. If the bucket is small, the water may overflow and cause large ripples. Now imagine throwing the same rock into a lake full of water. This same rock will have little to no effect on the large body of water. This is exactly how liquidity pools function, the larger the pool, the less impact buying and selling will have on the price. It is for this reason we want to create the LARGEST pool of liquidity possible prior to anyone selling.
On launch the total liquidity pool fee is 52% which will decrease by .25% every day until it reaches 2% at which point the fee stops decreases. Early paper handing sellingers will VERY quickly create a strong liquidity pool so that the later selling Graphene Hand holders will have a strong liquidity foundation to stand on. 

### What are our Plans regarding locking and renouncing the contract?
The Graphene Hands token evolution/life will be the following. Note that we are waiting to lock dev tokens and liquidity in order to minimize cost as each lock has an associated cost with it.
- Initially the deployer account of the Graphene Hands token will use its tokens to add liquidity. This will be done as the price rises, prior to anyone selling their position
- The liquidity pool will be locked as the value of the pool increases (Using Cryptex - https://cryptexlock.me/)
- Majority of the Developer tokens will be locked via Cryptex as value increases (Using Cryptex - https://cryptexlock.me/)
- The deployer account will remain unlocked so as to use for adding liquidity and listing on additional exchanges
- The contract will not be renounced for at least the 1st year until the liquidity fee drops to 2%

### Protections
Core to the smart contract are inherit benefits of the high liquidity fees. 

#### Whale Protection and Dump Protection
Within PancakeSwap there is a hard limit of 49% slippage. By starting fees above this value it will not be possible to sell tokens. It is not until the fees+price change are less than 49% that the first sales can take place. If you are a big holder and attempt to dump your holdings the sale will simply not go through because the fees+price change will go above the slippage amount. For those that are interested, the API that is used that causes all of those annoying Pancakeswap errors takes in an input token amount and an expected output token amount. If the output token amount is less than what is expected (based on slippage) then the entire sell order fails. Because of this, whales simply cannot dump because the price change will be too large. If they bypass Pancakeswap then we should all thank them for their liquidity contributions!

#### BOT Prevention
As previously mentioned, BOTs that use the lower level APIs to buy and sell will be eaten by the Graphene Hands smart contract. Bypassing Pancakeswap will allow the BOTS to trade in and out, but will pay very hefty fees that will benefit the greater community

#### Managing Liquidity
The Dev team will manage liquidity and initially will not rely on the automated swapandliquify() functions that other contracts use. Manually managing this functionality allows us to beef up the liquidity prior to anyone selling and avoid BOTS and the elites from predicting when the next liquefaction event will occur. This way everyone benefits from better price stability versus a couple big whales dumping on the community. 



