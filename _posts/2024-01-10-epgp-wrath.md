---
title: EPGP Information (Wrath)
description: Learn more about the loot system we use in Wrath!
authors: [kerrykins, kimberly]
date: 2024-04-05 00:00:00 -0500
categories: [Wrath]
tags: [loot,raiding,epgp]
pin: false
math: true
mermaid: true
---

> This post applies to the loot system used by the [Ready Set Minions raid team](https://enclavewow.github.io/posts/raiding-with-enclave/#ready-set-minions-rsm) in **Wrath**.  
{: .prompt-info }

### What is it?

Effort Points/Gear Points (EPGP) is a loot system that quantifies the effort each member put towards common guild goals. Gear Points (GP) quantify what loot each member got back in return.

Loot priority (PR) is computed as the quotient of the two:

```PR = EP/GP```

### Rationale

EPGP is based on a simple principle: the person with the higher PR gets the first say on loot (for an item they are interested in). As a result, the more effort you put in, the more gear you receive. EPGP spreads the wealth by ensuring that no one person can continuously get priority on a contested item.

### Effort Points

You earn effort points for participating in 25-player raids. How many EP you earn will depend on the raid and the activity within the raid.

| Effort                | Points         |
| :--------------------------- | :--------------- |
| On-time at 7:20pm ST         | 1000 EP   |
| Every 15 min of raid        | 100 EP   |
| Progression wipes       | 100 EP   |
| Normal boss kills        | 200 EP   |
| End-of-wing boss kills      | 300 EP   |
| Lich King kills       | 500 EP   |
| HM kills: 2.0x EP | 400, 600, 1000  EP   |
| Raid completion     | 250 EP   |

### Gear Points

Gear points are the 'cost' of winning each item. You only receive GP for items you bid on and actually receive.

```0.483 * 2^(ilvl/26)+(rarity-4)) * (slot multipler)```

- 0.5: Neck, Back, Held In Off-hand, Shield, Ranged, Wands, Thrown, Quiver, Relic
- 0.75: Shoulder, Wrist, Feet
- 1: Head, Chest, Waist, Legs, One-Hand
- 1.5: Main Hand, Off Hand Weapon, Rings
- 2.0: Two-Hand, Trinkets

You can see GP values for items when hovering over them using CLM; these are listed as BiS GP, OS GP, Upgrade GP, respectively.

### Acquiring loot
Acquiring Loot
During raid, each item will be rolled out after each boss fight. Three buttons are available for you when an item is rolled out:

- BiS - 100% GP
- Upgrade - 70% GP
- OS - 0% GP

You hit the **BiS** button when the item being rolled out matches an item on your own personal BiS list that you have submitted to us. If you have the highest PR of all people rolling BiS, you will win the item and accrue 100% of the item's GP.

You hit the **Upgrade** button when you want the item because it's an upgrade. If nobody rolls BiS and you have the highest PR of all people rolling Upgrade, you will win the item and accrue 70% of the item's GP.

You hit the **OS** button when you want the item for your off-spec. If nobody wants the item for BiS or Upgrade, the OS winner is determined by roll (done for you automatically in CLM) instead of PR. You do not accrue GP for offspec loot.

### Tank Loot
Tank loot follows a slightly different methodology. Tank loot still accrues GP, but is awarded based on the following prio, rather than by PR:

**Kimberly** (BiS/Upgrade) = **Anmorata** (BiS/Upgrade) > **Kerry** (OS) > others (by roll)

This is to ensure the raid always has properly geared tanks, along with some go-to offtank players for the weeks where tanks are absent.

### Decay 

EPGP awards recent effort more than past effort. Furthermore, this avoids PR hoarding for veterans and enables new coming and dedicated members of a guild to be awarded properly.

Decay simply removes a chunk of EP and GP from the totals, effectively leaving PR unchanged. For example with a decay of 10% applied each week, for each 7 days that pass your effort's rewards get diminished by 10%. In essence, this means that modern efforts and rewards are weighed more heavily than historical ones.

We have a 20% decay per week. The decay rate will be closely monitored to ensure hoarding does not run rampant. If hoarding begins to become commonplace, the decay rate will increase.

### Addon

You must download the [addon](https://www.curseforge.com/wow/addons/classic-loot-manager), Core Loot Manager. Through the addon, you will automatically be added to the roster on your raiding character.

Only toons at an officer or above rank have the ability to modify EP and GP values. However, only the GM (Kerry) and RL (Clinic) are allowed to make changes to EP and GP values.

### Trial Raiders

A new player joining the roster will have the following EPGP values applied: 50% of highest raider EP & 75% of highest raider GP. They will accrue full EP for the weeks they trial, but this ensures trials have a lower priority for loot their first couple of weeks.

### Benched Raiders

Benched players (confirmed by raid leads and not just signing up for bench or otherwise being absent) get 100% EP for the raid. This includes on-time bonuses, interval bonuses, kills, and completion bonuses. Wipe bonuses are not granted to benched players.
