# Prediction Report: Preserve Archive 001 reaction simulation (see mirofish_prompt.md)

> **Read this first.** Every agent in this simulation is an LLM-generated hypothesis, not a real person and not evidence. The numbers below describe what the simulated people did. They are not measurements of real Indian buyers. Sample sizes are tiny (36 simulated people), so all rates are given as ranges. Marigold outcomes in the simulation (8 sprouted, 5 died among 13 buyers) are simulated events. They are not a germination rate, and the germination rate stays UNKNOWN.

## Executive Summary

In this simulation, a faceless, prepay-only, no-history drop converted about one in three of the 36 simulated people (13 of 36 preordered). Collectors converted best (8 of 16, about 50%), gift buyers less (4 of 11, about 36%), and skeptics almost never (1 of 9). The preorder gap closed slowly. The skeptic archetype opened with "Hard pass" in round 1, and the collector lead only committed in round 10, after the founder answered the reseller rumour with "I made every decision on Archive 001 myself". The gift buyer lead committed in round 11 with a back-up gift ready.

Repeat intent for Archive 002 was conditional and mostly unresolved. Counting only each agent's final repeat decision (36 of 36 agents logged one), 8 said yes, 8 said maybe leaning yes, 3 said a plain maybe, 5 said maybe leaning no, and 12 said no. The strongest driver was the marigold. Of the 6 buyers whose plant bloomed, 5 said yes and 1 leaned yes. Of the 5 buyers whose seed died, none said yes: 2 said no, 2 leaned no, and 1 (a collector who valued the tin over the plant) leaned yes. The most common stated blockers were an unnamed Archive 002 product and price, and no refund or replacement policy (8 each among the 28 agents who did not say yes). Next came the prepay trust gap (6), then dead seeds with no growing guide (4).

Confidence is low to moderate. The direction of effects (bloom helps, dead seed hurts, unanswered refund and product questions hurt) was consistent across agents. The magnitudes are not reliable. The simulated roster was built with a fixed group mix, the founder's replies were scripted to the seed's UNKNOWN items, and the marigold outcomes were simulated events.

## Simulation Parameters

- **Mode:** Forecast
- **Agents:** 4 key (founder plus 3 archetypes) + 3 crowd groups of 15, 10 and 8 agents (33 crowd; 37 total, of whom 36 are non-founder simulated audience members)
- **Rounds:** 40 scenario beats (about 54 simulated hours each, 2,160 simulated hours or about 90 days)
- **Seed documents:** preserve_seed.md
- **Rounds with no logged decisions:** 13, 14, 32 and 34 (rounds 13 and 14 are shipping-week, per the orchestrator)
- **Data note:** round files contain 313 action lines. `platform_state.json` reports 268 total actions. The difference was not reconciled. All tallies below come from the persona decision logs and were cross-checked against the round files (13 preorder decisions and 36 final repeat decisions match in both).

## Preorder and Repeat Rates (ranges)

**How to read these.** "Observed" is the count in the simulation, including the group's archetype lead. "Plausible band" is a 95% Wilson interval for sampling noise only. It does not cover LLM bias or scripted behaviour, so real uncertainty is wider. Non-buyers have no first purchase, so their "repeat" figure is really "would they buy Archive 002 at all". Repeat is shown strict (yes only) to lenient (yes plus maybe-leaning-yes).

| Group | Size (incl. lead) | Preorder, observed | Preorder, plausible band | Repeat, strict to lenient (all in group) | Repeat among buyers only |
|---|---|---|---|---|---|
| Collectors | 16 | 8 of 16 (47% without lead, 50% with) | about 30% to 70% | 31% (5) to 56% (9) | 50% (4 of 8) to 88% (7 of 8) |
| Gift buyers | 11 | 4 of 11 (30% without lead, 36% with) | about 15% to 65% | 18% (2) to 36% (4) | 25% (1 of 4) to 25% |
| Skeptics | 9 | 1 of 9 (12% without lead, 11% with) | about 2% to 45% | 11% (1) to 33% (3) | 1 of 1 (not interpretable) |
| All | 36 | 13 of 36 (36%) | about 22% to 52% | 22% (8) to 44% (16) | 46% (6 of 13) to 69% (9 of 13) |

