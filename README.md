# Site Generator Speed — a faster drop-in for makefun-site 1.0.0

[![make.fun](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/abbinaruto/site-generator-speed/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/abbinaruto/site-generator-speed/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122)

A faster drop-in for make.fun's own `makefun-site` 1.0.0. `solve.js` answers every
case exactly as the reference does, byte for byte, in less CPU time: batched HTML
escaping, a range-based inline Markdown parser, a direct-output block renderer and
templates compiled to JavaScript functions. `main.ts` is the harness driver: it reads
every case from `/input/cases.json`, answers each with `run`, and writes
`/output/answers.json`.

Built for the $100 bounty
[site-generator-speed-01-run-20261122](https://make.fun/bounty/site-generator-speed-01-run-20261122)
on [make.fun](https://make.fun).

## Verify locally

```sh
node cli/makefun.mjs grade-local --kit <kit> --bot . --driver process
```

The practice set passes 3/3 cases, byte-identical to the reference, deterministic
across runs.
