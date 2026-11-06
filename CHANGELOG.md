# Changelog

## 0.1.4

Version bump only, with no skill changes. It lets the Claude plugin directory check the plugin again under its current rules.

## 0.1.3

The skills and route catalog now match RoyaleTools 0.1.3 for the OpenAI plugin directory, which gathers the website's plugin updates of October 24, 27 and 30, 2026. The adaptations listed under 0.1.2 are kept.

- Added Claude plugin manifests, `.claude-plugin/plugin.json` and `.claude-plugin/marketplace.json`, so the same skills install in Claude.
- README.md and TESTING.md now cover installing in Claude as well as Grok Bot.
- The progression skill covers Collection Level rewards. `/collection-level-rewards` lists every reward from Level 20 to 2,500. With a Player Tag, it shows which milestones the player's level has reached and the next reward, but it cannot tell whether a reward was collected in game.
- The community skill can help with a personal balance proposal in Balance Planner, `/community/balance-planner`, by changing the level 11 stats on a card's screen with the page's own controls. The plan saves in the browser used, and it is the visitor's opinion, not an official change.
- The community skill can point players to RoyaleTools Giveaways, a separate site, through `/giveaways?from=plugin`. The agent only shares the link. It does not solve the site's puzzles, claim rewards, or enter draws for the player, and it never promises a win. The navigator sends giveaway requests to the community skill.
- The learn-and-practice skill suggests Stat Showdown, a minigame at `/minigames/stat-showdown` that compares level 11 card stats, and the Spell Check puzzle at `/puzzles/spell-check` for spell interactions.
- The route catalog lists 68 destinations, up from 63. Collection Level Rewards, Balance Planner, Giveaways, Stat Showdown, and Spell Check are new, and the All Puzzles description now mentions spell damage.

## 0.1.2 (Grok Bot edition, unreleased)

First release from this repository. It has the same nine skills, website contract, and route catalog as RoyaleTools 0.1.2 for the OpenAI plugin directory, adapted for Grok Bot and other hosts that read the Cursor plugin format.

- The manifest is `.cursor-plugin/plugin.json`. OpenAI-only metadata, `extensions.com.openai` and each skill's `agents/openai.yaml`, is not included.
- Browser-state wording no longer assumes the user's own browser is Chrome. It explains that a cloud or agent browser cannot read the user's own saved decks, and that values saved in a persistent agent browser stay there.
- The website contract tells the agent to hand security checks and human verification to the user. On October 15, 2026, `/head-to-head` showed a Cloudflare "Verify you are human" page to an automated browser.
- The manifest description includes the unofficial fan-made disclaimer.
- The logo is the existing 512x512 RoyaleTools app icon, `public/pwa/icon-512-v2.png` on the website, the same artwork as the OpenAI package's 192x192 icon.
