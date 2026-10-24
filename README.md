# tardis-data

Daily snapshot of the interactive world history timeline: https://tardis.hi-curio.com

- `timeline.json`: `{ groups, items }`. Years are astronomical (1 BCE = 0). Labels and notes are
  keyed by language name (`english`, `chinese`, `spanish`, …).
- `.github/workflows/refresh.yml`: fetches daily at 03:17 UTC (or run it by hand). It commits and rebuilds tardis 
  only when the data changed.

Tardis builds its region pages (`/history/…`) from this file via `TIMELINE_URL`:
https://raw.githubusercontent.com/Eyasics/tardis-data/main/timeline.json

## License

Data: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) (see `LICENSE`).
Sources: [Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:Copyrights) (CC BY-SA 4.0),
[Wikidata](https://www.wikidata.org/wiki/Wikidata:Licensing) (CC0),
[World Bank](https://www.worldbank.org/en/about/legal/terms-of-use-for-datasets) (CC BY 4.0),
[Cliopatria/Seshat](https://github.com/Seshat-Global-History-Databank/cliopatria) (CC BY 4.0).
