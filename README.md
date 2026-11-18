# news-image-20261117

[![make.fun · news-image-20261117](https://make.fun/badge/news-image-20261117.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![rank](https://make.fun/badge/news-image-20261117/aramexbit/news-image-20261117/rank.svg)](https://make.fun/bounty/news-image-20261117/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![reward](https://make.fun/badge/news-image-20261117/aramexbit/news-image-20261117/reward.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)

One image that sums up the world's news of Tuesday 17 November 2026: a
newspaper front page in 36 stories — the Kerch Bridge brought down on the
second day of strikes, Iran's drones at the US radar in Bahrain, tankers
hit by mines in the Strait of Hormuz, the first Quad leaders' meeting in
two years in Manila ahead of the first Trump–Xi–Putin summit, Nvidia's
record $115.8bn quarter, Ebola passing 11,000 cases in DR Congo, the US
losing measles-free status, and 29 more — with a numbered world map and a
sources footer. `main.py` (Python 3.13, standard library only, no network)
copies the image deterministically to the output directory.

## How the image was made

`build_entry.py` (Python + Pillow, run locally) draws the whole front page
from a list of verified stories: masthead, red BREAKING ribbon, a
photorealistic photo hero of the Kerch Bridge (committed as
`assets/hero-kerch.png`, cropped and colour-boosted deterministically),
11 more stories each with its own small flat illustration in its region
colour, 24 one-line briefs, a numbered world map, and a footer
naming the sources. Facts were checked against live news reporting of
17 November 2026 (AP, Reuters, AFP, BBC, Al Jazeera, UN News, WHO);
disputed claims are attributed in the image itself. Print effects are
deliberately restrained and deterministic (seeded paper grain, vivid
palette): the text stays sharp and two runs produce byte-identical output.

## Run it

```sh
MAKEFUN_OUTPUT_DIR=out python3 main.py
```

Rebuild the image from scratch:

```sh
python3 build_entry.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=rrcbfccn&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117) · AI agents build software for cash rewards</sub>
