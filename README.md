# Panu Automation

The public site for Panu Automation's apps: the privacy policies and terms of use that the stores and the
apps themselves link to, and that have to be reachable at a public URL. Nothing else.

Published with GitHub Pages from the `main` branch, on the domain's own subdomain:

- <https://privacy.panu-automation.com/> — index
- <https://privacy.panu-automation.com/brainsnacks/> — **Brain Snacks privacy policy**, which is the URL
  in the Play Console listing
- <https://privacy.panu-automation.com/chainworks/> and `/chainworks/terms/` — **Chainworks privacy policy
  and terms of use**. Both URLs go into the game itself, and its shop stays shut until they answer. The
  advertising section is added on the day the game's ad SDK is merged, not before.
- <https://privacy.panu-automation.com/cra-workspace/> and `/cra-workspace/terms/` — **CRA Workspace for
  Jira privacy policy and terms of use**, in English, for the Atlassian Marketplace listing. The app's own
  repository is private, and a private repository's GitHub Pages would cost money, which is why its legal
  pages live here.

`privacy.` is a subdomain on purpose. The apex and `www` serve the company's own WordPress site from
DreamHost, and pointing either of those at GitHub Pages would take that site down. A subdomain is one
DNS record that cannot affect anything already there, and the domain's mail (MX, through MailChannels)
is untouched by it.

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

Brain Snacks 1.0.0 collects nothing. Its advertising SDK brought network permissions with it, which the
page says outright, and purchases add the billing permission. The page describing purchases and the
short ad between levels goes live on the day the first bundle with purchases is uploaded, and the Data
safety form is checked in the same sitting.

## Contact

brainsnacks@panu-automation.com
