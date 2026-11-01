# Injection-molding AI review: supporting data and code

Version 1.2.0 supports the accompanying review *Intelligent Process Parameter Decision-Making in Polymer Injection Molding: From Initial Setting to In-Process Adaptation*.

## Evidence scope

This package contains the same 151 primary research publications, stable source IDs and author-confirmed D/V assignments as the corresponding evidence set in version 1.1.0. One record represents one publication's complete implemented system; D and V refer to the same application. Frequencies describe the selected evidence set of a structured critical narrative review, not field-wide prevalence.

The manuscript-local reference numbering and authentic search documentation align with the accompanying review. Searches and bounded incremental updates were completed by 1 November 2026. Historical execution dates and windows remain authentic. The bounded 28 October–1 November update added no newly included study.

## Contents

Extract `Injection_molding_evidence_dataset_v1.2.0.zip` while preserving folders. Within the extracted directory:

- `Supplementary/Supplementary_Table_S1.xlsx`: the 151-record evidence table, D/V definitions, eligibility and evidence bases, original-PDF locations/hashes, statistics and authentic search methods/queries.
- `Supplementary/Evidence_matrix.csv` and `Supplementary/Primary_DV.csv`: matching views of the same 151 publications, not independent samples.
- `Supplementary/Search_and_selection.csv` and `Supplementary/WoS_query_log.csv`: search-method and actual-query records matching S1.
- `Supplementary/heatmap_generation/`: the 151-record plotting input, DOI/reference map, Python script, validation results, instructions and MIT license.
- `Supplementary/Figures/`: reference Figure 4 in PDF/PNG/SVG and the count matrix.
- `requirements.txt`: the required Python package version.
- `CITATION.cff`, `.zenodo.json`, licenses and `MANIFEST_SHA256.json`: citation/archival metadata, license scope and file checksums. The checksum manifest excludes itself.

`Supplementary/Repository_information.txt` documents the earlier fixed archive and its relationship to manuscript companion files. It is retained verbatim from the accompanying formal supplementary materials; it does not identify a new version DOI for this package. Earlier published versions remain unchanged. Use the fixed-version DOI shown on the Zenodo record for version 1.2.0 when citing this package. Any version 1.1.0 DOI inside the byte-preserved companion documents is prior-version provenance and is not the identifier of version 1.2.0. The Zenodo record supplies the persistent identifier for this version.

## Reproduction

Use Python 3.12 and run `python -m pip install -r requirements.txt`. From the extracted dataset directory, run:

```text
python Supplementary/heatmap_generation/draw_heatmap.py
```

The script checks the input/workbook IDs, D/V assignments and DOI/reference mapping, computes matrix/totals and current SHA-256 values, and writes Figure4.svg, heatmap_counts.csv and validation.json. Its source paths are resolved relative to the script, so no local machine path is needed. Inkscape 1.4.4 on PATH is optional for PDF/PNG export; Arial is the intended plotting font. Fonts/exporters may change graphical or PDF bytes while preserving the underlying counts. Use a working copy if the archived output files should remain untouched.

Expected D0–D4 rows (columns V0–V3): `[0,3,1,0]`, `[15,32,3,0]`, `[21,11,16,1]`, `[0,5,23,1]`, `[0,1,18,0]`. D totals: 4, 50, 49, 29, 19. V totals: 36, 52, 61, 2. Total: 151. D4/V3: 0.

## Rights and public scope

Data, author-created tables/figures and documentation: CC BY 4.0; see `LICENSE_DATA.txt`. Python code: MIT; see `Supplementary/heatmap_generation/LICENSE`. Third-party publications, quoted source evidence and bibliographic material retain their own rights; the data license does not relicense source publications. Original-PDF filenames and hashes identify provenance without distributing the PDFs.

No literature full-text PDFs, private individual coding/review sheets, historical author disagreements, permissions, editorial correspondence, credentials or raw proprietary-database exports are included. The public methodological review description in S1 is retained. OpenAI Codex (GPT-6.1) assisted author-led script updating and consistency checks; the evidence assignments remain author-confirmed.

Creators, in confirmed order: Ningsheng Han; Yitao Ma; Zhongjie Li; Kaifang Dang; Weimin Yang; Pengcheng Xie.
