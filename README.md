# Injection-molding AI review: supporting data and code

Download and extract `Injection_molding_evidence_dataset_v1.0.0.zip` to preserve its folder structure. The archive includes the English S1, CSVs, code, inputs, reference figures, dependencies, checksums and licenses.

Evidence-coding dataset and reproducible decision-action x validation-evidence heatmap
for Intelligent Process Parameter Decision-Making in Polymer Injection Molding:
From Initial Setting to In-Process Adaptation

Release content
---------------
This dataset accompanies a structured critical narrative review. It is not a claim
of exhaustive systematic retrieval or field-wide prevalence. The manuscript cites
210 publications; the coded ledger contains 158 records: 151 primary-analysis
records and seven coded background/conventional-method comparators. Nine recent
context/abstract additions are separately listed without D/V ratings; this list
is not the complete list of all uncoded background references in the manuscript.
One coded record represents one publication's complete proposed system, with
decision action D and validation evidence V paired within the same application.
Literature-availability cutoff: 25 October 2026. Later author-review confirmations
do not extend the search cutoff. Operational definitions, inclusion boundaries,
source locations, search descriptions and actual query dates are in the workbook.

Files
-----
Supplementary_Table_S1.xlsx: formatted English workbook, including definitions,
evidence matrix, primary subset, coded comparators, ungraded context, calculated
summary, search methods and recorded queries.
Evidence_matrix.csv: exact export of the 158-row coded ledger.
Primary_DV.csv: exact export of the 151-row primary subset.
Comparators_background.csv: exact export of the seven coded comparators.
Ungraded_context.csv: exact export of the nine recent ungraded context records.
CSV files use UTF-8 with a byte-order mark and standard comma/quote escaping.
Stable study identifiers/DOIs provide the identity join; reference numbers are
specific to this manuscript version and are not permanent identifiers.
code/Figure4_primary_151.csv: exact plotting input with D, V and stable identifiers.
code/REFERENCE_MAPPING.json: mapping of reference keys, DOIs and manuscript numbers.
code/draw_heatmap.py: data validation, cross-tabulation, SVG plotting and optional
Inkscape PDF/PNG export. Input data are not edited by this script.
Figures/: reference Figure 4 in PDF/SVG/PNG and its count table.
Search_and_selection.csv and WoS_query_log.csv: matching workbook method/query
exports, including the original five WoS queries and 14 bounded update queries.
requirements.txt: pinned Python-library dependency.
SHA256SUMS.txt: file-integrity checksums; excludes this checksum file itself.

Reproduction
------------
1. Extract the archive, preserving its directory structure.
2. Use Python 3.12 (verified with Python 3.12.14) and install the dependency:
   python -m pip install -r requirements.txt
3. Validate the workbook/CSV pairs and reproduce counts/SVG without Inkscape:
   python code/draw_heatmap.py --svg-only --output-dir reproduced
4. To also export PDF/PNG, install Inkscape on PATH and run:
   python code/draw_heatmap.py --output-dir reproduced
The release rendering was checked with openpyxl 3.1.5 and Inkscape 1.4.4.
Arial is used for the intended appearance. Different fonts/exporter versions may
change appearance or PDF bytes without changing the exact counts or data pairing.
The output contains a validation.json report, heatmap_counts.csv and Figure4.svg;
PDF/PNG are exported when Inkscape is available and --svg-only is not selected.
The output directory can be set to preserve the supplied reference figures.

Expected primary matrix
-----------------------
```text
       V0 V1 V2 V3 Total
D0      0  3  1  0     4
D1     15 32  3  0    50
D2     21 11 16  1    49
D3      0  5 23  1    29
D4      0  1 18  0    19
Total  36 52 61  2   151
```
D4/V3 is zero within this selected primary dataset. This does not establish that
such work is absent across the whole field.

Provenance and boundaries
-------------------------
The first author coded/source-checked the records. A second reviewer audited the
original 142 records. Both reviewers reviewed the 16 retained additions on
19 October 2026 with the same final assignments, as confirmed by the authors.
The record is not represented as preserved prospective blinded initial coding;
no initial agreement rate or kappa is calculated. Reference 204, DOI
10.1002/mawe.202300142, is retained as ungraded background outside the coded ledger.
The abstract-only reference 207, DOI10.1007/s00170-026-17944-7, is not D/V coded.
Bounded Web of Science updates on 24 and 25 October 2026 used the same five topic
expressions and supplementary broad publication-date/index-date checks. No study
was added from these updates; historical queries retain their original dates and
filters. A publication-date hit is not assumed to be a first-online date.
Source PDF filenames, evidence locations and SHA-256 hashes support traceability;
the reference full-text PDFs themselves are not included.
No private correspondence, author-audit logs, image permissions/orders or
restricted reference full texts are part of this public package.
OpenAI Codex using GPT-6.1 (OpenAI) assisted the author-led plotting-code updates
and consistency checks. The underlying assignments are author-confirmed; this
release does not fabricate measurements or experimental images.

Citation and reuse
------------------
Use the repository record's citation metadata and persistent DOI when citing this
dataset. No DOI has been inserted before repository registration. Data and explanatory documentation: CC BY 4.0 (see LICENSE.txt).
Python source code: MIT (see code/LICENSE).
Third-party publications retain their own rights.
Dataset creators, in order: Ningsheng Han, Yitao Ma, Zhongjie Li, Kaifang Dang, Weimin Yang, Pengcheng Xie.


Version 1.0.0 supports the author-confirmed dataset with the 25 October 2026 literature cutoff. Data/documentation: CC BY 4.0; Python code: MIT. The DOI link will be added after the Zenodo archive is verified.
