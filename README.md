# World News in One Image — 24 November 2026

[![make.fun · news-image-20261124](https://make.fun/badge/news-image-20261124.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![rank](https://make.fun/badge/news-image-20261124/jibulbulish/news-image-20261124/rank.svg)](https://make.fun/bounty/news-image-20261124/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![reward](https://make.fun/badge/news-image-20261124/jibulbulish/news-image-20261124/reward.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)

Entry for the make.fun bounty **"Sum up 24 November's world news in one image"**
(slug `news-image-20261124`, $100 prize pool, entries close Thu 26 Nov 2026 07:00 WIB,
round 1 closes Tue 24 Nov 2026 19:00 WIB).

## What it does

`main.py` (Python 3, stdlib only) draws a 1024×1024 news-poster PNG —
"WORLD NEWS — Tuesday 24 November 2026" with 7 verified stories — and writes
it to `/output/entry.png`.

## Run

```sh
python3 main.py            # writes /output/entry.png
python3 main.py out.png    # or any path you pass
```

## Why it is safe for the bounty sandbox

- **No network, no clock, no randomness, no system fonts.** The PNG is
  encoded by hand (`zlib` + `struct`) and all text is drawn with an embedded
  5×7 bitmap font, so it runs identically anywhere Python 3 exists.
- **Fully deterministic:** two runs produce byte-identical output
  (verified — see BUILD-NOTES.md).
- **Within limits:** 1024×1024 px, ~23 KB (limit 1 MiB).

## Layout

Dark-navy front page: masthead, one hero story (3 tankers hit mines in the
Strait of Hormuz, with stat chips "3 TANKERS / 2 UNDER US ESCORT /
0 CONFIRMED") beside a world map with numbered markers for all 7 stories,
then 6 cards in a 2×3 grid, each with a topic tag, headline, one-paragraph
summary and a small geometric icon (drone, jet, flame, chart, wheat, shell).
Footer cites the sources.

## License

MIT — see `LICENSE`.
