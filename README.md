# Panu Automation

The public site for Panu Automation's apps: the privacy policies Google Play requires to be reachable at
a public URL, and nothing else.

Published with GitHub Pages from the `main` branch:

- <https://p-salo.github.io/panu-automation/> — index
- <https://p-salo.github.io/panu-automation/brainsnacks/privacy/> — **Brain Snacks privacy policy**,
  which is the URL in the Play Console listing

## What is deliberately not here

**No application source code.** This repository is public because a privacy policy has to be, and for no
other reason. Each app's source lives in its own private repository; nothing in here is generated from an
app build or links back into one.

Keeping it to flat HTML is the same decision: no build step, no dependencies, nothing to update, and
anyone can read the page source and see that it matches what the page says.

## Changing a policy

A privacy policy describes **the version of the app a person can install right now**, not a version that
is planned. So the order is: update the page, publish it, *then* release the build that makes it true -
and update the Play Console Data safety declaration in the same sitting, because the two have to agree.

Brain Snacks 1.0.0 collects nothing and has no network permission at all. The day advertising or
purchases are added, both the page and the Data safety form have to be rewritten before that build goes
out. Both this file and the page itself say so, on purpose.

## Contact

brainsnacks@panu-automation.com
