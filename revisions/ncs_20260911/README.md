# NCS revision processed source data

This additive revision supports six main figures, eight Extended Data figures and six Supplementary figures in **Collective state conditions the computational value of neuronal complexity**. Earlier data releases are preserved unchanged.

`DATASET_INDEX.json` lists 289 content-deduplicated CSV/JSON source datasets. `tables/` contains the processed values, `panel_maps/` preserves the revised display-item grouping, and `supplementary_tables/` contains the two tabular supplements. The companion [code revision](https://github.com/neuromorphicscience-sys/state-dependent-complexity/tree/main/revisions/ncs_20260911) provides numerical replay commands.

## Traceability

`panel_maps/biological_panel_crosswalk.json` and its CSV companion bind all
19 quantitative lettered panels (28 microplots) in Fig. 5-6 to 34 exact dataset
IDs, display transformations, observation units and interval rules. Plotting
helpers and assembler functions were reviewed, rather than inferring use from
file-read order alone. This uncovered one omitted existing summary, now added
as `sd_306538b8385c4e1aa127`: Fig. 5c reads its observed rho and permutation P
from this JSON, in addition to its null-draw CSV. The earlier 288 datasets are
unchanged; this is a source-coverage correction, not an added experiment.
Fig. 6g has 12 plotted mouse rows, each already averaging 24 unit splits.
Fig. 5j shows point estimates without error bars; Fig. 5i(right) and 5k show
coefficient intervals. This record does not certify every statistical model or raw fit.

`panel_maps/computational_panel_crosswalk.json` and its CSV companion add
23 quantitative lettered panels (28 microplots) in Fig. 3-4, bound to 23 exact
datasets. The mapping distinguishes the two-graph/36-condition discovery,
the five historical strata whose pooled summary contains 225 task conditions,
and the 12-graph task/shared-policy evidence. It verifies the task panels'
per-mask minimum-before-control-mean order, graph-mean historical heatmap,
four-candidate/six-pair nesting, and equal-weight stress summaries. Historical
boxplots contain nine graph-state observations per budget, not nine independent
networks or bootstrap intervals. Existing source tables remain unchanged.
Fig. 1-2 and the ED/SI figures still require the same detailed mapping; listed
processed-table checks are not a certification of all raw estimators.

Each dataset has a stable content identifier, SHA256, source-table aliases and a relative filename. Dataset aliases are scientific table names, not private workstation paths. Three records had local path metadata removed; these changes are explicitly recorded and do not alter numerical values. All other dataset bytes are unchanged. Different source filenames with identical content are stored once. `SHA256SUMS.json` binds every file in this revision except itself.

The assembly-level source collections are not a claim that every listed dataset is used in every panel. The panel map gives the exact historical panel/group identity, while the dataset index resolves source-table aliases. More detailed source-to-estimator coverage is provided with the code. Independent sample counts follow the relevant dataset and legend; the number of tables or microplots is not an experimental sample size.

`resource_provenance/openscope_000248.json` records the original DANDI 000248 version 0.240502.2344, upstream DOI and the twelve analysis-source session assets. The 78-file inventory matches published asset identities, paths and sizes; all twelve session NWBs identified by archived cache source paths were freshly SHA-256 verified against the official version. This manifest contains identifiers and hashes, not raw recordings. Historical cache extraction was not repeated, and old caches did not record raw hashes at creation. The upstream resource DOI/license is not a DOI/license assigned to this processed-data revision.

## Scientific scope

Two additional metadata-only source manifests bind the population analyses:
`resource_provenance/steinmetz_000017.json` identifies DANDI version
0.240329.1926, 39 sessions from 10 mice and the matching published SHA-256s.
`resource_provenance/allen_vbo_1_1_0.json` identifies official Allen manifest
1.1.0, its versioned S3 objects and BLAKE2b hashes: 72 input experiments from
24 containers/24 mice, three experiments per container. All referenced raw
files were freshly content-hashed; archived input identities and metadata also
match. Endpoint-specific filtering can reduce these counts. Original fits and
cache extraction were not rerun; historical fit outputs lack contemporaneous
raw hashes. Only identifiers and verification metadata are included here.

Cellular source bindings are in `resource_provenance/glif_metadata.json`,
`glif_model_runs_400.csv` and `synphys_r2_1.json`. GLIF archived model-run metadata
(created 18 August 2026; hash recorded) match the historical 1,218-cell atlas.
All 2,000 model-run IDs and explained-variance values for the 400-cell primary
mouse cohort also match the current Allen API and the released cost table.
This mutable API is not represented as an immutable versioned release.
The SynPhys Phase-1 record identifies `synphys_r2.1_full.sqlite`: direct read-only
queries reproduce all 57 selected cell fields (24,739 rows) and 34 pair fields
(123,506 rows) in the archived input tables. Numerical differences are zero;
literal empty-string/CSV-null conversions are explicitly recorded. Official
release manifest, schema metadata and object length agree. The database was
**not** fully content-hashed, and its multipart ETag is not a raw-file MD5.
These checks do not rerun raw feature extraction, model fitting or later
transfer/statistical analyses. Only identifiers and verification metadata are
added; no raw database or electrophysiological recordings are redistributed.

The release retains the complete six-task comparison families, not only delayed recall and interval discrimination. Shared-policy results use the reference-corrected frozen evaluation. Task primary-null results, unresolved shared sufficiency and biological landscape-null controls remain explicit. Biological tables are processed summaries from public resources; no raw third-party recordings are redistributed.

The underlying resources include Allen Cell Types/GLIF, SynPhys, Steinmetz, Allen Visual Behavior and OpenScope. Access raw data through the original providers under their terms. The data repository currently has no assigned reuse license; public availability alone does not grant a reuse license. No new license or archival DOI is asserted by this revision.
