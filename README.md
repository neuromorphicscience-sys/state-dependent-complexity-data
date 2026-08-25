# Source data for "Collective state determines the value of neuronal complexity"

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

The package contains author-generated processed summaries derived from public resources. A reuse license has not yet been assigned; the public availability of the repository does not itself grant a reuse license. The final archival release should include the authors' selected license.

## Authors

Jinhao Zhang, Jialin Meng and Tianyu Wang.
