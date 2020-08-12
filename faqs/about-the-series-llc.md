---
description: This section answers common questions regarding the Series LLC.
---

# About the Series LLC

## How is a Series LLC established?

A Series LLC is created when the Master creates the smart contract that holds that Series' LLC Operating Agreement \(the "Agreement"\).

This smart contract is created by signing a transaction on the Ethereum blockchain which triggers`otoco.eth.`

This `otoco.eth`contract contains the  Master LLC Operating Agreement which derives its authority to establish Series LLCs directly from the Act, e.g. in the case of Delaware: 

> Pursuant to Section 18-215\(b\) of the Act and the Limited Liability Company Agreement of the Master LLC \(the "Master LLC Agreement"\), the Master LLC is authorized to establish separate members and limited liability company interests with separate and distinct rights, powers, duties, obligations, businesses and objectives \(each a "Series"\).

After the transaction confirms, typically , the Series LLC Operating Agreement is signed with the public wallet address of the sender, which legally becomes the LLCs first Member.

The Agreement makes sure that equivalence is given to the use of a user's private key with his/her digital or wet signature. 

> Any signature or execution made through the use of private keys on the blockchain for any matters relating to the Company shall be valid, as if signed in writing.

As a result, the individual Series LLC is owned by the smart contract created by the Master.

## How is an individual Series insulated from other Series?

The principle that one individual Series cannot be contaminated by what happens in the other Series LLCs under the Master is the very reason why Delaware and other States in the US created the Series LLC structure.

In a traditional context, the Master is typically the "sponsor" of a common project that requires individual LLCs for each asset held, e.g. individual properties financed by the same sponsor who is typically Member in each of the LLCs.

However, there is no requirement for the Master to be a Member in the individual Series LLCs and in our setup, the Master is expressly excluded from Membership.  Also, there is no requirement for the individual LLCs to have any communality.  In our setup, the Series will not even know of each other's existence since in Delaware \(in contrast with e.g. Wyoming\) there is no need to report the names of the individual Series LLCs in the Annual Filing by the Master.

Such structure could not work if there is any risk of cross-contamination, and this key operating principle is expressly articulated in the Agreement.

> \[...\] 
>
> none of the debts, liabilities, obligations and expenses incurred, contracted for or otherwise existing with respect to the Master LLC generally or any other Series of the Master LLC will be enforceable against the assets of the Company. A member participating in one Series will have no rights or interest with respect to any other Series, other than through that Member's interest in that Series independently acquired by that Member. This Agreement and all provisions herein will be interpreted in a manner to give full effect to the separateness of each Series.

and further down in Article II:

> The dissolution and termination of the Company will not, in and of itself, cause or result in the dissolution or termination of the Master, LLC or any other Series.

## Is the Series LLC a legal entity in its own right?

Categorically yes. Your LLCs is entirely independent from other Series LLCs: it has its own Members, Managers, assets and liabilities, just like a normal LLC.  

As a result, whatever happens to the other Series LLCs will not affect your LLC.

## What are the benefits of a Series LLC over a single LLC?

The advantages of the Series LLS is that you have a valid legal entity that can be spun up immediately, fully online and at very low cost: 

* You do not have to make any filing to form your LLC.
* Your LLC will be spun up with a ready Operating Agreement rather than having to instruct and pay a lawyer or service provider to draft one for you.
* You do not have to pay the Delaware or Wyoming Annual Franchise tax since only the Master, resp. OtoCo DE LLC and OtoCo WY LLC, pays the tax, not the individual Series.
* Your LLC is automatically given a Delaware address.  For a small extra fee you can have Otonomos provide a business address in all major US States where you can receive physical mail and have it scanned to you.
* The LLC is also entirely private: there is no public filing of a Certificate of Formation with the name of the first Member and Manager.
* Finally, the LLC can also be entirely anonymous if setup via Otonomos: as long as the address you use to spin up your LLC is not whitelisted, your identity will not be publicly linked to the ownership of the LLC \(see below "How about identity"\). 

All this improves significantly on the speed, costs, maintenance and privacy of the traditional LLC, which typically takes 2 days to form and a couple of hundred dollars in setup costs and annual maintenance. 

## What does it cost to setup my LLC with Otonomos?

It is FREE until September.  Pricing from September on will be announced soon and whilst no longer free it will be cheap. 

## What are the typical use cases for an LLC?

Its low price and instantaneousness makes our OtoCo LLC product ideally suited as a vehicle to hold physical assets e.g. real estate but also digital property such as patents, trademarks and copyright.

We also see high demand for the LLC as an instant limited liability wrapper around  smart contracts, reducing the legal risk to developers of self-executing code.  

Finally, the LLC can also be a fully operational entity in its own right with offices and staff etc.

## Ok, how do I proceed and spin up an LLC with Otonomos?

For now, spinning up and LLC is FREE until September.  From then on, you ill have to send a set amount of stablecoin \(DAI\) to `otoco.eth` to instantly activate your LLC.  We will shortly announce detailed pricing: whilst it won't be free anymore, it will be cheap.

## What are the steps involved?

There are only a few steps:

1. First, you enter the name you have in mind for your LLC to check its availability.
2. If the name is available, just connect your wallet you want to use and sign a transaction on the Ethereum mainnet \(soon this will be a payment of a set amount of DAI\). Note that this address will be the address that controls the smart contract that is created for your LLC. You pay for the gas fees of the Ethereum blockchain.
3. After confirmation of your transaction, your company will typically activate within 5 seconds.  The address for your LLC smart contract will show and you will be able to download an executed copy of its Operating Agreement from the Dashpanel.

