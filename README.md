# BURN TO EARN
## Inspiration

Our project is inspired by the desire to promote physical fitness and encourage more people to lead a healthy lifestyle. By offering discount coupons, we aim to incentivize individuals to actively put in the work in their workouts consistently while providing tangible rewards for their efforts. Our goal is to create a seamless and engaging fitness experience that combines the power of trustless, decentralized and transparency in web3 to create a product solution.

## What it does

Burn2Earn is a fitness mobile application where the users can earn tokens for their physical activity every day. We have integrated with GoogleFit APIs to fetch the steps, calories bunt, heart points for each day and calculate the total amount of tokens using a complex algorithm with the help of Chainlink cloud functions to mint ERC20 Tokens(BuffTokens) to the user. Tokens can be claimed regularly by the users in a 24 hour window based on their physical activity. One can purchase BuffCoupons(ERC115 Tokens), Discount Coupons or Offers using the BuffTokens earned. More into the technical aspect, we have two javascript source codes for two actions: RegisterAccount and MintToken. The Register Account source code when called authenticates the wallet address to the gmail account with the help of DON encrypted google access token. Once registered, the wallet can use the access token to Mint Token every 24 hours using the MintToken source code which has the algorithm that generates the amount of tokens that can be minted for the physical activity performed by the user. One can claim coupons using the claimCoupon function by burning the specified amount of tokens labelled for the discount coupon.

## How we built it

The entire application is built purely on React Native. We used the ThirdWeb SDK to integrate web3 functionality into our mobile application. We used the Google API for Authentication and Google Fit API to get the fitness metrics on-chain using our Chainlink Cloud functions. We built our smart contracts with Solidity bootstrapped by OpenZeppelin.

