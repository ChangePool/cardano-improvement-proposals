# It Takes a Village

## Preamble

---

Title: It Takes a Village  
Author: Paradoxical Sphere <support@paradoxicalsphere.com>  
Cardano Stake Pool: [Change](https://change.paradoxicalsphere.com)  
Status: Draft  
Type: Process  
Created: 2022-11-15  
License: [DMCA](https://www.dmca.com/r/69428j8)  

---

## Abstract

<p align="center">
  <code>"I think one of the things that people need to stop doing is asking, 'What is the ultimate blockchain?'...<br>
In my opinion, it doesn't exist because it really depends."</code>
</p>
<p align="center">
<code>—<a href="https://cointelegraph.com/news/the-best-blockchain-does-not-exist-cardano-foundation-exec">Mel McCann</a>, Vice President of Engineering, Cardano Foundation</code>
</p>
<!-- <p align="center">
<code>—<a href="https://nationworldnews.com/cardano-foundation-official-says-there-are-different-use-cases-for-different-blockchains/">Mel McCann</a>, Vice President of Engineering, Cardano Foundation</code>
</p> -->

Are you interested in responsive, emergent, collaborative and sustainable governance for Cardano, to help Cardano not only survive but thrive based on <b>human values</b>? The Cardano protocol is a means to economy—not an end—and is not perfect. With appropriate governance, the protocol may not require perfection.<sup><a href="#dependency">1</a></sup>

<p align="center">
    <img src="https://github.com/paradoxicalsphere/cardano-improvement-proposals/blob/67ec3da1c085f86ae2ae9f74548a5c9ff5463973/CIP-x/images/Here%20to%20Help.png" alt="" title="">
    <br>
    <i>Figure 1 - <a href="https://xkcd.com/1831/">Here to Help</a></i>
</p>

Currently, the supply of stake pools exceeds the demand from delegators. Creating increased demand to meet the supply produces a net effect of growing the Cardano economy. The current proposal aims to improve and enhance governance of the stake pool operator (SPO) community with the help of Input Output (IO), Cardano Foundation (CF) and EMURGO employees including the support of their employers as well as the Cardano community.

Prior to reviewing the current proposal further, please watch the following videos:

* [Empowering Community-Driven Governance on Cardano](https://www.youtube.com/watch?v=YvTfSx6pv9Y) (December 2022)<sup><a href="#mbo">2</a></sup>
* [Essential Governance: Building Strong Blockchain Foundations](https://www.youtube.com/watch?v=lHlofcMNNo8) (November 2023)
* [What Would It Take to Actually Trust Each Other?](https://www.youtube.com/watch?v=r54-jjAKEuE) (January 2026)

<a name="dependency"></a><sup>1</sup> The current proposal incorporates research conducted by the [Center for Humane Technology](https://www.humanetech.com/). Decision-making processes based on token-weighted governance, such as [CIP-1694](https://github.com/cardano-foundation/CIPs/tree/master/CIP-1694), are out of scope for the current proposal. **The current proposal suggests a complementary approach to mitigate risks associated with token-weighted governance models, in which users with the most tokens have the biggest share of voting power, by refining how the stake pool delegation mechanism—on which the DRep delegation mechanism that CIP-1694 introduces is based—is incentivized.**

<a name="mbo"></a><sup>2</sup> The video refers to the Cardano Member-Based Organization (MBO), also known as [Intersect](https://www.intersectmbo.org/).

## Motivation

Imagining a better world without Cardano is possible. Building a better world with the help of Cardano may be preferable. In 1977, Hubert Humphrey, who served as US Vice President from 1965 to 1969, said, "The moral test of government is how that government treats those who are \[most vulnerable\]."<!-- https://atkinsbookshelf.wordpress.com/2018/02/21/famous-misquotations-a-civilization-is-measured-by-how-it-treats-its-weakest-members/ -->

Changing the world without people changing is impossible. Trustless systems are meant to build trust.

Central in the design of the Cardano protocol is [mathematical game theory](https://cardano.org/ouroboros/). In [mathematical game theory](https://en.wikipedia.org/wiki/Game_theory), the [Prisoner's Dilemma](https://www.youtube.com/watch?v=mScpHTIi-kM) is a standard analyzed example.

As William Poundstone describes in the book [_Prisoner's Dilemma_](https://www.worldcat.org/title/23383657), two members of a criminal gang are arrested and imprisoned. Each prisoner is held in solitary confinement with no means of speaking to or exchanging messages with the other. The police admit that they do not have enough evidence to convict the pair on the principal charge. They plan to sentence both to a year in prison on a lesser charge. Simultaneously, the police offer each prisoner a self-defeating bargain. The possible outcomes are:

- If Prisoner A and Prisoner B both defect—that is, betray each other—then each prisoner serves two years in prison.<sup><a href="#betray">3</a></sup>
- If Prisoner A betrays Prisoner B and Prisoner B remains silent, then Prisoner A will be set free and Prisoner B will serve three years in prison.
- If Prisoner A remains silent and Prisoner B betrays Prisoner A, then Prisoner A will serve three years in prison and Prisoner B will be set free.
- If Prisoner A and Prisoner B both do **not** defect—that is, Prisoner A and Prisoner B both do **not** betray each other—and both remain silent, then both prisoners will serve one year in prison (on the lesser charge).

Communication between the Cardano stake pool operator community and employees of Input Output, Cardano Foundation and EMURGO is limited. Also, IO, CF, EMURGO and the SPO community share a common interest in achieving Cardano's success.

Based on the Prisoner's Dilemma, where the SPO community may be represented as Prisoner A and employees may be represented as Prisoner B, or vice versa, the current proposal aims to achieve an outcome based on trust, mutual benefit, cooperation and coordination for each "prisoner" as well as in the relationship between "prisoners," rather than an outcome based on self interest.

Often, discussion of the Prisoner's Dilemma seems to focus on logic or the outcome of a single interaction, overlooking how an outcome of a dilemma may affect the world view and relationships for involved "prisoners" in possible subsequent interactions, with ongoing potential for entrenching and escalating patterns of betrayal—or for building trust—over time.

<a name="betray"></a><sup>3</sup> For example, the suggestion to [burn all of the funds in the treasury](https://www.youtube.com/live/57d2_Knd4mI) (September 2024) encourages betrayal.

## Specification

The current proposal, **emerging from the Cardano community** in the Voltaire era of independent governance, begins to explore the potential for a process change empowering employees of the founding entities—Input Output, Cardano Foundation and EMURGO—with discretionary (t)ADA<sup><a href="#tada">4</a></sup> to delegate to stake pools in the Production (Mainnet) environment as well as any and all testing environments. In other words, the process change would make (t)ADA available to each IO, Cardano Foundation and EMURGO employee only for delegation to one or more stake pools based on the judgement of the individual employee.<sup><a href="#employees">5</a></sup> <b>The process change aims to increase decentralization, transparency, agility and scale, potentially, of delegations to stake pools and related decisions that founding entities currently may make, and/or have made in the past. Funds that employees may delegate are investments that earn awards according to the Cardano protocol.</b>

To find a balance that may help vitalize employees as well as the SPO and wider Cardano communities without introducing risks to the security of Cardano networks or any other potential forms of instability, <b>analysis, evaluation, planning, elicitation, collaboration, design, management and communication are needed from Input Output, Cardano Foundation and EMURGO to gain knowledge in support of the proposed initiative in order to complete a proposal capable of garnering sufficient community understanding and consensus to progress towards becoming operational.</b>

For example, questions such as the following must be addressed:

- How much (t)ADA in total may be available for such an initiative?
- What may be the source(s) of (t)ADA available for such an initiative?
- Within such an initiative, what may be the limits of delegation for an employee?
- What requirements may include or exclude employees from delegating?
- How may awards that delegations may receive be managed? By whom?
- How may existing or new workplace contracts, agreements, guidelines, codes of conduct or practices between employer and employee apply to such an initiative?
- What record keeping or know your customer (KYC) requirements may apply to such an initiative?
- How long must any records be kept?
- Who may access records kept in support of such an initiative?
- How is privacy protected?
- When required, how may records be securely destroyed?
- How may the potential or need for changes or adjustments to the operational guidelines for such an initiative be managed?
- What aspects of such an initiative may be administered using smart contracts?
- Would such an initiative affect existing delegation strategies that Input Output, Cardano Foundation and EMURGO currently may practice, and if so, how?
- How may organizations or institutions involved be set up to satisfy all legal and regulatory requirements?<sup><a href="#legal">6</a></sup>

<a name="tada"></a><sup>4</sup> Whereas ADA is the digital currency of the Cardano Production (Mainnet) environment, tADA is the digital currency of testing environments. The current document refers to Cardano digital currencies collectively as (t)ADA.

<a name="employees"></a><sup>5</sup> The current proposal does not restrict whether employees may already serve in existing roles within the respective organizations, or be newly hired explicitly or solely for the purposes of fulfilling roles related to delegating discretionary (t)ada to stake pools.

<a name="legal"></a><sup>6</sup> For information on some organizational and institutional designs that seem to warrant further investigation in order to develop the current proposal further, see the <a href="#resources">Resources</a> section.

## Rationale

The following primary stakeholders are identified:

- The Cardano community
- Input Output
- Input Output employees
- The Cardano Foundation
- Cardano Foundation employees
- EMURGO
- EMURGO employees

With further stakeholder engagement and research, over the longer term perhaps the current proposal may support the creation of a form of [decentralized autonomous organization](https://legalnodes.com/article/swiss-foundation-dao-legal-wrapper) (DAO) for Input Output, Cardano Foundation and EMURGO employees to help with governance of the SPO community.

In token-weighted governance models, tokens are considered more important than people. Sasha Ivanov, a theoretical physicist by background, founded the [Waves](https://waves.tech/) blockchain platform in 2016.<sup><a href="#connection">7</a></sup> In the article [DAOs Will Never Work Without Fixing Governance](https://cointelegraph.com/news/daos-will-never-work-without-fixing-governance) published in September 2022, Ivanov identifies the following primary risk associated with DAOs in practice:

<b>Token-weighted governance, in which users with the most tokens have the biggest share of voting power, can inadvertently end up handing over control to a few wealthy participants and stripping it away from the many.</b>

To mitigate the aforementioned risk, in the current proposal—as part of an initiative to allocate an amount of (t)ADA to employees solely for the purpose of potential delegation to one or more stake pools based on the judgement of the individual employee—Input Output, Cardano Foundation and EMURGO as employers regulate weighted voting and tokenomics, establishing constraints at the management level to maintain a balance of voting power. Employee roles and responsibilities include the potential to delegate (t)ADA based on the terms and conditions of employment. In workplaces, managing roles and responsibilities while empowering employees to complete their day-to-day activities and duties successfully is a fundamental existing requirement.

In his article, Ivanov also identifies the following opportunities. The list also explains how the current proposal aims to realize each opportunity:

* <b>DAOs have been heralded as the future of governance, unlocking a more egalitarian approach to decision making</b>—The current proposal offers an approach for further decentralizing existing decision-making processes within Input Output, Cardano Foundation and EMURGO organizations related to stake pool delegations.
* <b>A voting structure based on meritocracy may be just what is needed</b>—[Meritocracy](https://en.wikipedia.org/wiki/Meritocracy) is "a system, organization or society in which people are chosen and moved into positions of success, power and influence on the basis of their demonstrated abilities and merit." Within the framework of a workplace, rewarding successes in achieving goals set for performance is a form of motivation. In relation to the current proposal, Input Output, Cardano Foundation and EMURGO may seek to reward employee contributions meeting or exceeding expectations with increased benefits and responsibilities related to allocation of discretionary (t)ADA solely for potential delegation to stake pools, for example.
* <b>Imagine a new model, one where voting members are assessed against certain key performance indicators (KPIs) [involving] engagement and development metrics within the DAO<!--... a failure to meet these KPIs can result in that user’s voting power being reduced or removed entirely--></b>—[KPIs](https://www.qlik.com/us/kpi) are "quantifiable measures of performance over time for a specific objective [providing] targets for [individuals and] teams [within organizations] to aim for; milestones to gauge progress; and, insights that help people across the organization make better decisions... [KPIs] help every area of the business move forward at the strategic level." Within organizations and workplaces, KPIs are commonly in use. Existing organizational structures within Input Output, Cardano Foundation and EMURGO may provide a foundation well suited for implementing KPIs designed to enable and support the continuing operation of a stable DAO. As Ivanov points out, assessing employees against certain KPIs potentially encourages all entities to make decisions that are in the broader interest of the community, not just themselves.

<p align="center">
    <img src="https://github.com/paradoxicalsphere/cardano-improvement-proposals/blob/656c36911185cd7ac78460b3a68edfe26593b6de/CIP-x/images/DAOs%20Within%20Workplaces.png" alt="" title="">
    <br>
    <i>Figure 2 - The Organizational Structure of an Incorruptible DAO Within the Workplace</i>
</p>

<a name="connection"></a><sup>7</sup> For example, EMURGO and Waves both partner with the [Ergo Platform](https://ergoplatform.org/).

## Example Use Cases

### Participating in On-Chain Polling

As explained in the article [Entering Voltaire: Poll Experiment Live on Mainnet](https://cardanofoundation.org/en/news/entering-voltaire-poll-experiment-live-on-mainnet/), the on-chain polling mechanism implemented via [CIP-0094](https://github.com/cardano-foundation/CIPs/tree/master/CIP-0094) introduces an elegant mechanism to hear the voices of (t)ADA holders: "After the [poll or survey] question gets published, SPOs will have until the end of the next epoch to vote. A period of two additional epochs will then give stake delegators the time to consult the dashboards, see how [or whether] SPOs voted, examine the results, and decide whether or not to redelegate their stake to another SPO."

Over time, the on-chain polling mechanism may serve to create a space where shared understanding within the (t)ADA-holding community grows and improves.<sup><a href="#questions">8</a></sup> <b>Presenting data without first requiring a decision about which parameters to use and how to apply them to interpret or analyze the data may help create robust mechanisms for governance participation.</b>

The current proposal may introduce an opportunity for employees to participate in the delegation or redelegation phase of on-chain polls or surveys using discretionary (t)ADA.

<a name="questions"></a><sup>8</sup> The development of poll or survey questions is out of scope for the current proposal.

### Addressing the Unintended Consequences of Multiple-Pool Operators

The article [Multiple Stakepool Operators are Harming Cardano](https://adapulse.io/multiple-stakepool-operators-are-harming-cardano/), published in February 2022, describes the challenge associated with stake pool operators who register multiple pools as follows:

<blockquote>
The increasing centralization of the network by a handful of entities is eroding the value of the ecosystem, and it might never come back...
    <br /><br />
Cardano wants to assign blocks to entities proportional to how much "skin in the game" they have, and what their standing is in the community. In this way, hopefully, only people who have a lot to lose if they were to maliciously misrepresent the transaction data get assigned the blocks to process. However, if you don’t occasionally give new people a chance to showcase their loyalty to the network, power begins to concentrate to a handful of early adopters. To that end, stake pools reach a saturation level at around 67 million ADA, so the expected rewards per minted block go down. This is to incentivize [delegators] to go elsewhere.
    <br /><br />
Nevertheless... there’s naturally the incentive [for stake pool operators] to open more than one [pool]... the problem is that this becomes a positive feedback loop: you’re able to afford more marketing... and you’re able to fill more pools to saturation, which gets you even more resources and thus you can expand your operations...
    <br /><br />
The success of a large multi-pool stake pool necessarily means that someone is worse off. There will only ever be 45 billion ADA, so this hard cap means that every time a delegator decides to go with an SPO, every other SPO on the network loses potential revenue (assuming that they don’t already have a saturated pool and don’t have any intentions of opening a new one).
    <br /><br />
In economics terms, this would be called a "Zero Sum Game," as in a situation where the success of one person necessarily means everyone else that participates is worse off. Think of it as having a slice of cake. Every time you take a slice, that means someone else can't have that same portion... Much as we already saw in the real world where entities like Walmart crushed Mom & Pop stores, the same is bound to happen in Cardano... If we simply recreate the tyrannies of the past but ON THE BLOCKCHAIN, what’s really the point?
    <br /><br />
It is with this backdrop that it becomes particularly heinous when stakepool operators just keep opening multiple pools. They’re essentially robbing opportunity from new entrants, thereby centralizing the system and making everyone worse off in the long term, because they are trying to extract as much value as they can for themselves.
</blockquote>

Using an implementation of the current proposal to address the unintended consequences of multiple-pool operators, in a scenario where the number of SPOs operating multiple unsaturated stake pools may be identified as centralizing or introducing fragility into the Cardano ecosystem "too much," on individual, cooperative or collective bases employees may delegate or redelegate discretionary (t)ADA to stake pools identified as single-pool operations for example—within the constraints established by the founding entities Input Output, Cardano Foundation and EMURGO—to maintain or restore a balance of decentralization and resilience within the network.

## Backwards Compatibility

To be determined

## Path to Active

The current proposal introduces a requirement for a new type of [wallet address key pair](https://developers.cardano.org/docs/operate-a-stake-pool/cardano-key-pairs/#wallet-address-key-pairs).<sup><a href="#wallet">9</a></sup> Wallet addresses assigned the new type are included in a closed set—a subnet—of wallet addresses. Support for multiple closed sets is required. Wallet addresses included in a closed set belong to exactly one closed set, and no more. A closed set may include many unique wallet addresses. Wallet addresses in a closed set may only send (t)ADA to or receive (t)ADA from wallet addresses included in the same closed set. Wallet addresses belonging to a closed set maintain the existing functionality to delegate the wallet to a pool and receive awards using a staking address.

To implement the current proposal, employees must maintain a professional ethical relationship with stake pools and stake pool operators.<sup><a href="#ethics">10</a></sup> Each employee is assigned a unique closed set of wallet addresses. Closed sets, as well as the public verification key files for payment and stake addresses of wallet addresses belonging to closed sets, may be shared publicly and transparently.<!-- <sup><a href="#private">4</a></sup> --> The private signing key files for a wallet address belonging to a closed set are accessible only to the employee assigned the wallet address and to the employer.<sup><a href="#secret">11</a></sup>

For the employer to administer the new type of wallet address, the current proposal also requires implementation of new mechanisms to:
* Create closed sets
* Uniquely assign a closed set to an employee
* Add wallet addresses to closed sets<sup><a href="#addwallets">12</a></sup>
* Remove wallet addresses from closed sets<sup><a href="#removewallets">13</a></sup> <!-- Add wallet addresses to—or remove wallet addresses from—closed sets -->
<!-- * Set strictly-enforced permissions for closed sets in terms of the other closed sets—or one or more specific wallet addresses that do NOT belonging to any closed set—allowed to send (t)ADA <b>to</b> wallet addresses in a closed set
* Send (t)ADA safely and securely <b>from</b> wallet addresses included in a closed set to one or more wallet addresses NOT belonging to any closed set without compromising the integrity of the closed set of wallet addresses—or (t)ADA balances of wallet addresses in the closed set—for the employee end user -->

Any smart contracts and related infrastructure that may support an implementation of the current proposal must enforce the existing definitions of closed sets.

<a name="wallet"></a><sup>9</sup> Each Cardano wallet address is comprised of a payment address and a staking address.

<a name="ethics"></a><sup>10</sup> For example, an employee delegating discretionary tADA to a stake pool that the employee operates in a testing environment is ethical. An employee delegating discretionary ADA to a stake pool that the employee, a family member or friend operates in the Mainnet environment seems unethical.

<a name="secret"></a><sup>11</sup> The private signing key files give access to monies in the wallet address.

<a name="addwallets"></a><sup>12</sup> Wallet addresses may carry zero or non-zero balances. Only the respective employee—NOT the employer—may send or stake (t)ADA from wallet addresses belonging to a closed set.

<a name="removewallets"></a><sup>13</sup> Only the employer—NOT the respective employee—may send or stake (t)ADA from wallet addresses removed from closed sets. <!-- <a name="private"></a><sup>4</sup> The relationships between closed sets may be private. -->

## Appendix: Distilling a Constitutional Framework Reflecting Useful Human Values

In the video [One Small Step for Cardano; One Giant Leap for the Industry](https://www.youtube.com/watch?v=rqvymw3gEeA) (September 2024) published on the day of the Chang hard fork, Charles Hoskinson directly or indirectly references the following useful human values (timings provided):

- Seeking happiness (00:04)
- Freedom of movement (00:10)
- Meaningful engagement and struggle (00:40)
- Functional society (2:30)
- Resisting support or promotion of war (05:35)
- Building trust (07:58)
- Having a voice (09:55)
- Developing identity (10:43)
- Accepting responsibility (11:32)
- Equality (18:00)
- Cooperation (18:20)
- Opportunity (20:02)
- Universality (20:59)
- Stability (21:12)
- Supporting education (24:46)
- Forgiveness (25:25)
- Access to good health care (25:54)
- Practicing gratitude (29:28)

As in the year 2024:

1. The world is currently experiencing dysfunctional tension on a path towards World War III, and
2. Dysfunctional tension holds the potential for change, and
3. As the [Cardano Constitution](https://constitution.gov.tools/en/interim-constitution) is a document intended for a global audience articulating how we intend and agree to treat each other, and
4. The Cardano Constitution thereby having the potential to increase the fitness of the global system at all scales in order to dissipate tension and increase everyone's ability to thrive in the given environment,

The current proposal suggests embedding the aforementioned principles in the Cardano Constitution as minimum viable values.

## Resources

Consider the following related articles and other resources:

<!-- * Discussions
    - [20 Epochs without a block averaging around 300,000 in stake](https://forum.cardano.org/t/20-epochs-without-a-block-averaging-around-300-000-in-stake/101527)
    - [Please help with checking my Stakepool configuration](https://forum.cardano.org/t/please-help-with-checking-my-stakepool-configuration/101824/64)
    - [340 ADA Pool Fee is becoming more of a concern](https://forum.cardano.org/t/340-ada-pool-fee-is-becoming-more-of-a-concern/107035)
    - [Why 340 Ada min fee is not being reduced](https://forum.cardano.org/t/why-340-ada-min-fee-is-not-being-reduced/107412)
    - [Announcing the stake pools chosen for October 2022](https://forum.cardano.org/t/announcing-the-stake-pools-chosen-for-october-2022/109142/38)
    - [No Blocks Generated in Last Two Epochs](https://forum.cardano.org/t/no-blocks-generated-in-last-two-epochs/110662)
    - [No Blocks Again... Everything Appears Normal. Bad Luck?](https://forum.cardano.org/t/no-blocks-again-everything-appears-normal-bad-luck-yyc-pool/114804)
* Related Links
    - [Idea for Proposing a Cardano Improvement Proposal](https://forum.cardano.org/t/idea-for-proposing-a-cardano-improvement-proposal/107720)
    - [Seeking Feedback on a CIP Idea](https://forum.cardano.org/t/seeking-feedback-on-a-cip-idea/107889) -->
* Articles
    - [The Future of DeFi, the Blockchain Ecosystem and More, Featuring Frederik Gregaard of the Cardano Foundation](https://medium.com/bittrexglobal/the-future-of-defi-the-blockchain-ecosystem-and-more-featuring-frederik-gregaard-of-the-cardano-ffd395b910e2)
    - [Waves Founder: DAOs Will Never Work Without Fixing Governance](https://cointelegraph.com/news/daos-will-never-work-without-fixing-governance)
    - [Why and How the PIVX DAO Works](https://pivx.org/news/why-and-how-the-pivx-dao-works)
    - [Why Less May Be More When Building Web3](https://cointelegraph.com/innovation-circle/why-less-may-be-more-when-building-web3)
    - [The Legal Dangers of Getting Involved with DAOs](https://cointelegraph.com/magazine/legal-dangers-getting-involved-daos/)
    - [Web 3.0 Hackathon on Astar Sponsored by Toyota Motor Corporation](https://dailyhodl.com/2023/02/01/web-3-0-hackathon-on-astar-sponsored-by-toyota-motor-corporation/)
    - [History of Money: From Fiat to Crypto, Explained](https://cointelegraph.com/explained/history-of-money-from-fiat-to-crypto-explained)
    - [Ethereum as a Deflationary Asset, Explained](https://cointelegraph.com/explained/ethereum-as-a-deflationary-asset-explained)
    - [DAOs are Not Corporations: Where Decentralization in Autonomous Organizations Matters](https://vitalik.eth.limo/general/2022/09/20/daos.html)
    - [ZKP Could Help Resolve Blockchain Tensions with GDPR](https://cointelegraph.com/innovation-circle/zkp-could-help-resolve-blockchain-tensions-with-gdpr)
    - [Joe Lubin: The Truth About ETH Founders Split and "Crypto Google"](https://cointelegraph.com/magazine/joe-lubin-the-truth-about-eth-founders-split-and-crypto-google)
    - [Entering Voltaire: Poll Experiment Live on Mainnet](https://cardanofoundation.org/en/news/entering-voltaire-poll-experiment-live-on-mainnet/)
    - [Are DAOs Overhyped and Unworkable? Lessons from the Front Lines](https://cointelegraph.com/magazine/dao-hyped-voting-decentralization/)
    - [Multiple Stakepool Operators are Harming Cardano](https://adapulse.io/multiple-stakepool-operators-are-harming-cardano/)
    - [Separation of Powers](https://en.wikipedia.org/wiki/Separation_of_powers)
    - [Swiss Foundation as a DAO Legal Wrapper: What You Need to Know](https://legalnodes.com/article/swiss-foundation-dao-legal-wrapper)
    - [UAE Launches Regulatory Framework for DAOs](https://www.globallegalinsights.com/news/uae-launches-regulatory-framework-for-daos/)
    - [Former Coinbase Exec Posits Blockchain-driven Vision of Future Societies](https://cointelegraph.com/news/coinbase-exec-blockchain-future-societies)
    - [8 Tips for Doing Macromanagement the Right Way](https://asana.com/resources/macromanagement)
    - [Technology is Not Values Neutral: Ending the Reign of Nihilistic Design](https://consilienceproject.org/technology-is-not-values-neutral-ending-the-reign-of-nihilistic-design-2/)
    - [Decentralizing in Spite of the Pareto Principle](https://bytemaster.medium.com/decentralizing-in-spite-of-pareto-principle-eda86bb8228b)
    <!-- - [Meditations On Moloch](https://slatestarcodex.com/2014/07/30/meditations-on-moloch/) -->
    <!-- - [50% of Cardano Nodes Hit with Disconnection Bug, Input Output Investigates](https://cryptoslate.com/50-of-cardano-nodes-hit-with-disconnection-bug-input-output-investigates/) -->
    <!-- - [Cardano Block Production Temporary Outage](https://input-output-hk.github.io/cardano-updates/2023-04-17-ledger/) -->
    <!-- [Democracy and the Epistemic Commons](https://consilienceproject.org/democracy-and-the-epistemic-commons/) -->
* Other Resources
    <!-- - [The True Meaning of Community](https://d3n8a8pro7vhmx.cloudfront.net/fce/pages/16/attachments/original/1419804654/True_Meaning_of_community.pdf) -->
    <!-- https://chattanoogaendeavors.org/service/community-building/stages/ -->
    <!-- - [Stages of Community Making](https://chattanoogaendeavors.org/wp-content/uploads/2019/04/The-Different-Drum-Chapter-5.pdf) by M. Scott Peck, MD -->
    <!-- - [Why You Need More Women at Your Workplace](https://www.linkedin.com/feed/update/urn:li:activity:7241302346318630912/) -->
    <!-- - [World](https://youtu.be/1JDY1KvoQYk?si=57Gfyhqm5efA9X25) -->
    - [Without Opposition, There is No Democracy](https://latinoamerica21.com/en/without-opposition-there-is-no-democracy/)
    - [Greenpilled: How Crypto Can Regenerate the World](https://www.worldcat.org/title/1303554957)
    - [Center for Humane Technology](https://www.humanetech.com/)
    - [Constitution of the Cardano Blockchain (by ChatGPT)](../constitution/AIConstitution.md)
    - [Relevant Research Papers and Specifications - Voltaire](https://docs.cardano.org/about-cardano/explore-more/relevant-research-papers#voltaire)
    <!-- - [Traffic Analysis as an Identifier of Toxic Workplace Environments or Negative Interpersonal Interactions in the Workplace: A Design Study](http://hdl.handle.net/20.500.11803/589) -->
    <!-- - [Method of Conducting Workplace Electronic Communication Traffic Analysis](https://patents.google.com/patent/US11423362B2/en?oq=11423362) -->
    <!-- - [Empowering Community-Driven Governance on Cardano](https://youtu.be/YvTfSx6pv9Y?si=6wacibbUWA-Vw_Cx) -->
    <!-- - [On Hydra Scaling](https://www.youtube.com/watch?v=vep6yMM-l3k) -->
    <!-- - [Playing the Infinite Game During the Meta-crisis with James Carse](https://www.youtube.com/watch?v=EFKa3zRFo7o) -->
    <!-- * Example Conflicts of Interest
    - Andrew Westberg, Senior Community Member—Operating Multiple [Blue Cheese Stake House](https://bluecheesestakehouse.com/) Pools
    - Robert Phair, [CIP Editor](https://cips.cardano.org/#editors)—Operating [COSD Pool](https://cosd.com/pool) -->

## Copyright

[DMCA Protected Item](https://www.dmca.com/r/69428j8)

## History

- <b>November 2022 to present</b>—Preparing an initial draft and seeking review
