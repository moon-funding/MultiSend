# MultiSend

## Problem
Private individuals usually make a few transactions, so they don't have any kind of problems with blockchain.
However, Moon Funding company had the need to make hundreds of transactions every single day. And making hundreds of them on a one by one basis would take an eternity in terms of time.

## Solution
We use that smart contract to send payments to our users in groups of ~100. We have that number limitation because if we sent everything at the same time, we would fill entire blocks of the ETH blockchain.
So, we use https://ethgasstation.info/ to pay as little transactions fee as possible while making fast payments to our customers. 

### Payment Proofs
You can see our payment proofs at https://moonfunding.com/payment-proofs/

