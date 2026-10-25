# No Petals Plucked: In-Silico Bioprospecting for the Shirui Lily

Korounganba Rajkumar  
The Scindia School  
ORCID: [0009-0003-8686-3762](https://orcid.org/0009-0003-8686-3762)

This repository contains the manuscript and its accompanying data and code supplement.

- [Read the paper](paper/No_Petals_Plucked_Korounganba_Rajkumar.pdf).
- [Browse the supplement and its reproduction instructions](supplement/README.md).
- [Open the experiment notebook](supplement/code/Siroi_Lily_Geometric_Bioprospecting_A100_Final.ipynb).

The supplied paper's author name, affiliation and ORCID have been corrected using the author's details. The unconfirmed email address has been omitted. The scientific text, results, figures and references have been retained.

## Files

`paper/` contains the corrected manuscript. `supplement/` preserves all 477 substantive files from the supplied supplement, including the notebook, source snapshots, processed data, experiment logs, splits, result tables and figures. Mac Finder metadata files are excluded.

The supplement's internal directories and original checksum manifest are preserved. `REPOSITORY_SHA256_MANIFEST.csv` records the paths, sizes and SHA-256 checksums of every other file in this repository.

## Running the code

Follow the instructions in the [supplement README](supplement/README.md) and the notebook. The full experiment is configured for an NVIDIA A100 GPU in Google Colab. The recorded run environment is in [environment.json](supplement/study_artifacts/sirolily_geometric_bioprospecting/environment.json).

Packaging checks verified the supplied checksums and the absence of stored notebook error outputs. The experiments were not rerun while preparing this repository.

## Data provenance and reuse

ChEMBL and PubChem records retain their source terms and attribution requirements; see the [database and provenance notice](supplement/DATABASE_TERMS_AND_PROVENANCE_NOTICE.txt).

The screening candidates are literature-reported compounds from *Lilium lancifolium*. Their presence in *Lilium mackliniae* has not been established. Predictions are computational screening results, not experimental confirmation of occurrence or activity.
