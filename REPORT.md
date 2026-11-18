# news-image-20261117 — report

Entry for make.fun competition `news-image-20261117`, "Sum up 17 November's
world news in one image". Account: daring-puffin-40. Submitted as a GitHub
repo (parent agent to create `denytrust/news-image-20261117` and submit).

## The image

A newspaper front page, 1024 × 1024 px, JPEG bytes in `entry.png`
(238,254 bytes, sha256 `cc423027233ef80cd17b829b600fb8914faaed0af39b9386f33824de1c3b41af`).
Masthead names the day in large type — "17 NOVEMBER 2026", "TUESDAY · WORLD
NEWS IN ONE IMAGE" — then six stories, each with a picture and a short label:

1. **U.S. STRIKES IRAN** (hero) — warplanes hit missile sites on Qeshm
   Island after attacks on tankers in the Strait of Hormuz; Trump weighs
   reports of a "dirty bomb" plot, Iran denies it.
2. **BRIDGE HIT AGAIN** — Ukraine strikes the Crimean Bridge; Russia hits
   Kyiv's bridges.
3. **GAZA AID PLEA** — the UK, Australia, Canada and Italy urge Israel to
   open crossings as winter rain floods shelters.
4. **U.S. LOSES MEASLES-FREE STATUS** — first loss since 2000, after a year
   of uninterrupted spread.
5. **JETS SCRAMBLED** — Japan sends fighters up as Russian aircraft enter
   its airspace.
6. **TRUMP-XI-PUTIN SUMMIT SET** — first-ever trilateral meeting confirmed
   for Thursday in Shenzhen, on the sidelines of the APEC summit.

The four photographs are AI-generated editorial illustrations (no text in
them, so nothing can garble); all headlines, captions and the date are
typeset programmatically, so the text is crisp at any size. The two lower
panels are drawn graphics (red cross; U.S., Chinese and Russian flags).
Composition script: `../compose.py`; source illustrations kept in
`../assets-src/`.

## Sources (all reporting 17 November 2026)

- Reuters, via Profile News roundup, "November 17 2026 World News: U.S.
  Strikes Iran" — U.S. strikes on Qeshm Island; Oman evacuating 24 seafarers
  from the gas tanker Tara Gas; Crimean Bridge attack; U.S. measles
  elimination status lost (PAHO announcement).
  https://www.profilenews.com/en/november-17-2026-world-news/
- ASAS Press, "World News Digest: Top Stories of November 17, 2026" — joint
  Western call to open Gaza crossings; Depardieu; Japan scrambling jets
  after Russian airspace violation; Houthi advance in Yemen; Crimean Bridge.
  https://asaspress.com/en/news/world-news-digest-top-stories-of-november-17-2026
- LinkedIn Daily Buzz, "Daily Buzz: 17 November 2026" — China confirms the
  Xi–Trump–Putin trilateral meeting; Ukraine reports major Russian ballistic
  missile attack on Kyiv; U.S. chip export ban tightening.
  https://www.linkedin.com/pulse/daily-buzz-17-november-2026-china-biz-buzz-v0zcc
- ABC World News Tonight, Tuesday 17 November 2026 episode summary —
  U.S. airstrikes on Iranian missile sites; Trump–Xi–Putin summit; loss of
  U.S. measles elimination status.
  https://podcastrex.com/shows/world-news-tonight-with-david-muir/full-episode-tuesday-november-17-2026
- NewsTrendToday, "Morning Headlines Roundup (17 November 2026)" — Russian
  strike on Zaporizhzhia; COP31 draft deal; Xi–Trump–Putin summit set for
  Thursday in Shenzhen.
  http://newstrendtodaypk.blogspot.com/2026/11/morning-headlines-roundup-petrol-diesel.html

## Verification

- `main.ts` run twice with different `MAKEFUN_OUTPUT_DIR` values: both
  outputs byte-identical (sha256 `cc423027…3b41af`), 238,254 bytes.
- Image opens cleanly as JPEG, 1024 × 1024, under the 1 MiB cap.
- `main.ts` refuses a truncated file (JPEG SOI/EOI or PNG signature check)
  before writing.
- Grade-local: the kit's RULES.txt states there is no local grade for this
  competition ("the server grades every entry"); the CLI was checked and no
  local scorer is shipped, so verification above is the local check that
  applies. Dev grade happens on the server after submission.
- Node prints a harmless MODULE_TYPELESS_PACKAGE_JSON warning on stderr
  (no `package.json` in the repo, same as the kit starter); exit code 0 and
  the output file is written correctly.
