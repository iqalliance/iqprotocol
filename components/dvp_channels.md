---
layout: default
title: DvP Channels
nav_order: 2
parent: IQ Protocol Components
---

TODO: This is a dump of ideas, worse than a draft. Add. Distill. Proofread.

Goal for page: explain dvp channels - what problems they solve, and when they are optional.

****

DvP channel stands for Delivery-versus-Payment channel, that technically is special-purpose off-chain state channel.
It is established between power enterprise and consumer for the purpose of accounting and audit trail.
The communication between both parties is end-to-end encrypted, chained together and signed by either party.

Parties communicate through DvP channel with messages.
Furtermore, it is assumed that continuation of conversation implies accepting the other party's claims so far.
The majority of messages would be consumer's requests and delivery confirmations and provider's status and RCP updates.
The minority of messages would be challenges to the other party's claims and reconsilation.
This way if a dispute arises, the audit trail would facilitate the case in the court.
At the very least, the audit trail give a weight to anonymous service reviews on online platforms.

Although DvP channels will have standardized messages, in essence it just synchronizes current RCP between the parties and thus is very flexible to accommodate for discounts, promotions, refunds, credits, penalties, trials, etc.

Communication Platform will be needed to facilitate DvP channel discovery and communication.
It would look like an end-to-end (E2E) chat application with the ability to browse all Power Enterprises on-chain, start a (normal or DvP) conversation with them, and have pre-built message templates for DvP channel needs, as well an ability to create, send, and verify received proofs.
Under the hood, the Communication Platform is more a combination of chat app and blockchain wallet and IPFS explorer.
For the Server part of Communication Platform, it will have a strong API to support automation and facilitate proliferation of bots, integrations and alternative end-user apps.
