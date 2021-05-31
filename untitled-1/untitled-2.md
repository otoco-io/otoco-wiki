# 2. Our proposed staking smart contract

A first release of our staking smart contract reflecting the above design can be found in [OtoCo’s GitHub](https://github.com/otoco-io), together with initial technical documentation.

The staking contract lets anybody who wants to pre-purchase the OtoCo token reserve a slot in a pre-order queue over a specific period of time.

During this token pre-order period, stakers can:

#### 1. Secure a place in a pre-order queue

They can do so by simply staking any amount of crypto assets - up to a given maximum - into a smart contract that keeps track of the amounts staked and the order in which staking happened.

**2. Lock in their pre-order token price**

The bonding curve function of the smart contract generates a price Y for each slot X in the pre-order queue. The curve slopes upwards, so the later you pre-order the higher the price.

Our front-end will show what place in the queue is available next and the corresponding token price for that specific slot.

Stakers who unstake at any time during the pre-order period but will lose their place in the queue and hence forfeit the price they had locked in.

Each staking and unstaking triggers an event at the smart contract level which dynamically recalculates the pre-order price for each staker. By simply connecting their wallet, stakers can see at all times how their price adjusted when other stakers left the queue.

As long as stakers stay staked throughout the entire pre-order period, their price can only move in their favor, since they move back down the sloping curve. This is a very powerful incentive for stakers to stay in the queue!

**3. Click into the deal**

At the end of the pre-order period, stakers will automatically be issued the number of tokens equivalent to the amount they staked divided by their final pre-order token price, as calculated above.

The cut-off date and time will be clearly announced and - at least in our proposed implementation - anybody who remained staked up to that point will automatically see their stake convert into committed capital. They clicked into the deal.

**Get yourself sorted!**

What this deal precisely entails is entirely up to the sponsors of the project to decide.

The idea here is very much that the pre-order period gives project leads sufficient time to work on deal terms with early stakers and communicate with the community at large about what they will do with the committed capital in the next phase for the project, including figuring out the legals and regs.

This design gives full freedom to future users to at that stage determine if for instance:

* tokens will automatically flow to the wallets of participants since there is no need to whitelist them. This would be the case for projects that do not issue a security token, such as OtoCo;
* or there’s a hold period during which everybody will be asked to whitelist and accredit e.g. under a Reg D+S type security token offering. In such case, there would also need to be a way for the sponsor to return funds to those participants who do not cooperate or otherwise fail to whitelist, and future versions of our smart contract may cater for this.

