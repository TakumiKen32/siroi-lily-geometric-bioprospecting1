# Computational experiment handoff

- Completed (UTC): 2026-07-17T18:08:13.680361+00:00
- Accelerator: NVIDIA A100-SXM4-80GB
- Profile: paper
- Scaffold split seed: 20260717

## Dataset summary

| task   | kind           |   n_molecules |   n_scaffolds |   median_heavy_atoms |   median_mol_wt |   label_mean |   label_std |   n_positive |   positive_fraction |
|:-------|:---------------|--------------:|--------------:|---------------------:|----------------:|-------------:|------------:|-------------:|--------------------:|
| ALOX15 | regression     |           387 |           143 |                   21 |         321.804 |     5.71787  |    0.869012 |          nan |          nan        |
| ARE    | classification |          5419 |          2879 |                   14 |         212.333 |     0.133235 |    0.33986  |          722 |            0.133235 |
| COX2   | regression     |          4325 |          1225 |                   27 |         390.892 |     6.20627  |    1.11979  |          nan |          nan        |

## Aggregate benchmark metrics

| task   | model                  | primary_metric   |     mean |       std |   n_seeds |   minimum |   maximum |
|:-------|:-----------------------|:-----------------|---------:|----------:|----------:|----------:|----------:|
| ALOX15 | ECFP4_RF               | RMSE             | 0.819618 | 0         |         1 |  0.819618 |  0.819618 |
| ALOX15 | ECFP4_XGB              | RMSE             | 0.974939 | 0         |         1 |  0.974939 |  0.974939 |
| ALOX15 | EGNN_3D_multiconformer | RMSE             | 0.936397 | 0.176184  |         5 |  0.819073 |  1.2479   |
| ALOX15 | EGNN_3D_multitask      | RMSE             | 0.904672 | 0.0132172 |         5 |  0.892188 |  0.920426 |
| ALOX15 | MPNN_2D                | RMSE             | 1.08041  | 0.142675  |         5 |  0.840848 |  1.1997   |
| ARE    | ECFP4_RF               | PR_AUC           | 0.283903 | 0         |         1 |  0.283903 |  0.283903 |
| ARE    | ECFP4_XGB              | PR_AUC           | 0.295215 | 0         |         1 |  0.295215 |  0.295215 |
| ARE    | EGNN_3D_multiconformer | PR_AUC           | 0.233488 | 0.0189527 |         5 |  0.203484 |  0.250486 |
| ARE    | EGNN_3D_multitask      | PR_AUC           | 0.173463 | 0.0576381 |         5 |  0.130865 |  0.242667 |
| ARE    | MPNN_2D                | PR_AUC           | 0.282703 | 0.0479909 |         5 |  0.226432 |  0.352087 |
| COX2   | ECFP4_RF               | RMSE             | 0.960198 | 0         |         1 |  0.960198 |  0.960198 |
| COX2   | ECFP4_XGB              | RMSE             | 1.02322  | 0         |         1 |  1.02322  |  1.02322  |
| COX2   | EGNN_3D_multiconformer | RMSE             | 1.06835  | 0.029183  |         5 |  1.01905  |  1.09697  |
| COX2   | EGNN_3D_multitask      | RMSE             | 1.1045   | 0.0202681 |         5 |  1.0855   |  1.13117  |
| COX2   | MPNN_2D                | RMSE             | 1.04619  | 0.0133288 |         5 |  1.03162  |  1.0632   |

## Validation gate

| check                                   | passed   | detail   |
|:----------------------------------------|:---------|:---------|
| Three endpoints present                 | True     |          |
| No scaffold leakage                     | True     |          |
| No exact-structure leakage              | True     |          |
| Finite labels                           | True     |          |
| All endpoint models evaluated           | True     |          |
| Class test contains both labels         | True     |          |
| Candidate provenance retained           | True     |          |
| Candidate applicability domain reported | True     |          |
| Bootstrap intervals generated           | True     |          |
| Figures generated                       | True     |          |
| Checkpoints generated                   | True     |          |

## Interpretation boundary

Predictions are computational prioritizations and require species-occurrence confirmation and experimental validation.