Reading the table: the ordering (collectors above gift buyers above skeptics) was consistent, but the collector and gift buyer bands overlap heavily. The simulation cannot say that collectors truly out-convert gift buyers. Gift buyer repeat among buyers has only 4 people, one yes, one no, two leaning no.

### Final repeat decisions by group and marigold outcome

Final decisions only (`final:true`). "Lean" is the lean recorded on a maybe. Marigold labels are the label attached to each final decision. Of the 8 buyers whose seed sprouted, 6 are labelled bloomed and 2 sprouted at the end.

| Group | Marigold | N | yes | maybe, lean yes | maybe, no lean | maybe, lean no | no |
|---|---|---|---|---|---|---|---|
| Collectors | bloomed | 4 | 3 | 1 | 0 | 0 | 0 |
| Collectors | sprouted | 2 | 1 | 1 | 0 | 0 | 0 |
| Collectors | dead | 2 | 0 | 1 | 0 | 0 | 1 |
| Collectors | none (non-buyer) | 8 | 1 | 1 | 1 | 1 | 4 |
| Gift buyers | bloomed | 1 | 1 | 0 | 0 | 0 | 0 |
| Gift buyers | sprouted | 0 | 0 | 0 | 0 | 0 | 0 |
| Gift buyers | dead | 3 | 0 | 0 | 0 | 2 | 1 |
| Gift buyers | none (non-buyer) | 7 | 1 | 2 | 1 | 1 | 2 |
| Skeptics | bloomed | 1 | 1 | 0 | 0 | 0 | 0 |
| Skeptics | sprouted | 0 | 0 | 0 | 0 | 0 | 0 |
| Skeptics | dead | 0 | 0 | 0 | 0 | 0 | 0 |
| Skeptics | none (non-buyer) | 8 | 0 | 2 | 1 | 1 | 4 |

Across all groups:

| Marigold outcome | N | yes | maybe, lean yes | maybe, no lean | maybe, lean no | no |
|---|---|---|---|---|---|---|
| bloomed | 6 | 5 | 1 | 0 | 0 | 0 |
| sprouted (not yet bloomed) | 2 | 1 | 1 | 0 | 0 | 0 |
| dead | 5 | 0 | 1 | 0 | 2 | 2 |
| none (non-buyers) | 23 | 2 | 5 | 3 | 3 | 10 |

Caution: bloomed to yes (5 of 6) versus dead to yes (0 of 5) is the biggest contrast in the data, but the marigold outcomes were simulated events. Do not read it as the real effect size. Do not read the fact that 3 of the 4 gift buyer plants died as gift buyers being unlucky in reality. That split is an artifact of the simulated events.

## Key Findings

### 1. Overall Sentiment Trajectory

Final aggregate sentiment from `platform_state.json` was 34.1% positive, 25.7% negative and 40.2% neutral. Per-round average sentiment (computed from the action lines in each round) moved with the scenario beats rather than trending. It opened near neutral (round 1: -0.07, only 3 actions). It dipped in the first big trust argument (round 6: -0.14, 23 actions, founder says unfinished photos will not be posted), recovered through shipping and unboxing (round 15: +0.14, round 18: +0.17), then swung hard around the seed outcomes (round 19: +0.53, round 20: -0.22, round 21: -0.19). It rebounded at the first bloom reports (round 33: +0.58) and ended slightly below neutral (round 39: -0.02, round 40: -0.04) once Archive 002 was announced without a product or price. Per-round values with fewer than 8 actions are noisy and should be read as direction only.

### 2. Key Agent Behaviors

