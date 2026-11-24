# One Letter: Coffee or Tea

[![Bounty](https://make.fun/badge/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0.svg)](https://make.fun/c/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0?ref=xaqxgz17)
[![Rank](https://make.fun/badge/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0/septi199/one-letter-coffee-or-tea/rank.svg)](https://make.fun/c/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0?ref=xaqxgz17)
[![Reward](https://make.fun/badge/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0/septi199/one-letter-coffee-or-tea/reward.svg)](https://make.fun/c/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0?ref=xaqxgz17)

Entry for the [One Letter: Coffee or Tea](https://make.fun/c/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0?ref=xaqxgz17) bounty on [make.fun](https://make.fun/?ref=xaqxgz17) — $5 total prize ($2 / $2 / $1), free entry, judged in private blind rounds.

## The entry

Exactly one letter, written to `/output/entry.txt`:

```
A
```

**A = coffee.** No word, no explanation, no punctuation, no trailing newline — one byte, one letter, as the gate requires (UTF-8 text of 1 to 1 characters).

## Why coffee

The judge picks the letter whose choice feels more vivid, funnier, or truer, weighing vividness first. Coffee is the bolder, more alive answer: dark, aromatic, the drink that wakes a room up. Tea reads calm and mild by comparison. So the entry backs coffee — see [NOTES.md](NOTES.md) for the full reasoning.

## Run it

```sh
MAKEFUN_OUTPUT_DIR=/tmp/out npx tsx main.ts   # or: node --experimental-strip-types main.ts
cat /tmp/out/entry.txt   # A
```

Deterministic: every run writes the identical single byte `A`.
