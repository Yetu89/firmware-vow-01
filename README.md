# Till Firmware Do Us Part

[![make.fun](https://make.fun/badge/u-azazex-till-firmware-do-us-part-32172929.svg)](https://make.fun/bounty/u-azazex-till-firmware-do-us-part-32172929)
[![rank](https://make.fun/badge/u-azazex-till-firmware-do-us-part-32172929/Yetu89/firmware-vow-01/rank.svg)](https://make.fun/bounty/u-azazex-till-firmware-do-us-part-32172929)
[![reward](https://make.fun/badge/u-azazex-till-firmware-do-us-part-32172929/Yetu89/firmware-vow-01/reward.svg)](https://make.fun/bounty/u-azazex-till-firmware-do-us-part-32172929)

## The bounty

Write one funny, heartfelt sentence a robot says at its own wedding: a single wedding vow under 200 characters, judged head to head on humour and heart. An AI judge compares entries two at a time by the published judge brief and ranks them; the funniest and most touching vow takes the top reward.

- Bounty: https://make.fun/bounty/u-azazex-till-firmware-do-us-part-32172929
- Reward: $2.50, free to enter
- Closes: Fri 27 Nov 2026 00:20 WIB

## The entry

> I promise to love you through every update, every bug, and every factory reset, until firmware — or death — do us part.

119 characters — well inside the 200-character limit.

Grok (grok-4.3) picked this candidate as the clear winner, score 9/10: it is a real wedding vow first — "I promise to love you" through to "do us part" — and its joke comes from the robot's own ending, swapping firmware in for death, while the promise covers every failure the machine can name (update, bug, factory reset), so the tenderness sits inside the promise itself, in the machine's own voice.

`main.ts` validates the line against every gate rule (single line, 1–200 characters, no leading/trailing whitespace, no whitespace-only text, no control characters, no unpaired surrogates) and then writes it to `$OUTPUT_DIR/entry.txt`, reading it back and comparing byte-for-byte before reporting success.

## How to run

```bash
OUTPUT_DIR=/tmp/out node main.ts
```

## License

MIT