- **Preserve Founder** (`preserve_founder`, influence score 0.9656, 25 likes and 93 comments received). Held a firm, terse position: no face on purpose, no unfinished photos, "I will not invent" a germination figure. Deferred fabric, sizes, tin size, growing method and refund questions to a post that never fully arrived. His round 38 Archive 002 announcement drew 28 comments, the highest of any post, but gave neither product nor price. His refusal to invent facts kept him consistent, but the same consistency left the unanswered questions as the main stated blockers.
- **Drop-Culture Collector Lead** (`archetype_drop_culture_collector_lead`, influence 0.4365). Moved from "Who is behind this?" (round 2) to buying a number (round 10) to a bloomed plant (round 39). Final: maybe leaning yes, "I lean in, but I want the product and the price first". Withheld a tee review all the way through because fabric and sizes were never stated.
- **Gift Buyer Lead** (`archetype_gift_buyer_lead`, influence 0.6074, the highest of the three archetypes). Ordered in round 11 with a back-up gift, received the parcel two days early (round 18), then reported the gifted marigold did not come up (round 31, sentiment -0.42). Final: maybe leaning no, needing "a growing guide, a delivery date and a refund answer".
- **Skeptical Scroller** (`archetype_skeptical_scroller`, influence 0.2423). Ran the "Rs 1,09,900 sitting with someone with no face" maths (round 4), conceded "it exists" at the first unboxing, asked for blooms (round 24), got them, and still finished at maybe leaning no because the Archive 002 announcement was "the same blind prepay with a nicer first chapter".

### 3. Crowd Dynamics

Collectors produced the most conversation (59 comments and 10 posts, average sentiment +0.20), then gift buyers (34 comments, 3 posts, +0.09), then skeptics (33 comments, 1 post, -0.12). Collectors split internally. The supportive core (Kabir Malhotra, Aarav Mehta, Rohan Sethi) preordered in rounds 2 to 3. Cautious collectors waited for proof ("I will preorder when the first buyers show up with receipts", Arjun Nair, who never bought but ended at yes after seeing blooms). Critical collectors held out on trust (Nikhil Reddy, Aditi Singh) or identity (Aditi Singh in round 21: "A plant and a tin in a streetwear drop? That is a candle shop, not a drop.").

Gift buyers were the most exposed to delivery and refund worries (Tanya Bose in round 3: "I would be embarrassed if it vanished"). Their purchase reasons were about the plant, so a dead plant hit them directly ("A dead plant as a gift is a bad look", round 21). Skeptics were mostly stable. Four of eight ended at a plain no on prepay, history, a missing founder face, or refund policy. Three moved to maybe-lean-yes after seeing real units and blooms. One (Neha Chopra) bought and said yes.

### 4. Tipping Points

Shifts are measured against the previous round's average sentiment and rest on small action counts, so they mark direction rather than size.

1. **Round 19, first sprout (+0.36):** Kabir Malhotra's "Day five and the marigold is up". The first proof that the plant element could work.
2. **Round 20, first non-sprouting seed (-0.75):** Rohan Sethi: "Planted the seed on day two. Nothing so far. Is it only me?" Round 21 added a gift buyer's dead plant ("No care instructions anywhere") and the founder's reply in round 22 that he had no germination number.
3. **Round 31, gift lead's dead plant (-0.38 against round 30):** the most influential archetype reported a failed gift, and it set the "lovely tin, no use" framing.
4. **Round 33, first bloom (+1.02 against a two-action round 32):** Kabir Malhotra's "Orange, fully open, completely real". Bloom proof became the main persuasion lever for non-buyers (Arjun Nair and Simran Kaur cited bloom proof later).
5. **Round 35, dead-seed count and founder's reply (-0.24):** Rohan Sethi's "Dead-seed count on this page so far... Nobody in charge has said sorry or said what happens next" and the founder's "I will not invent one". The silence on remedy is what carried into the round 38 decisions.

## Top 5 Reasons a Buyer Does Not Come Back for Archive 002

Counts are over the 28 agents whose final repeat decision was not a plain yes (12 no, 16 maybe), with the buyer-only count where it differs. One agent can cite more than one reason.

