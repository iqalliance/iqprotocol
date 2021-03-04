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

It turns out that such change to subscription-first perspective provides immense performance gains in the blockchain context, by enabling the off-loading of the majority of transactions away from blockchain itself.
In the best case scenario many transactions are not required anymore, but in the worst case scenario the same amount of transactions would be offloading to a special off-chain state channel called [DvP channel](./dvp_channels.md).
Such gains are possible because all involved parties are able to depend on a mutually trusted and shared "service" - the time itself.
The trade-off is that all parties require access to precise time, which should not be a problem in the modern world.
