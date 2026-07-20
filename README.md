# NRK Radio — Help &amp; Setup

This repository hosts the help and setup page for the **NRK Radio** Alexa skill at:

**https://theomnilord.github.io/NRKRadio-Help/**

The page covers what the skill does, how to talk to it, the channel list, how "latest news"
picks a bulletin, troubleshooting, and the privacy and content terms — in English.

The page is public only because GitHub Pages requires it. The skill itself is a **personal,
unpublished project** running on its developer's own Echo devices, is not available to install,
and is **not affiliated with or endorsed by NRK**. The skill's own repository is private.

## Why the anchors matter

Alexa's "About this Skill" panel exposes exactly two tappable links — **Privacy Policy** and
**Terms of Use** — and the labels cannot be renamed. Pointing them at `#privacy` and `#terms`
on this page makes the whole guide reachable in one tap from a phone, which is otherwise
impossible: a custom skill has no help or website URL field, and URLs written into the
description are not clickable.

So the skill manifest points at:

- `privacyPolicyUrl` → `https://theomnilord.github.io/NRKRadio-Help/#privacy`
- `termsOfUseUrl` → `https://theomnilord.github.io/NRKRadio-Help/#terms`

Both anchors must keep existing in `index.html` for those links to land correctly.
