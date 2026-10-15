# RoyaleTools plugin

Skills for using [RoyaleTools](https://www.royaletools.com), a Clash Royale companion website. An agent can find observed decks that fit a player's cards, improve a deck, build Clan Wars decks, read public player and clan data, plan upgrades, research the sampled meta and rankings, find guides and practice activities, and open the Merge Tactics builder.

RoyaleTools is a fan-made Clash Royale tools platform by Dcmat. This content is unofficial and not endorsed by Supercell.

This is a skills-only plugin. It contains instructions, not a service: no MCP server, backend, API key, or account connection. The agent works through the RoyaleTools website with the browser and web access it already has. In Grok Bot, that is the browser on the Bot's cloud computer.

## Skills

| Skill | Purpose |
|---|---|
| `royaletools-navigator` | Choose the right Clash Royale website tool |
| `clash-royale-decks` | Find observed decks that fit your cards |
| `clash-royale-players-and-clans` | Read public profiles, clan activity, and plans |
| `clash-royale-progression` | Plan upgrades with public and entered resources |
| `clash-royale-competitive-data` | Read sampled meta, card usage, and leaderboards |
| `clash-royale-community` | Explore clans, polls, tier lists, and brackets |
| `clash-royale-learn-and-practice` | Find published guides and suitable practice drills |
| `clash-royale-creators` | Find approved creator profiles and active codes |
| `clash-royale-merge-tactics` | Use the partner team builder and public stats |

## Example requests

- Find a Clash Royale deck that fits my card collection.
- Improve my eight-card deck while keeping my favorite cards.
- Help me plan my next upgrades and Clan Wars decks.

## Requirements and limits

- Public lookups need no RoyaleTools account. Collection-based answers need a public Player Tag. The plugin never asks for a Supercell login or game password.
- Many results load in the page with JavaScript, so they need a browser that can run the page and operate its controls. With only a page reader, the plugin gives the link and the steps to finish instead of claiming a result.
- Saved decks, Saved Tags, entered resource balances, and many personal bests stay in the browser where they were saved. RoyaleTools does not sync them between devices. In Grok Bot, the Bot's cloud browser is separate from your own browser and phone, so it cannot see decks you saved there, and anything the Bot saves stays in its browser.
- The Merge Tactics builder and stats come from a MergeTactics.gg embed. Opening it sends a normal browser request to MergeTactics.gg, which includes the public Player Tag for stats. If the agent cannot operate the embed, it gives you the page link.
- Some websites block traffic from cloud computers. If RoyaleTools shows a verification step, the agent hands it to you.

## What it will not do

- Cast community votes, showcase clans, register leaderboard scores, or complete human verification for you.
- Play timed minigames or puzzles for you, or submit AI-generated scores.
- Call RoyaleTools or partner APIs directly, or rewrite partner embed URLs.
- Act in the game, make purchases, or enter Creator Codes for you.
- Clear or overwrite saved decks, tags, or balances that you did not ask to change.

Deck observations show usage in sampled battles. They are not win rates or guarantees.

## Privacy and terms

The plugin itself does not collect or store data. Pages it opens are covered by the RoyaleTools [privacy policy](https://www.royaletools.com/privacy), [cookie policy](https://www.royaletools.com/cookies), and [terms](https://www.royaletools.com/terms), and your agent platform's own policies apply to the conversation.

## Support

Read the [FAQ](https://www.royaletools.com/faq) or email contact@rekonmedia.com.

## Testing

[TESTING.md](TESTING.md) lists the test cases and expected behavior.

## License

[MIT](LICENSE). The license covers this plugin's instructions and documentation. It does not grant rights to the RoyaleTools name or logo beyond identifying this plugin. Clash Royale and its card names belong to Supercell.
