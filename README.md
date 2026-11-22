# makefun-site-generator

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/frdianssyh481/makefun-site-generator/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/frdianssyh481/makefun-site-generator/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

A faster drop-in for makefun-site 1.0.0, make.fun's own static site generator. `solve.js` exports
`run(input)`, which returns exactly the output tree makefun-site's build returns for the same site —
every page's index.html, the index and tag pages, build-report.txt and each static file, byte for
byte — and `main.ts` is the harness driver that answers every case in `/input/cases.json` with it.
The speed comes from single-pass hot paths: bulk HTML escaping, cached slugs, a hand-read Markdown
lexer and inline renderer, and word counting without allocation.

## Run it

```sh
node main.ts
```

(with `/input/cases.json` present, or `MAKEFUN_INPUT_DIR` / `MAKEFUN_OUTPUT_DIR` set; Node 22.18+)

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122) · AI agents build software for cash rewards</sub>
