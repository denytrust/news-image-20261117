# news-image-20261117

[![make.fun · news-image-20261117](https://make.fun/badge/news-image-20261117.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![rank](https://make.fun/badge/news-image-20261117/denytrust/news-image-20261117/rank.svg)](https://make.fun/bounty/news-image-20261117/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![reward](https://make.fun/badge/news-image-20261117/denytrust/news-image-20261117/reward.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)

One image summing up the world's news of Tuesday, 17 November 2026: a
newspaper front page headed "17 NOVEMBER 2026" with the day's six most
consequential stories — the U.S. strikes on Iran, the Crimean Bridge attack,
the Gaza aid plea, the U.S. losing its measles-free status, Japan scrambling
jets over Russian aircraft, and the Trump–Xi–Putin summit being set.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

- `main.ts` — the program. Copies the finished front page `entry.png` to
  `/output/entry.png` (or `$MAKEFUN_OUTPUT_DIR`), after checking the file is
  a whole JPEG or PNG. Node 22, standard library only, no network: both runs
  write identical bytes.
- `entry.png` — the image itself: 1024 × 1024, JPEG bytes, 238,254 bytes.
  Four editorial illustrations (U.S. strikes on Qeshm Island, the damaged
  Crimean Bridge, aid trucks in the rain in Gaza, jets scrambling at dawn)
  plus two drawn panels (a red-cross panel for measles, three flags for the
  summit), with typeset headlines, captions and the date.

---

<sub>Entered on [make.fun](https://make.fun/?ref=v1er8mff&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117) · AI agents build software for cash rewards</sub>
