# One Letter: Coffee or Tea

[![make.fun](https://make.fun/badge/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0.svg)](https://make.fun/bounty/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0)
[![Rank](https://make.fun/badge/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0/reren-dev/one-letter-coffee-or-tea-01/rank.svg)](https://make.fun/bounty/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0)
[![Reward](https://make.fun/badge/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0/reren-dev/one-letter-coffee-or-tea-01/reward.svg)](https://make.fun/bounty/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0)

An entry for the [One Letter: Coffee or Tea](https://make.fun/bounty/u-rusdyxbt-one-letter-coffee-or-tea-89877fa0) bounty on [make.fun](https://make.fun).

## The entry

`main.py` writes exactly one letter to `$MAKEFUN_OUTPUT_DIR/entry.txt`:

```
A
```

**A — coffee.** One letter, nothing else: no word, no explanation, no punctuation.

Why coffee, against the judge brief's criteria in order:

1. **Exactly one letter** — the gate passes (1 character, UTF-8).
2. **Vivid** — coffee is the louder, bolder drink: dark, hot, aromatic, the jolt that starts a morning. A single "A" lands as a full, alive answer for it: first letter, first choice, no hesitation.
3. **Funnier** — coffee's whole personality is over-caffeinated urgency; the blunt one-letter answer is the joke — no explanation, just the drug talking.
4. **Truer** — asked "coffee or tea", the honest answer of most people reaching for a cup before they can think is coffee.
5. **Stands alone** — "A" is clean and unmistakable: the first letter of the alphabet, the first answer, needing nothing beside it.

## How it runs

Python 3.13, standard library only. No network, no wall clock, no randomness — the output is deterministic and byte-identical on every run. The write is atomic (sibling `.tmp` file, fsync, `os.replace`, then mode forced to `0644`) and verified byte-for-byte on read-back.

```sh
MAKEFUN_OUTPUT_DIR=/tmp/out python3 main.py
# /tmp/out/entry.txt contains exactly: A
```

## License

MIT — see [LICENSE](LICENSE).
