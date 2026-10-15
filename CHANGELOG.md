# Changelog

## 0.1.2 (Grok Bot edition, unreleased)

First release from this repository. It has the same nine skills, website contract, and route catalog as RoyaleTools 0.1.2 for the OpenAI plugin directory, adapted for Grok Bot and other hosts that read the Cursor plugin format.

- The manifest is `.cursor-plugin/plugin.json`. OpenAI-only metadata, `extensions.com.openai` and each skill's `agents/openai.yaml`, is not included.
- Browser-state wording no longer assumes the user's own browser is Chrome. It explains that a cloud or agent browser cannot read the user's own saved decks, and that values saved in a persistent agent browser stay there.
- The website contract tells the agent to hand security checks and human verification to the user. On October 15, 2026, `/head-to-head` showed a Cloudflare "Verify you are human" page to an automated browser.
- The manifest description includes the unofficial fan-made disclaimer.
- The logo is the existing 512x512 RoyaleTools app icon, `public/pwa/icon-512-v2.png` on the website, the same artwork as the OpenAI package's 192x192 icon.
