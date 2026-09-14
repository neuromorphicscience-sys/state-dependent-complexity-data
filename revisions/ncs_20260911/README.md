# NCS revision processed source data

This additive revision supports six main figures, eight Extended Data figures and six Supplementary figures in **Collective state conditions the computational value of neuronal complexity**. Earlier data releases are preserved unchanged.

`DATASET_INDEX.json` lists 290 content-deduplicated CSV/JSON source datasets. `tables/` contains the processed values, `panel_maps/` preserves the revised display-item grouping, and `supplementary_tables/` contains the two tabular supplements. The companion [code revision](https://github.com/neuromorphicscience-sys/state-dependent-complexity/tree/main/revisions/ncs_20260911) provides numerical replay commands.

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
Listed processed-table checks are not a certification of all raw estimators.

`panel_maps/primary_panel_crosswalk.json` and its CSV companion complete
Fig. 1-2: 18 quantitative lettered panels, 32 microplots and 27 directly used
datasets. The map distinguishes two discovery graphs in Fig. 1f from three
closure graphs and twelve inference graphs. Fig. 1j uses validation repeat 0,
with 24 graph-state observations per box from twelve graphs. Thirteen Fig. 2
interval tables satisfy ci95 = 1.96 SEM = 1.96 SD/sqrt(n); these are run-level
normal summaries, not graph bootstraps. All 1,895 saving observations reproduce
the topology summary statistics. One existing 252-row discovery task-method
table is added to make the reconstruction of all eighteen Fig. 1f means and
interval endpoints inspectable. The earlier 289 datasets are unchanged.

`panel_maps/task_support_crosswalk.json` and its CSV companion map all sixteen
ED8 panels. The complete primary and secondary six-task families are retained.
The 66 method/task summaries in ED8i-n use equal-weight raw scores across two
states, whereas the primary and secondary contrasts use worst-state normalized
scores, taking per-mask minima before control-mask averaging. All 22 SI Table 2
rows match frozen statistics, including the primary aggregate null. Shared
input-history controls are not twelve independent graph controls. The subsequent historical support crosswalks below complete the remaining ED1-5 mappings.

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


## Biological support crosswalks and reporting correction

`panel_maps/cellular_support_crosswalk.json` and its CSV bind ED6 and SI1:
20 lettered panels, 22 microplots, 17 datasets. Five display matrices and nine
stored-OOF subgroup correlations match; all 30-split distributions and 16 STP
interval rows retain their definitions. ED6d/e use stored original OOF values,
not the nested-rerun vector in b/c. PFC descriptors describe 6,357 canonical
neurons across 64 projection subtypes; they are not SynPhys target cells.

`panel_maps/population_support_crosswalk.json` and its CSV bind ED7 and SI2-6:
41 panels, 53 microplots, 46 datasets. One existing inventory JSON omitted by
the earlier table-read capture is added (SI2a). All prior 290 datasets are
unchanged; the revision now has 291. Engagement matrices use 38 valid sessions,
choice/outcome 39. ED7k/l have 72 records per representation, but finite raw /
residual counts are 71 / 67 for running and 69 / 65 for pupil. Original NaNs
leave point-only displays, not visible box summaries.

SI6b's inherited ylabel incorrectly named Jaccard. Its 12 values exactly match
leave-one-mouse-out mean top-unit AUC crossover, not Jaccard. The correction
changes only the ylabel and caption; no data, test, geometry or other figure
pixels change. Old and corrected PDF hashes are recorded. This metadata preserves
the original defect explicitly. Coefficient-landscape and Jaccard matched-null
boundaries remain non-confirmatory; they are not replaced by repeat averages.
All six main figures, ED6-8 and SI1-6 now have source-reviewed display/estimator
mappings. This is not raw-estimator or complete production-launcher portability.


## Complete quantitative-panel coverage

`panel_maps/full_quantitative_coverage.json` verifies disjoint coverage of all
202 quantitative lettered panels / 246 microplots across six main, eight ED and
six SI figures against frozen geometry. These are reporting counts, not new
independent experiments. Existing figure values and layouts are unchanged.

The transfer, stress and historical support crosswalk JSON/CSV pairs complete
ED1-5: 65 panels / 67 microplots. They distinguish graph, condition, state,
calibration and search-repeat units and each actual interval construction.
ED1b/d/e/f and ED4a use descriptive three-graph mean +/- 1.96 SEM bands, not
bootstrap intervals. ED2a/c transform clipped means and bounds separately.
ED3c-g use condition-level mean +/- 1.96 SEM, h saved condition-bootstrap limits,
and k/l twelve-graph percentile-bootstrap limits. Exact checks and remaining
raw-estimator limits are recorded in the corresponding JSON, including that
ED3h bootstrap endpoints and underlying ED4o masks were not regenerated.

Five already-existing generated SI10 source tables, used by final ED4j-o, were
omitted by the earlier upstream-read capture. They are now indexed byte-exact:
120 depth rows, six 10-to-20 gain pairs, 60 repeat crossovers, 120 search/held-out
pairs and 1,140 nested mask-overlap pairs (78,147 bytes total). All prior 291
dataset records and contents are unchanged; total indexed datasets is 296.
No new scientific runs, raw third-party records, licences or manuscripts are
part of this addition. Complete mapping does not certify raw-model rerunning.
