# MultiSend

## Problem
Private individuals usually make a few transactions, so they don't have any kind of problems with blockchain.

However, Moon Funding company had the need to make hundreds of transactions every single day. And making hundreds of them on a one by one basis would take an eternity in terms of time.

## Solution
We use that smart contract to send payments to our users in groups of ~100 instead of one by one. 

## Why ~100 and not more?
We have that number limitation because if we sent everything at the same time, we would fill entire blocks of the ETH blockchain, thus making it slower and more expensive for all the community.

Sending transactions in blocks of ~100 consumes on average 3,1 million of gas limit and every block has a ~8 million capacity. So we use 39% of block space in every transaction.
We would have to pay 0,062 ETH transaction fee at average price ($41 at the time of writing) using a 20 Gwei gas price.

So, we use https://ethgasstation.info/ to pay less transaction fees while making fast payments to our customers. 
By using 1 Gwei gas price, we only pay 0,0031 ETH ($2 at the time of writing). 

That way, transfers are not almost instant but they usually take between 30 minutes and a few hours. We just need to wait until there is a 39% empty space with a >=1 Gwei price in a block so we can jump in.

### Payment Proofs
You can see our payment proofs at https://moonfunding.com/payment-proofs/