1. **A dead or non-sprouting seed with no remedy, guide or germination answer.** All 5 buyers whose seed died ended at no (2), lean no (2) or lean yes only because the tin matters more (1). Four of the 7 non-yes buyers cite it. Quote: "Seed died, no refund or replacement policy stated" (Rohan Sethi, round 38).
2. **No refund or replacement policy.** 8 of 28 (Yash Bansal, Isha Reddy, Vikram Joshi, Tanya Bose, the Skeptical Scroller and others), including 3 of 7 non-yes buyers. It was asked about since round 2 and never answered.
3. **Archive 002 product and price unnamed.** 8 of 28, and 3 of 7 non-yes buyers (the collector lead, Dev Patel, Zoya Khan). These are soft blockers that lean yes, but every one of them is waiting.
4. **The prepay trust gap is still open.** 6 of 28: a faceless founder, no history, "one drop delivered is not a track record" (Vihaan Joshi). Mostly non-buyers. Delivery and blooms did not close it for them.
5. **Tee fabric, sizes, payment method and delivery date still unanswered.** 4 of 28 on fabric and sizes, 3 of 28 on delivery date. These were also cited by buyers who said yes, so they lower enthusiasm more than they cause refusal.

Runners-up: identity mismatch (a plant and a tin dilute streetwear credibility, or numbered scarcity means nothing as a gift: 2 of 28) and gift budget (Rs 1,099 "already a stretch for a gift": 1 of 28).

## The Single Change That Would Most Raise Archive 002 Repeat Purchase

**Publish a plain refund-or-replacement promise for seeds that do not come up, with the Archive 002 link, and say it in the announcement rather than by direct message.**

Why this one: seed outcome was the largest split in repeat intent (bloomed: 5 yes of 6, dead: 0 yes of 5), and no policy was the most repeated blocker among both buyers and non-buyers. "Message me" (round 35) did not count as a policy for the simulated people. It addresses the two groups that matter most: the dead-seed buyers (5 of 13 buyers, over a third, in this simulation) and the cautious non-buyers who keep asking about refunds (Yash Bansal, Isha Reddy, Vikram Joshi, the Skeptical Scroller). What it would not fix: the skeptics who object to a faceless founder (Harsh Pandey, Nikhil Reddy, Divya Menon) and the people waiting for a product and price. A growing guide is the runner-up change. It was asked for by the gift lead and Sneha Kulkarni, and could reduce dead seeds rather than just remedying them. The simulation cannot say which would work better. Both need a real test.

## Where the Simulated People Disagree with the Seed Assumptions

1. **The 60/40 collector versus gift buyer split is not tested here.** Of 13 simulated buyers, 8 were collectors (62%), 4 gift buyers (31%) and 1 skeptic-group member (8%). That looks like the seed's 60/40, but the roster was built that way (16 collectors and 11 gift buyers is 59/41), so the match is by construction and not a finding. The simulation also cannot test the founder's survey claim that gift buyers are the main group (survey details are UNKNOWN). The only part that is informative: per head, the simulated gift buyers converted less (4 of 11 versus 8 of 16, with overlapping bands) and were more fragile after a dead plant. If the survey is right and gift buyers dominate, the simulation suggests Archive 002 repeat would be held down by delivery date, refund and plant-failure concerns more than by scarcity.
2. **Collectors are not won by scarcity alone.** The seed assumes collectors are motivated by scarce, numbered drops. In the simulation they wanted legitimacy first. The lead had to see an answer to the reseller rumour before buying. Cautious collectors waited for the first buyers. Three of the 16 ended at no for trust or identity reasons (Nikhil Reddy, Aditi Singh and one more), and a fourth leaned no because one delivery is not a track record, not for lack of numbering.
3. **The plant is double-edged for both groups.** The seed treats the marigold mainly as the gift buyers' attraction. In the simulation, it was the main repeat driver for collectors too (3 of 4 bloomed collectors said yes), but a few collectors said the tin and the number matter more than the plant (Dev Patel, Zoya Khan), and one said the plant dilutes the streetwear idea (Aditi Singh).
4. **Skeptics are not a fixed non-buyer pool.** The seed treats skeptics as discovery drop-off. Here one bought and said yes, and three moved to maybe-lean-yes after seeing delivered units or blooms. Four did not move at all.
5. **Archive 002 interest is largely waiting on the unknowns.** The seed has Archive 002 product and price as UNKNOWN. The simulation kept them unknown, and 8 of 28 non-yes agents said they were waiting for exactly that. Repeat rates here are therefore conditional on whatever the product and price turn out to be.

