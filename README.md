# Injection-molding AI review: supporting data and code

Version1.1.0 contains the151primary research publications used in *Intelligent Process Parameter Decision-Making in Polymer Injection Molding: From Initial Setting to In-Process Adaptation*. One record represents one publication’s complete proposed system; decision action D and validation evidence V refer to the same application. Frequencies describe this selected structured narrative-review evidence set, not field-wide prevalence.

## Content
Extract `Injection_molding_evidence_dataset_v1.1.0.zip`, preserving folders. `Supplementary/Supplementary_Table_S1.xlsx` supplies the151primary records, D/Vdefinitions, evidence bases and original-PDF locations, eligibility criteria, source hashes, statistics and authentic search methods/queries. `Evidence_matrix.csv` and `Primary_DV.csv` are matching views of the same151publications, not separate samples. Both method/query CSVs match the workbook. `Supplementary/heatmap_generation/` contains the151-row input, DOI/reference map, reproducible Python script, current computed validation and MITlicense. `Supplementary/Figures/` contains reference Figure4 and counts. `manifest_sha256.csv` excludes itself.

## Reproduction
Use Python3.12 and install `openpyxl==3.1.5` (or `python -m pip install -r requirements.txt`). Run `python Supplementary/heatmap_generation/draw_heatmap.py`. The script checks input/workbook alignment, computes the matrix/totals and fresh SHA256values, and writes Figure4.svg, heatmap_counts.csv and validation.json. Inkscape1.4.4 on PATH is optional for PDF/PNG export. Arial is the intended plotting font. Exporter/font differences may change appearance or PDFbytes while preserving data/counts.

Expected D0–D4 rows: `[0,3,1,0]`, `[15,32,3,0]`, `[21,11,16,1]`, `[0,5,23,1]`, `[0,1,18,0]`. Dtotals4,50,49,29,19; V0–V3 totals36,52,61,2; total151; D4/V3=0. The primary assignments and matrix are unchanged from the corresponding subset of version1.0.0. The literature cutoff is27October2026; all historical query execution dates/windows remain authentic.

## Scope and licensing
This release contains only the151primary D/Vrecords. Non-primary comparison/context records are excluded from this release and retained in the authors’ internal archive. No literature fulltexts, private author-review records, permissions, editorial correspondence or raw proprietary-database exports are distributed. Source-PDF hashes identify provenance without granting redistribution rights to source articles. The first author prepared the coding and another author reviewed it; no prospective blinded initial-coding agreement or kappa is claimed. Scientific assignments remain author-confirmed. OpenAI Codex using GPT-6.1 (OpenAI) assisted author-led plotting-script refinement and consistency checks.

Data/documentation: CC BY4.0, see LICENSE_DATA.txt. Python code: MIT, see Supplementary/heatmap_generation/LICENSE. Creators in confirmed order: Ningsheng Han; Yitao Ma; Zhongjie Li; Kaifang Dang; Weimin Yang; Pengcheng Xie.

## Version and citation
Version1.1.0 is the curated151-primary-publication release supporting the final review. Cite its fixed-versionDOI from the associated Zenodo release record. The earlier fixed version1.0.0 remains unchanged at https://doi.org/10.5281/zenodo.23641277 . No archived version is overwritten.
