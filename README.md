# DM Toolkit
A system-agnostic tabletop companion (not a VTT) that enhances in-person TTRPG sessions. The DM/GM runs a desktop app that acts as the table's server; players join from their phone browsers over the local network. An optional TV/projector "display" screen can show maps and images to the whole table. 

One of the core tenants of DM Toolkit is local only, no online subscription, no cloud hosting, no accounts, no telemetry. The only time an internet connection is required is updating the app or adding/updating a ruleset. Your campaigns, and worlds all live in a database on your machine. On that note the only thing the app does ask for is your players' name when joining the table for the first time. 

Please note this app was created with the help of AI.

## What it does

**At the table**
- Players' character sheets on their phones — live, editable, shaped by whatever game you play (rulesets are data, not code)
- An encounter tracker with initiative, turn alerts to the right phone, defenses, conditions, spotlight, and a fallen strip — with combatant sheets one click away. This is where both the player name and character name can be shown. Useful if you are running with a new group or doing a one shot at a store or convention.
- The DM Screen: a configurable widget canvas (rule cards, party at-a-glance, roll tables, clocks, scratchpad) on its own monitor for when you want to have a digital DM Screen
- Send images, maps, and messages to one player, some, everyone, or the TV
- Shopkeeper NPCs with real inventories — open the shop to the table, players browse on their phones and buy straight onto their sheets; prices stay askable, so haggling is still a thing
- Loot: give monsters weighted loot tables, then "roll the bodies" and grant the haul or if you want you can just provide whatever loot you want to the players

**Your world**
- A world codex that works like a wiki: lore pages, `[[name]]` links that mint pages, automatic backlinks, and search built for hundred-NPC worlds
- Locations on clickable maps — draw regions on your own map art (boxes, circles, pins, or traced borders); tapping or clicking one opens its page, and maps nest: world → region → city
- Races, organizations, events, and a declarable calendar with your world's own eras and months — rename or renumber an age and every date follows
- One world, many tables: bind campaigns to a world, fork what diverges per campaign, and adopt a fork into canon when you're ready

**Your rules**
- Starter ruleset profiles included, and an editor to build your own
- Import your favorite TTRPG from a licensed SRD or a book you own (personal use at your table; sharing is gated by the license) — reference cards, creatures, spells, and items come in through guided, teach-once importers
- An items catalog players can pull gear from, with stats landing in the right sheet columns

**Between sessions**
- Notes with full-text search, session summaries, player briefs and handouts
- Automatic on-quit backups with in-app restore — including a recovery window that works even when the database won't open
- Export a campaign, a world, or a character to a file that travels

## Status: Beta

DM Toolkit is in active beta and my table has been using it for a couple of months now. I am improving it fast (typically one release a week and sometimes more).
This beta exists to make it run yours. The **ruleset importer** wears a **Beta** badge in-app as of v0.12.0 — up from Alpha, after six rulebooks went through it end to end:
I feel that the importer is at a good place currently which is why its now in Beta. It reads real books and tells you what it couldn't read, but it's still being shaped by your
feedback.

If you find a bug, or wish something existed? [Open an issue](../../issues) 

The [project board](../../projects) shows what's I have planned and where your bug/feature lands.

## Backstory

This piece of software is something I have been playing around with for years. The first iteration of this was a website written in c# back in late 2015 for my first group. Since then it has gone though several iterations with different groups and campaigns. 
This latest version has been the brainchild of myself and my group I have been running for the past 5 years. 
Finally with the help of AI I have been able to get the software to a functional state and am now happy to share it with the public. 

So feel free to take the app for a spin and let me know if you find any bugs or want additional features added in. 

## Tech Stack

- **Node 24 LTS**, **pnpm** workspaces, **TypeScript** (strict) everywhere.
- **React + Vite** (player web app, DM renderer), **Electron** (DM desktop app).
- **Express + socket.io** (embedded server), **`node:sqlite` + Drizzle ORM**
