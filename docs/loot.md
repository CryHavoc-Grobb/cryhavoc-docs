---
title: Loot
---

# Loot System

The current system is Loot Council with [TMB](https://thatsmybis.com). 

We are currently toying with the idea of a new loot system based on Softres. With it, the goal is:

- Reduce management overhead. Loot council requires constant grooming.
- Reduce subjectivity. Some players get salty and start developing good-ole-boy conspiracies which tends to turn toxic.
- Incentivize performance to ensure gear is going to those that will bring the most value first.
- Still work with PUGs should we need to fill spots
- Not allow gear sniping - those scenarios where you've SR'd a piece for 6 weeks in a row, uncontested, then suddenly someone that got their last SR decides to SR against you, the item finally drops and *they* win it. There should be a way to reduce the chance that this can happen.

## Tentative SR system

Standard 2 SR system as a base and then we add incentives on top of it. Items that are not SR'd fall back to MS>OS + 1.

### Incentives

- Top 3 performers from previous week may trade 1 SR for 1 HR for the current week
- Top 5 (including top 3) receive a roll buff equal to `4(8 - rank)`. For example if you were rank 5 in the previous week then `4(8 - 5) = 12` you would get a roll buff of +12. So when you use the roll buff, if you were to roll a `50` then we would count it as a `62`.

If you miss the prior week, then you will have no placement and therefore do not qualify for incentives. You will get your normal 2 SR.

!!! note
    This might only make sense for the 25m raid at first glance, however it might have some value across 10 mans to ensure those groups are staying competitive as well. For example, if you rank across all groups, then players can still get incentives. The down side is that a lower performing *group* might cause some players to underperform -- this is debateable. You can still argue that the placements would still be generally correct.

    The thought process here is that:

    - By incentivizing, we don't have to penalize
    - It might be easier to just have MS>OS+1 in 10m groups but leaving it all up to luck can still lead to some imbalances. Also, by ranking across all groups, we ensure everyone is still incentivized and it still adds some competition between groups
    - The system doesn't change for PUGS, however they do need to be made aware that they might lose a roll to a roll buff. We might have to devise a way for the pug to optionally get a roll buff, but it might open a new can of worms.
    - This is just for prioritizing loot, those that don't receive incentives will still get their items.
    - We might be able to extend the roll buff across the raid based on rankings, but figuring out the forumla would be tricky and it would be a LOT to manage.
    

## Performance Rankings

So how is "performance" gauged?

### DPS

DPS ranking is pretty straight forward: more DPS = higher rank. However, to ensure we're recognizing *performance* not just flexing, we will use parse ranking *by bracket*. The objective here is to not punish players for their gear and not over-reward players for being overgeared. The hope is also that, by bumping people up the ranks based on this metric, it should give them more opportunities to receive better gear more quickly, bringing them up to snuff faster so we can all benefit from their increased performance. In other words, we want gear to first go to players that will get the most out of it.

### Healers

// TBD

### Tanks

// TBD

!!! info

    Still need to work out a few issues with tank and healer placements since they can be really subjective.

    **Tanks**

    - Ranking based on DTPS, or TPS is problematic because the MT will always be higher
    - Ranking based on CD usage and fight control is subjective and cannot be quantified

    **Healers**

    - Ranking based on HPS is subjective especially with stuff like priest bubbles and as fights get easier, less healing is needed so some healers start to do more DPS
    - Overhealing could be a viable metric since it really measures effective healing vs. wasted healing, but it would need to be paired somehow with overall healing.
    - The best metric would really to be to measure overall healing along with landing heals when they're needed the most, but there's no easy way to track that without writing our own addon.