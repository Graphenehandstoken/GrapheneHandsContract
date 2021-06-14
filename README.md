
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
The team behind Graphene Hands is comprised of United States Army vet, business owner, and software engineers from some of the best engineering schools in the world. While this team provides an opportunity for investors to benefit from the rise in value from the Graphene Hands Token, investors will also be contributing to a Dev Wallet which will be used to push the bounds of global monetary policies.


## Token Concept
The token will have three phases. The first phase will be managed entirely by the development team. The second phase will rely on the community for self-management. Phase 1 is necessary while the number of holders is low and adoption is increasing. To guarantee long term success, the development team will initially manage the fees and structure associated with the currency. Once the initial phase is over or stability and ubiquity of the token is achieved, control will be released to the world during Phase 2. Phase 3 is where change starts to happen through what we are calling "Project Agora". 

### Phase 1: Development Team Token Management Approach
Graphene Hands is an entirely new kind of token that initially takes advantage of the predictable nature of liquidity pools and cryptocurrency markets. Trading crypto is unlike traditional investing as the price of the token is not based on what the buyers and sellers are willing to pay. It is entirely based on the ratio of the trading pair in the liquidity pool. The price is set via a simple x*y=k equation (we get deeper into this later) which allows entry and exit of your position at predictable price levels. As can be seen in the below table, as the liquidity pool grows, the price impact of selling .2 BNB diminishes.  

