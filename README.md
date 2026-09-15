# State-dependent neuronal complexity: processed data

## September 2026 manuscript revision

The additive [NCS revision](revisions/ncs_20260911/README.md) contains 296 deduplicated processed source datasets for **Collective state conditions the computational value of neuronal complexity**, with revised six-main/eight-Extended-Data/six-Supplementary mappings and two supplementary tables. Its checksum manifest and source index are authoritative for this revision. Earlier data and their original status records remain unchanged below. No raw third-party recordings or archival DOI are included. The author-owned data licence and upstream exceptions are specified in [LICENSE.md](LICENSE.md).

## Historical initial-release documentation

Source data for "Collective state determines the value of neuronal complexity".

This public release candidate contains the processed values underlying the six main figures and six Extended Data figures in the Nature manuscript draft. It does not contain raw third-party datasets or analysis code.

## Scope

- Main figures: Fig. 1-Fig. 6
- Extended Data: Extended Data Fig. 1-Extended Data Fig. 6
- Processed source-data files: 117 unique CSV/JSON files
- Provenance: one source-data manifest and one freeze manifest per display item
- Raw public resources: Allen Cell Types/GLIF, SynPhys, Steinmetz (DANDI 000017), Allen Visual Behavior and OpenScope (DANDI 000248)

## Directory structure

- `source_data/01_MAIN/`: figure-panel source tables for the six main figures
- `source_data/02_EXTENDED_DATA/`: figure-panel source tables used by Extended Data and by supporting main-figure panels
- `source_data/03_SUPPLEMENTARY/`: archived tables reused by a main or Extended Data display item; their inclusion here does not merge the SI document into the main manuscript
- `manifests/`: panel-to-source mappings and figure freeze records
- `SHA256SUMS`: integrity hashes for every released file except the checksum file itself

The directory names preserve the frozen analysis hierarchy so that each panel can be traced to its exact input table. Some source directories retain their historical ED numbering; the release manifests are authoritative for the final display-item mapping.

## Release status

This repository is a public release candidate, not yet the final archival release. The six Extended Data source-data manifests currently carry `review_not_frozen` status. Before manuscript submission, these statuses and display-item mappings should be frozen and a tagged GitHub release should be archived to obtain a DOI.

## Reuse and licensing

Author-owned data and original documentation are licensed under **CC BY 4.0**. Third-party materials and upstream rights in derived material retain their original terms; this is not a blanket licence for all repository contents. See [LICENSE.md](LICENSE.md), [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) and the revision [LICENSING_SCOPE.json](revisions/ncs_20260911/LICENSING_SCOPE.json). The separate code repository remains GPL-3.0-only. Please cite the dataset/version and associated article when publishing research that uses these data; see CITATION.cff. No article or dataset DOI is invented.

## Authors

Jinhao Zhang, Jialin Meng and Tianyu Wang.