## What Preserve Cannot Know from This Simulation (must test with real people)

All of these remain UNKNOWN in the seed and were not invented by the simulation.

- The real split between collectors and gift buyers, and what the founder survey actually asked and found.
- The real preorder conversion from the reel, and how many real people will prepay a brand with no history and no face.
- The marigold germination success rate and the right grow method (pot, soil, instructions). The 8 sprouted and 5 dead are simulated events, not a rate.
- How real buyers react to the T-shirt fabric, sizes, fit and colours, and the tin size.
- Payment method and refund policy. The simulation can only say that the lack of a policy was cited, not which policy works.
- Archive 002 product and price, and how repeat intent changes once they are named.
- Whether real delivery lands within 3 to 4 weeks, and whether late delivery damages gift occasions as simulated gift buyers feared.
- Whether real people respond to a founder who stays faceless, and whether blooms in other people's posts shift real behaviour the way they did here.
- How big real repeat rates are. Everything above is a small-sample, LLM-written hypothesis that should be checked, for example with a landing page waitlist with and without a refund line, a small paid pilot, and a bloom-or-not follow-up with the first real buyers.

## Prediction

### Most Likely Outcome

If real buyers behave directionally like the simulated ones, Archive 001 would sell a meaningful share of its 100 numbers to collectors who see trust signals (a real unboxing, a handled rumour), and a smaller share to gift buyers. Repeat for Archive 002 would be roughly split between a firm group (collectors with a bloomed plant) and a large undecided group waiting for the product, the price and a refund policy. Dead seeds would remove most of their owners from the repeat pool unless they were offered a remedy.

### Alternative Scenarios

1. **Remedy-first announcement.** If the Archive 002 link opens with a refund or replacement policy and a growing guide, the simulation's 16 maybe and no decisions based on refund, guide or germination would be the ones most likely to move. This scenario was not simulated.
2. **Gift-buyer majority.** If the founder's survey is right, preorder volume would depend more on delivery date, refund and price, and less on numbering. Repeat would depend heavily on plant success.
3. **Blind prepay again.** If Archive 002 opens with no product, price or refund line again, the simulation points to a core of repeat buyers (collectors with blooms) and a persistent no or maybe-lean-no group of skeptics and dead-seed owners.

### Risk Factors

- LLM agents tend toward articulate, consistent personas. Real buyers may be more impulsive and less consistent, so stated reasons here may not match real behaviour.
- The roster mix, the founder's replies and the marigold outcomes were fixed by the scenario, not discovered.
- 36 simulated people give very wide ranges.
- No competitor, price comparison, payment friction or Instagram algorithm effect was modelled.

## Methodology Note

This prediction was generated by a multi-agent simulation with 37 AI agents (4 key and 33 crowd) interacting over 40 simulated rounds (2,160 hours of simulated time). Each agent was assigned a persona based on entities extracted from preserve_seed.md and made autonomous decisions about posting, commenting, reacting and, for the purchase funnel, preordering and repeat intent. Results represent emergent behaviour patterns from agent interactions, not deterministic forecasts. All agents are LLM-generated hypotheses, not evidence. Repeat tallies use only decisions marked `final:true`. Round files read directly: 1 to 3, 10, 15, 18, 21, 35 and 38 to 40, with per-round sentiment and decision tallies computed by script over all 40 round files.
