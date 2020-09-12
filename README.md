# MultiSend

## Problem
Private individuals usually make a few transactions, so they don't have any kind of problems with blockchain.

However, Moon Funding LTD needed to make hundreds of transactions every single day. And making hundreds of them on a one by one basis would consume a lot of time and money.

## Solution
We use that smart contract to send payments to our users in groups of ~100 instead of one by one. 

## Benefits
- We cut transfer fees and costs by 95%
- We reduce human resources needed to process transfers.

## Why ~100 and not more?
### Short answer
It reduces the company transfer fees and costs by 95%.

Sending more than 100 transfers at once would be more expensive for the company.
### Long answer
In the ethereum blockchain, for transfers to be confirmed they need to be included into a "block".

Each block has a capacity of ~8 million gas and by sending 100 transactions at once with this contract, we spend ~3,1 million gas.

That means that we fill 39% of an entire block.

If we chose to fill a 100% of the block, we could make faster payments but it would be by far more costly as we would need to pay the biggest fee in the market.

However, if we only fill a smaller percentage of the block we can compete in gas prices and therefore we are able to reduce costs by 95% in average.

| Number of transfers | % of block filled |  Gas Price |  Total Tranfer Fee (ETH) | Total Tranfer Fee (USD) | Cost per transfer (USD) |
| -------------| ------------- | ------------- | ------------- | ------------- |  ------------- | 
| 256 | 100%  | 20 Gwei  | 0,1589 ETH | $105 | $0.41
| 100 | 39%  | 1 Gwei  | 0,0031 ETH | $2  | $0.02
* Data as of 2018, when this smart contract was coded.

## Conclusion
Instead of sending transfers in bulks of 256, we send them in bulks of 100 which is by far more efficient economically speaking.

If we want to send 256 payments, we would send out 2 bulks of 100 transfers and 1 bulk of 56 (or what is the same -> 3 bulks of 85 [256/3] transfers) and that would cost $5,12 in fees instead of $105 (a 95% decrease in fees)

## Payment Proofs
You can see our payment proofs at https://moonfunding.com/payment-proofs/