## Can I chose any name for my LLC?

Yes as long as the name is not yet taken.  This is why we first perform a name check \(see previous FAQ\).   

The chosen name will appear on the cover page of the LLC's Operating Agreement. The business of the Company may be conducted under that name or under any other name that the Manager may determine. 

Under the Delaware Act regarding Series LLCs, there is no obligation though it is standard practice to refer the Master when using the LLC's offical name.  

E.g. for Acme LLC, in Delaware conventional naming would typically be: `Acme LLC, a Series of OtoCo DE LLC` however there is nothing in the Act that prohibits the use of the Series LLC by its individual name, `Acme LLC.`

In Wyoming, naming is more restrictive and a Series LLC's full legal name would be in the following format:  `OtoCo WY LLC - Acme - Series [Number of Series]` however users can do business as "Acme". To see their trade name protected, they would want to file a Doing Business As \(DBA\) with State Registry which Otonomos can help file.

## How does this work at the blockchain level?

There's two smart contracts at work and a fair bit of legal engineering.

Simplified, signing of a transaction \(eventually, receipt of stablecoin activation payment\) to the Master smart contract for OtoCo prompts the Master to create a new smart contract for every individual Series LLC.

Your Series LLC smart contract is controlled by the wallet you used to sign the tx/send the DAI.  This means that the first Member of the LLC is effectively a wallet address, since it is that address that signed the new LLCs Operating Agreement. 

The smart contracts are fully open source and can be found on our [github](https://github.com/otocorp).

## Is there an expiry date on my LLC?

No.  Its term is indefinite until terminated in accordance with the provisions of the Series LLC Operating Agreement. 

## Under what circumstances can termination happen?

There are four circumstances:

1. the final Distribution of the net assets of the Company to the Members or a Liquidating Vehicle in case of an involuntary winding-up;
2. the dissolution of the Master LLC;
3. a voluntary winding-up; or
4. entry of a judicial decree of dissolution of the Company pursuant to the Act.

## What happens upon the "dissolution of the Master LLC"?

The Master is automatically dissolved if there are no individual Series left.

If there are any issues that may result in the dissolution of the Master LLC whilst there are still Series LLCs, the Master will undertake reasonable efforts, to the extent legally allowed, to notify each Series so they can take appropriate measures.

## Where does my LLC have its office?

You can chose any address as your principal office, also outside of the US, subject to local rules.  Inside the US, specific regulations may apply in the State where you have your principal office.

The Registered Agent, i.e. Otonomos LLC or its appointed agent, is the LLC's registered agent for service of process, as per the [Series Operating Agreements](../operating-agreements/untitled.md).

## What purpose can my LLC have?

You can engage in any lawful activity.

## Can Member's capital be paid up in crypto currencies?

Yes. 

Article IV of the Series LLC Operating Agreement deals with Membership Capital, and most provisions reflect common practice across all LLCs.  It expressly provides that the Manager, in its sole discretion, may accept Digital Assets as a Member's Capital Contribution.

## Can I change Otonomos as Registered Agent?

Otonomos LLC as Registered Agent on file for the Master LLC has an obligation to be able to receive process for each Series LLC.  You would hence need to convert your Series LLC into a full stand-alone LLC with its own Registered Office if you would no longer want Otonomos LLC to be the process agent.

## Who files my Annual Report?

A Series LLC is for all intents and purposes a full legal LLC and hence the Series LLC's Manager will be responsible for the preparation of its Annual Report.

Otonomos can help with the actual filing but does not provide tax services.

## Can I open a bank account for the LLC?

Yes. As with a traditional LLC setup an Entity Identification Number \("EIN"\) will be required which you can obtain directly from the US Internal Revenue Service or which we can obtain on your behalf.

## What about identity and KYC?

In the US, Members of LLCs to do not have to provide attestation of their identity _at the moment of formation_ of their LLC.

The Certificate of Formation of an LLC does not mention its first Member\(s\), ony the Operating Agreement and the latter is a private document.  

In the case of a protected Series LLC, there is no filing of a Certificate of Formation, only a signing of the Series LLC's Operating Agreement.   

When such protected Series LLC is spun up via our smart contract technology, its Operating Agreement does not have the first Member\(s\) names but only the public address of the wallet they chose to activate their LLC with. 

## So this means I can set up my LLC entirely anonymously?

If you work on the assumption that blockchains are anonymous and the wallet you are using is not traceable to your real-world identity, then indeed your LLC can be formed and remain entirely anonymous. 

However, this may limit its actions in the real world: attestation of identity of ownership of the controlling wallet may kick in e.g. when the Series LLC is looking to open a bank account, or - depending on the applicable regulations - when its first Member looks to transfer part of its ownership interest.

Banks may ask for a Certificate of Incumbency, which would require your LLC to become _registered_ \(vs. _protected_\) in Delaware.  This is a simple process involving a filing and we would be happy to help.

Crypto-currency exchanges have varying degrees of KYC and may want to see a copy of the Operating Agreement. 

## Does Otonomos provide additional services to my LLC?

Yes we can help with various services, from a prestigious office address with mailscan to governance and Member agreements once your LLC has more than one Member.

In addition to offering OtoCo for C-Corps and in more jurisdictions, our technology roadmap includes adding layer after layer of blockchain solutions for all pain points in the LLC, from tokenizing and transferring Member interests to a genuine online crypto banking solution for your LLC. 



















1. 
