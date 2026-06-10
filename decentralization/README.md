---
CIP: CIP-y
Title: Creating a Parameter to Limit the Maximum Number of Delegators to Stake Pools and DReps
Category: Consensus
Status: Draft
Authors:
    - CoinCashew.io <doc@coincashew.io>
Created: 2026-06-10
License: CC-BY-4.0
---
<!-- Template based on: https://github.com/cardano-foundation/CIPs/blob/master/.github/CIP-TEMPLATE.md -->
<!-- Implementors: []
Discussions:
    - Original PR: https://github.com/cardano-foundation/CIPs/pull/? -->

## Abstract
<!-- A short (\~200 word) description of the proposed solution and the technical issue being addressed. -->

## Motivation: Why is this CIP necessary?
<!-- A clear explanation that introduces the reason for a proposal, its use cases and stakeholders. If the CIP changes an established design then it must outline design issues that motivate a rework. For complex proposals, authors must write a Cardano Problem Statement (CPS) as defined in CIP-9999 and link to it as the `Motivation`. -->

## Specification
<!-- The technical specification should describe the proposed improvement in sufficient technical detail. In particular, it should provide enough information that an implementation can be performed solely on the basis of the design in the CIP. This is necessary to facilitate multiple, interoperable implementations. This must include how the CIP should be versioned, if not covered under an optional Versioning main heading. If a proposal defines structure of on-chain data it must include a CDDL schema in its specification.-->

## Rationale: How does this CIP achieve its goals?
<!-- The rationale fleshes out the specification by describing what motivated the design and what led to particular design decisions. It should describe alternate designs considered and related work. The rationale should provide evidence of consensus within the community and discuss significant objections or concerns raised during the discussion.

It must also explain how the proposal affects the backward compatibility of existing solutions when applicable. If the proposal responds to a CPS, the 'Rationale' section should explain how it addresses the CPS, and answer any questions that the CPS poses for potential solutions.
-->

## Path to Active

### Acceptance Criteria
<!-- Describes what are the acceptance criteria whereby a proposal becomes 'Active' -->

<!-- For core categories (Ledger, Plutus, Network, Consensus) the following SHOULD be included:
- [ ] Implementation present within block producing nodes used by 80%+ of stake
-->

### Implementation Plan
<!-- A plan to meet those criteria or `N/A` if an implementation plan is not applicable. -->

<!--
OPTIONAL SECTIONS (see CIP-0001 > Document > Structure table for details):
These may appear here, between 'Path to Active' and 'Copyright', in any order
and at author/editor discretion. To use one, add it as an H2 below.

## Versioning            — if versioning is not addressed in Specification
## References            — external documents, prior art, related CIPs/CPSs
## Appendices            — supplementary material
## Acknowledgements      — contributors and discussion participants
## Open Questions        — unresolved design questions left for future discussion
-->

## Copyright
<!-- The CIP must be explicitly licensed under acceptable copyright terms. Uncomment the license you wish to use (delete the other one) and ensure it matches the License field in the header.
-->

This CIP is licensed under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/legalcode).

-----

Here’s another idea to address centralization in the network… maybe it’s useful directly or indirectly… maybe it’s a new idea, maybe it’s not… Reflecting Dunbar’s Number (https://en.wikipedia.org/wiki/Dunbar%27s_number) cap the total number delegators to a stake pool or DRep at about 150. Introduce MaxDelegators as a protocol parameter. Create a mechanism allowing stake pools and DReps to drop selected delegators. To implement the solution in the current network, keep the top 150 delegators by ADA for each stake pool and DRep, and then drop additional delegators.

Yes. The thinking was, if MaxDelegators is reached, then there is no possibility for a DRep (or SPO) to accept a new delegation without the ability to drop a delegator. Or maybe DReps or SPOs would prefer to operate having 148 delegators so there is always room for someone to come along and join. Or maybe DReps/SPOs prefer someone who wants to delegate to contact them and discuss first, in which case operating at MaxDelegators is fine. That mechanism would also force delegators to keep an eye in their delegation in case they get dropped, in order to find another DRep or stake pool to join and continue receiving rewards for example.

Do you know how to use https://github.com/input-output-hk/spo-incentives/blob/main/mainnet-indexer/README.md ? I wonder how difficult it would be to map decentralization in the current DRep and stake pool landscapes if different MaxDelegators limits are applied.

In the short term right after implementing, there may be an increase in the number of ADA holders not delegating as the MaxDelegators limit gets imposed, but in the medium to long term it may increase engagement between SPOs/DReps and delegators, as more active delegators may be more favoured or rewarded particularly over time as the ecosystem grows. There would also be a pull for new stake pools to come online, to give smaller ADA holders a selection of pools accepting delegations.

It might not fix everything but maybe it would be a step in the right direction. MaxDelegators could always be increased to 100,000 or something if removing the limit for all intents and purposes seems best in the future.

I would also look for a limit where most SPOs and DReps affected would lose an amount of delegation that would NOT be sufficient to incentivize starting another unsaturated pool or creating an additional, fake identity.

Maybe DReps would sometimes start to choose delegators who are friends or who are more supportive or easier to work with, rather than always focussing attention on delegators who have the most ADA

Maybe the way to implement something like MaxDelegators would be to start high, say 2000 for example, and then drop the limit gradually (over months or years) until there is a statistically significant increase in the number of viable stake pools (defined as having stake over 3M ADA, according to the recent Incentives report). If the total number of delegators in the ecosystem drops and does not recover in the short or medium term, then accept the theoretical loss in terms of network security and do nothing further to change MaxDelegators again until such time as it may make sense to do so.

Even having such a mechanism, without even using it, may eventually get rid of anyone in the ecosystem who is in it purely for a short-term profit motive without consideration for the health of the ecosystem over the longer term.

Polkadot has a mechanism where only the top 512 delegators to a pool receive rewards. However, Polkadot also has a 28-day waiting period with no rewards to leave a pool. Therefore, the incentive is to buy more DOT instead of joining a different pool. Buying more ADA or not spending rewards would be one way to mitigate the risk of not being dropped, but delegating to another pool or DRep would be designed to be easy, rather than difficult.

Even just the existence of MaxDelegators would help incentivize larger stake pools and DReps to support smaller pools and DReps to grow because if the number of viable stake pools and DReps grows regardless of the reason, then MaxDelegators can stay relatively high.

Rather than the current incentive where large stake pools and DReps are incentivized to let or even try to convince smaller pools and DReps to retire and leave Cardano because the total amount of available ADA is fixed and everyone wants a larger piece of the pie (rather than working to grow the size of the pie).

If MaxDelegators is implemented at an initial value that is significantly higher than the most delegators of any stake pool or DRep currently, meaning that no practical or measurable change in incentives would occur as a result of the implementation, then would implementing the parameter require a governance action or not?

The biggest hurdle to implementing something like MaxDelegators currently is that there seems no significant voting base in Cardano willing to put the long-term health of the ecosystem ahead of its own short-term personal profits, so proposing something like MaxDelegators for a vote would be a waste of time and energy.

Capping the number of delegators per stake pool and DRep is a variation on having a fixed total amount of ADA (45 billion).

Incentivizing group size based on the concept of Dunbar’s number helps create a context in which repeated interactions are more likely to occur between people, which in turn increases the likelihood of cooperation and trust developing.

