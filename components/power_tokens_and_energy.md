---
layout: default
title: Power Tokens and Energy
nav_order: 1
parent: How IQ Protocol Works?
---

<!--

Page meta:
- Goal: Explain how it works.
- Status: This is a dump of ideas, worse than a draft. Add. Distill. Proofread.

-->

Power Tokens and Energy
================================================================================

**Power token is a token that generates utility over time.**
Some examples of Power Tokens:
- Farmer sells tomato Power Tokens that represent 1 kg/day tomatoes with decay of 1 day half-life.
- CheapISP sells ISP Power Tokens that represent 1 MB/s internet with instant decay.
- ExpensiveISP sells ISP Power Tokens that represent 1 MB/s internet with a decay of 1 day half-life.

Power Enterprise sets a **global configuration** with 4 base properties for Power Tokens issued by it.
Based on the chosen payment method it can have more properties.
When configuration changes it is retroactively and instantly effective for all Power Tokens of the Power Enterprise.

Base Configuration:
- Definition of **underlying utility** (e.g. tomatoes)
- **Unit size** of 1 token (e.g. 1 kilogram)
- **Half-life** period (e.g. one day)
- **Delivery Frequency** (e.g. once per day)

When Power Enterprise sells its Power Tokens, it adds an additional parameter - expiry date (e.g. Feb 20, 2021, 18:00 UTC).
This is the only property that might differ from token to token.
If Power Tokens of the same Power Enterprise have the same expiry date, they are fungible.
Similar to milk in the shop, we consider two milk bottles equal even if they have different but not yet expired "best before" dates.
Power Tokens of different expiry dates are equal in all other aspects except expiry date.

Definition of **underlying utility** (good or service) contains the **type** (e.g. tomatoes) of it according to some standard classification, as well other type-specific details (e.g. dispatch location, working time, etc.).
Power enterprises can define them as anything they wish as long they can deliver it.
Community initiatives should translate current industry practices into guidelines and standards to ensure that goods and services are **comparable**, as well should shun excessive or creative bundling of goods.

**Unit size** is the amount of utility that is represented by 1 token.
In theory it can be anything, but in practice it should be a unit in the SI system to make it easy **comparable.**

**Half-life** property is a versatile variable that standardizes the approach to the problem of "saving up for later".
More on it below at "Energy".

**Delivery Frequency** is a versatile variable that solves a practical problem of logistics - if a farmer doesn't want to send a tenth of a tomato every minute it should better set it to daily, monthly or anything in-between.
Furthermore, it also doubles as a buffer time to deal with onboarding - consumers have the right to collect goods or services only **after** the Delivery Frequency has passed.
On the other hand, power enterprises like ISP can set it to "instant and continous" by using a value zero.




Retained Consumption Power (RCP)
--------------------------------------------------------------------------------

Unused utility from Power Tokens may be retained.
The extent to which RCP is controlled with **Half-life** property.

In the example of tomatoes above that have a half-life of 1 day, it means that if you don't collect tomatoes today then you can collect one and a half of them tomorrow (half saved from today and one whole from tomorrow).
The difference between two ISP providers illustrates it better.
Let's say you haven't used the internet all night and in the morning need to quickly download a huge file.
In the case of qCheapISP, you would download them only at 1MB/s because qCheapISP doesn't save any unused internet from the night.
On the other hand, with qExpensiveISP you would have accrued ~18k Retained Consumption Power (RCP) over the 8 night hours.
Within the connection limits, in the morning such RCP provides rights to theoretically consume 18 GB/s for one second, 2.4 GB/s for one minute, or 40 MB/s for one hour.
As you can see, bigger half-life is better for consumer, *as well sleeping is good for internet speed :)*.
Half-life quantifies "flexibility" of the service that enables **comparability** of otherwise similar services.


Power Enterprise
--------------------------------------------------------------------------------

**Power Enterprise** is an on-chain account that is able to publish configuration and mint power tokens.
Power enterprises can provide one or many services, each with its own separate power token.
There can be two kinds of it: blockchain-native or representations of real-life entities.

Blockchain-native Power Enterprise are elaborate smart contracts, which combine various smart contracts into one - governance & voting, power tokens, and custom equity funding - as well as means to withdraw funds to cover operational costs.

Real-life entities are a combination of simple multisig smart contracts with power token smart contracts, where one or more representatives of the real-life entity holds the signing rights.
That entity may or may not collect on-chain payments for the power tokens - in the former case it just gifts appropriate power tokens according to the off-chain payments to mirror the current state of affairs.

To facilitate standardization, the power token concept can be generalized to accommodate franchising - that is, instead of power enterprise (franchisee) publishing configuration with it's own values, it simply instead links to configuration of another enterprise (franchisor), effectively copying it, including all future edits.
This idea can be expanded further to accommodate various compensation schemes between franchisee and franchisor.




Future
--------------------------------------------------------------------------------

The concept of Power Tokens may be implemented at a blockchain protocol level.
Obviously it could be used for covering the transaction fees.
But the kicker is the emergence of a powerful new feature - smart contract ability to reactively pay transaction fees.
That would enable to react to other on-chain events, enabling unseen flexibility of smart contracts.
