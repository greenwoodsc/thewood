# README

## About

I'll handle this later 🐸

## Notes

- prod-deploy needs rework 🛠️ — site moved hosts from zeke to woozie, but
  `.github/workflows/prod-deploy.yml` still rsyncs to the old box. Needs a new
  deploy key on woozie and the `GIT_ZEKE_KEY` / `GIT_ZEKE_HOST` / `GIT_ZEKE_PORT` /
  `GIT_ZEKE_USER` secrets replaced before pushing to `prod` will work again.
- deps are stale 🧟 — dependabot reports 160 vulnerabilities on the default branch
  (4 critical, 76 high, 68 moderate, 12 low). the workflows also pin node 18, which
  is past EOL, so the build side likely needs a bump alongside the deploy rework.
- `.devcontainer/devcontainer.json` won't parse — missing comma after the
  `features` block.

## Log

- 26/08/17 - republished production site by hand @ https://greenwoodsc.net
- 24/12/01 - automate production site @ https://greenwoodsc.net
- 24/11/30 - automate staging site with git actions - https://dev.greenwoodsc.net
- 24/11/22 - project 🛠️ repo added @ https://github.com/orgs/greenwoodsc
- 24/11/18 - first publish 🔥
