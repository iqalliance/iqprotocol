---
layout: default
title: How IQ Protocol Works?
nav_order: 1
has_children: true
---

<!--

Page meta:
- Goal: summary of IQ Protocol works.
- Status: This is a dump of ideas, worse than a draft. Add. Distill. Proofread.

-->

How IQ Protocol Works?
================================================================================

The Power Token concept changes the perspective on economic relationships from transactional-first to subscription-first.

**Power Token generates utility over time.**
In contrast, conventional normal tokens represent only utility.

For example, the conventional "tomato token" would represent rights to collect 1 kg of tomatoes, whereas a Power "tomato token" (with weekly flow and expiry in 1 year) would represent a right to collect 1 kg of tomatoes per week for a year.

Such perspective facilitates product-as-a-service models.

****

It turns out that such change to subscription-first perspective provides immense performance gains in the blockchain context, by enabling the off-loading of the majority of transactions away from blockchain itself.
In the best case scenario many transactions are not required anymore, but in the worst case scenario the same amount of transactions would be offloading to a special off-chain state channel called DVP channel.
Such gains are possible because all involved parties are able to depend on a mutually trusted and shared "service" - the time itself, but he trade-off is that all parties require access to precise time, which should not be a problem in most cases.

The performance gains apply to fungible goods/services and/or subscription-alike relationships, but for non-fungible goods (unique objects) we will have to resort to conventional tokens.
Therefore to maximize overall performance, we will assume that all kind-of fungible goods (e.g. tomatoes, etc.) are fungible goods, which leaves us with very few non-fungible goods (e.g. land, buildings, cars, etc.).
All critical infrastructure services, like computing (blockchain fees) and storage (IPFS pinner fees) are essentially fungible services and thus can easily benefit from Power Tokens and DvP channels.
<!-- TODO: definition of "fungible service" -->