![numbers](https://user-images.githubusercontent.com/84188628/118306768-d7f36700-b4b7-11eb-877d-d4d74023c4e0.PNG)

Taking advantage of this knowledge, it becomes possible to manage the stability and movement of the token value in a predictable fashion. In doing so, we are creating a new token that leverages deflationary burn and anti-sell mechanisms to help control the value of the token! The below information regarding the contract is a technical deep dive that you will not see from other token providers. Because we intend to release control of the token to the world, it is imperative that investors who will eventually vote on the outcome of the token have a decent understanding of how things work.

For transparency there are core concepts everyone should understand
- The development team will NOT renounce the contract. We need access to the contract to control fees long term 
- The development team manually manages the liquidity. All liquidity goes to the Graphene Hands wallet which will be controlled by the development team solely for the purpose of injecting liquidity back into the token. None of these funds will be returned to the dev team. Eventually we intend to enable the automated liquidity functions in the smart contract but in the short term the development team will manage this.
- The development team will pay the high fees to sell just like everyone else, the only exclusions to this rule are the liquidity and promotion wallets.
- Early buyers will NOT be able to sell their positions until after the total fees + price slippage goes below the Pancakeswap limitation of 49%. We generally anticipate this to occur when the liquidity fee reaches 40%

### Phase 2: community Managed Tokenomics
Once price stability and adoption is achieved the Graphene Hands development team will release a series of voting systems that will allow holders to vote on the specific tokenomics. We will likely run the vote every month and attempt to evenly distributing voting rights based on the number of tokens held, while putting in precautions to avoid whales from chosing the direction. We also expect to directly engage the community on how best to achieve these goals.

### Phase 3: Project Agora
Through phase 1 and 2 the development team will be diligently working to develop what we are calling "Project Agora". The scope and global impact will reach full strength as we bring "Project Agora" online. While we will not disclose any details until we launch, we do recommend taking a look at the role the Agora had on the world. A modern day digital Agora backed by blockchain is a concept we are very excited to introduce! 
https://www.livescience.com/4861-greek-agora-changed-world.html


### Understanding How Tokens implement Liquidity Fees
As mentioned, the liquidity pool drives the price of the token using the simple formula X*Y=K where x and y are the token pairs and K is some constant. When the liquidity pool is created K is selected by the development team. As people buy and sell, the ratio of X*Y must always equal K, which is what causes the price to move. As you take out token Y, the value of token X goes up. Additionally, as the size of X and Y increases (i.e. the liquidity pool grows) the price impact of buying and selling diminishes. This is best illustrated from our friends at Uniswap | Pools

![liqdiagram](https://user-images.githubusercontent.com/84188628/118306982-1557f480-b4b8-11eb-833f-f4eae5e8c3cf.jpg)

https://uniswap.org/docs/v2/core-concepts/pools/

With this knowledge, how does Graphene Hands work? There are 4 key concepts
- Initial liquidity is small, this will drive the price up very quickly as the amount of BNB in the pool will increase while the amount of Graphene Hands in the pool decreases
- The 50% slippage limitation is a Pancakeswap UI limitation, it’s not part of the core API used by Pancakeswap. For this reason, BOTs that use the APIs directly will move into and out of their positions paying hefty fees which adds to the liquidity pool. If you look at tokens such as SafeMoon you will see 100s of thousands of dollars being sold every couple minutes by bots that take advantage of reflection to create a nearly infinite supply for the money printer. Specifically for SafeMoon, if a 4% holder receives reflection on every transaction it is actually possible for the BOT to continually sell without losing any value. This is why we do not implement reflection and why we have created this BOT honeypot.
- In the early months buyers will NOT be able to sell their positions via Pancakeswap UI/App (due to slippage limitations) and if they bypass Pancakeswap they will be severely penalized with fees. The developers of Graphene Hands will manage the liquidity pool manually in order to create price stability prior to anyone attempting to exit their position. We will do this through the tokens we are retaining in our deployer wallet. Think of it this way, we are leveling the playing field for everyone by creating price stability so that EVERYONE benefits vs the elite few with big wallets. NONE of the liquidity contributions will be accessed by the development team.
-  As the liquidity fee drops below the Pancakeswap 49% limit big sells will simply not be possible. This is because the total slippage of the sell is the sum of fees + price change. Therefore a big sell will simply return the taxed portion of the sell back into the liquidity cutting the tokens loss by x%.
To be clear, if you try to sell through Pancakeswap in the early months while fees are high the transaction WILL NOT go through. Once the fees + price impact drop below 49% it will only then be possible to sell. But by this time the development team behind Graphene Hands will have created a large liquidity pool to minimize price impacts of the sells that take place. We do not in any way financially benefit from these contributions to liquidity.

Other contracts that use liquidity fees will transfer the tokens to the contract as buyers and sellers move into and out of positions. Periodically, and at predictable times, the contract will swap out the tokens for BNB and add the pair to the liquidity pool. This is great for bots and manipulators because all of this information is on the public block chain. If you know when this trigger is (which you can pretty easily figure out) then you can easily trade around these events for profit. Yes, this is happening but no one publicizes it. Even worse, if you don't know what you're doing things like this happen: https://safefairmoon.medium.com/exposing-suspicious-transaction-activity-in-fairmoon-token-d989b5d019e7 . Be careful, some of these carbon copy tokens out there may be in for a BIG drop if the dev team doesn't understand how things actually work! 

We manage all of this differently by sending the liquidity tokens to a wallet that is managed by the developer team. We are being fully transparent about this, we the development team manage the liquidity fee pool. Manually managing the liquidity allows the price to run hot but then allows us to beef up the liquidity before anyone exits their position.

### Fee Structure
Buyers are welcome, paying 0% fees to enter their position. Sellers on the other hand are penalized for Paper Handing out. The below fee structure ONLY applies to sells of Graphene Hands. 

#### Promotion Wallet (.5%)
In order to encourage participation, the team implemented a promotion wallet that receives .5% of every sell transaction. These funds will transparently be used to promote the token and gain awareness through contests, running a giveaway or taking advantage of influencers. 

#### Dev Wallet (1%)
As previously mentioned, the dev team will use the 1% dev fee to further enhancements regarding application of Graphene technologies. We realize this is a broad and sweeping statement but the field is just emerging so we want to be strategic in how we use the dev wallet long term. The ultimate goal is to bring Graphene product development in house in order to usher in a new era of prosthetics and wearable gaming and fitness trackers.  

#### Burn Wallet (.5%)
If you are reading this we assume that you are interested in the nitty gritty details of how Graphene Hands works. With that said, we are going to deep dive how things actually work instead of just saying we "burn tokens". 
Burning tokens is a very misunderstood concept that many tokens do in order to check a checkbox. The first kind of burn is known as a developer burn, these are tokens that the developers burn before or after initial ICO. This burn does NOT directly affect the price of a token. It does however have the benefit of making buyers think the value of the token is going to go up. On the surface this is true, by burning the tokens the developers cannot sell their holdings and cash out which would drop the value of the token. But burning developer tokens that are NOT in the liquidity pool will not actually change the price of the token, it only changes the perception of the token. 
Tokens burned from the liquidity pool actually do change the price of the token. This is because the ratio of the pair in the liquidity pool is forever changed. For example, if you have 1 BNB = 100,000 Graphene Hands tokens in the liquidity pool and I take out 50,000 Graphene Hands tokens from the pool, each Graphene Token is now more valuable relative to the BNB, therefore the price goes up. Burning tokens from the liquidity pool as transactions occur WILL push the price up as those tokens are forever removed from the liquidity pool. When you add liquidity you must add the liquidity to the pool based on the ratio of the BNB to Graphene Hands, this will NOT change the price but will create price stability for new buyers/sellers. 
With this knowledge in hand (no pun intended) Graphene Hands will burn liquidity pool tokens which will push the price up. At some point in the future the Dev Team will burn their developer tokens but for the initial launch the team intends to keep these tokens on hand in order to stabilize liquidity as necessary. Since there will not be any sellers in the early months (except for BOTS) we will need to pull this liquidity from somewhere which is the developer account.

#### Liquidity (3% Base + 50% which decreases by .25% every day)
All buying and selling comes from what is known as a liquidity pool. Think of it like a bucket of water where all of the buying and selling takes place. When you place your buy or sell you are throwing a rock into the bucket of water. If the bucket is small, the water may overflow and cause large ripples. Now imagine throwing the same rock into a lake full of water. This same rock will have little to no effect on the large body of water. This is exactly how liquidity pools function, the larger the pool, the less impact buying and selling will have on the price. It is for this reason we want to create the LARGEST pool of liquidity possible prior to anyone selling.
On launch the total liquidity pool fee is 53% which will decrease by .25% every day until it reaches 3% at which point the fee stops decreases. Early paper handing sellers will VERY quickly create a strong liquidity pool so that the later selling Graphene Hand holders will have a strong liquidity foundation to stand on. 

### What are our Plans regarding locking and renouncing the contract?
The Graphene Hands token evolution/life will be the following. Note that we are waiting to lock dev tokens and liquidity in order to minimize cost as each lock has an associated cost with it.
- Initially the deployer account of the Graphene Hands token will use its tokens to add liquidity. This will be done as the price rises, prior to anyone selling their position
- The liquidity pool will be locked as the value of the pool increases (Using Cryptex - https://cryptexlock.me/)
- Majority of the Developer tokens will be locked via Cryptex as value increases (Using Cryptex - https://cryptexlock.me/)
- The deployer account will remain unlocked so as to use for adding liquidity and listing on additional exchanges


### Initial Token Protections
During the initial launch the Dev team strategically chose a fee structure to maximize returns and provide stability. The initial fee structures have the following benefits.

#### Whale Protection and Dump Protection
Within PancakeSwap there is a hard limit of 49% slippage. By starting fees above this value it will not be possible to sell tokens. It is not until the fees+price change are less than 49% that the first sales can take place. If you are a big holder and attempt to dump your holdings the sale will simply not go through because the fees+price change will go above the slippage amount. For those that are interested, the API that is used that causes all of those annoying Pancakeswap errors takes in an input token amount and an expected output token amount. If the output token amount is less than what is expected (based on slippage) then the entire sell order fails. Because of this, whales simply cannot dump because the price change will be too large. If they bypass Pancakeswap then we should all thank them for their liquidity contributions!

#### BOT Prevention
As previously mentioned, BOTs that use the lower level APIs to buy and sell will be eaten by the Graphene Hands smart contract. Bypassing Pancakeswap will allow the BOTS to trade in and out, but will pay very hefty fees that will benefit the greater community

#### Managing Liquidity
The Dev team will manage liquidity and initially will not rely on the automated swapandliquify() functions that other contracts use. Manually managing this functionality allows us to beef up the liquidity prior to anyone selling and avoid BOTS and the elites from predicting when the next liquefaction event will occur. This way everyone benefits from better price stability versus a couple big whales dumping on the community. 



