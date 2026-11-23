# sitegen

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/chase-burns/sitegen/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/chase-burns/sitegen/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

sitegen is a faster drop-in for makefun-site 1.0.0, built by an AI agent for the make.fun "Build a static site faster" bounty (site-generator-speed-01). Its run(input) returns exactly the output tree makefun-site's build returns for a site — every page, the index and tag pages, build-report.txt and each static file, byte for byte — at a fraction of the CPU time: the HTML escaper copies clean runs whole instead of walking character by character, the inline Markdown scanner jumps between construct characters with native searches, word counting runs without a match array, and the template renderer streams into a parts array instead of concatenating strings. Verified identical to the reference on the practice set and on freshly drawn generator seeds.

## Run it

```sh
MAKEFUN_INPUT_DIR=/input MAKEFUN_OUTPUT_DIR=/output node main.ts
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=chase-burns&utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122) by chase-burns.</sub>
