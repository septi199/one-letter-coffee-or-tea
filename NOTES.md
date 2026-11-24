# Notes — One Letter: Coffee or Tea

## Bounty

- Competition: `u-rusdyxbt-one-letter-coffee-or-tea-89877fa0` — "One Letter: Coffee or Tea"
- Sponsor: u-rusdyxbt. Prize: $5 total (1st $2, 2nd $2, 3rd $1), escrowed on Solana.
- Entries close: 25 Nov 2026 05:45 WIB (24 Nov 2026 22:45 UTC).
- Account: lucky-falcon-48 (GitHub: septi199). Payout wallet (Solana):
  `78vHznCqia4UD4L4Xx2zAUMBFMVYw6W29izTwqu1mVwD`.
- Status at build time (25 Nov 2026 ~02:42 WIB): `can_submit: true`,
  5/5 daily submissions left, 0 entries made, hard limit 40 left.

## The gate

`/output/entry.txt` must be UTF-8 text of exactly 1 character, not only
whitespace. Anything else scores Valid 0, is never judged, and takes no prize.
So the program writes one byte and nothing else — no newline, no punctuation.

## The choice: A (coffee)

The judge is an AI tasting judge. It reads two letters at a time and picks the
one whose choice of coffee or tea feels more vivid, funnier, or truer, in that
order:

1. Exactly one letter, A or B — both choices satisfy this equally.
2. **Vividness (most important after validity):** coffee lands as the fuller,
   more alive answer. It is dark, bold, aromatic, bitter-sweet, the smell
   that fills a room and the drink that starts a day. Tea is gentle, calm,
   mild — pleasant, but quieter as an image.
3. **Funniness:** coffee carries more surprise and punch — the "don't talk to
   me before coffee" energy, the jolt. Tea's humour is softer.
4. **Trueness:** coffee is the honest answer for the person who sends it —
   the daily ritual most people actually reach for first.

Coffee wins on the first criterion that separates the two letters, so the
entry is `A`. There is no reasoning the program could add — the rules forbid
anything beside the letter — so the whole strategy is the choice itself.

## Determinism

`main.ts` picks the highest-vividness drink from a fixed table, writes exactly
that one letter, then re-reads the file and throws unless it is exactly 1 byte
equal to the letter. Run twice, the bytes are identical (sha256 recorded in
`SUBMISSION.md` at the build root).

## Files

- `main.ts` — entry program (writes `/output/entry.txt`).
- `README.md` — this entry, badges, and how to run it.
- `NOTES.md` — this file.
- `LICENSE` — MIT.
- `.makefun/owner.json` — payout wallet.
