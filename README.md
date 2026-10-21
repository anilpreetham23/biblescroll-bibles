# BibleScroll Bible language packs

Downloadable Bible text packs used by the BibleScroll Android app. Each pack is a gzipped SQLite
database (`<lang>.db.gz`) attached to the release [`packs-v1`](../../releases/tag/packs-v1).

All texts come from [eBible.org](https://ebible.org). They are either **public domain** or licensed
**CC BY-SA 4.0**. Packs under CC BY-SA 4.0 remain under that same license.

## Changes made

The original texts are eBible.org's VPL and USFM downloads. We changed only the following:

- Verse text was converted to SQLite. Runs of whitespace were collapsed; the wording is unchanged.
- Book names were taken from the USFM headers (`\toc2` or `\h`).
- Only the 66 books of the Protestant canon are included. Apocrypha and deuterocanonical books were dropped.
- Where the source merges verses, the merged text stays under the first verse number.

Build script: `tools/build_translation.py` in the app repository.

## Packs

| File | Language | Translation | eBible.org ID | Copyright / license |
|---|---|---|---|---|
| ta.db.gz | Tamil | Indian Revised Version (IRV) | [tam2017](https://ebible.org/find/details.php?id=tam2017) | © 2017, 2019 Bridge Connectivity Solutions · [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| kn.db.gz | Kannada | Indian Revised Version (IRV) | [kanirv](https://ebible.org/find/details.php?id=kanirv) | © 2017, 2019 Bridge Connectivity Solutions · CC BY-SA 4.0 |
| ml.db.gz | Malayalam | Indian Revised Version (IRV) | [malirv](https://ebible.org/find/details.php?id=malirv) | © 2017, 2019 Bridge Communication Systems (as stated on eBible.org) · CC BY-SA 4.0 |
| mr.db.gz | Marathi | Indian Revised Version (IRV) | [marirv](https://ebible.org/find/details.php?id=marirv) | © 2017, 2019 Bridge Connectivity Solutions · CC BY-SA 4.0 |
| bn.db.gz | Bengali | Indian Revised Version (IRV) | [benirv](https://ebible.org/find/details.php?id=benirv) | © 2018, 2019 Bridge Connectivity Solutions Pvt. Ltd. · CC BY-SA 4.0 |
| gu.db.gz | Gujarati | Indian Revised Version (IRV) | [guj2017](https://ebible.org/find/details.php?id=guj2017) | © 2019 Bridge Connectivity Solutions · CC BY-SA 4.0 |
| pa.db.gz | Punjabi | Indian Revised Version (IRV) | [panirv](https://ebible.org/find/details.php?id=panirv) | © 2017, 2019 Bridge Connectivity Solutions · CC BY-SA 4.0 |
| or.db.gz | Odia | Indian Revised Version (IRV) | [oryirv](https://ebible.org/find/details.php?id=oryirv) | © 2017, 2019, 2021 Bridge Connectivity Solutions · CC BY-SA 4.0 |
| as.db.gz | Assamese | Indian Revised Version (IRV) | [asmirv](https://ebible.org/find/details.php?id=asmirv) | © 2017, 2018 Bridge Connectivity Solutions · CC BY-SA 4.0 |
| ur.db.gz | Urdu (Devanagari script) | Indian Revised Version (IRV) | [urdirv](https://ebible.org/find/details.php?id=urdirv) | © 2019 Bridge Connectivity Solutions Pvt. Ltd. · CC BY-SA 4.0 |
| es.db.gz | Spanish | Reina-Valera 1909 | [spaRV1909](https://ebible.org/find/details.php?id=spaRV1909) | Public domain |
| fr.db.gz | French | Louis Segond 1910 | [fraLSG](https://ebible.org/find/details.php?id=fraLSG) | Public domain |
| pt.db.gz | Portuguese | Bíblia Portuguesa Mundial (World Portuguese Bible) | [porbrbsl](https://ebible.org/find/details.php?id=porbrbsl) | Public domain |
| de.db.gz | German | Lutherbibel 1912 | [deu1912](https://ebible.org/find/details.php?id=deu1912) | Public domain |
| ru.db.gz | Russian | Synodal Translation | [russyn](https://ebible.org/find/details.php?id=russyn) | Public domain |
| zh.db.gz | Chinese (Simplified) | Chinese Union Version | [cmn-cu89s](https://ebible.org/find/details.php?id=cmn-cu89s) | Public domain |
| ar.db.gz | Arabic | Van Dyke Bible | [arb-vd](https://ebible.org/find/details.php?id=arb-vd) | Public domain |

SHA-256 checksums for each file are in `SHA256SUMS.txt`, and the app checks every download against them.

The packs were built on 2026-10-21 from eBible.org files downloaded that day.
