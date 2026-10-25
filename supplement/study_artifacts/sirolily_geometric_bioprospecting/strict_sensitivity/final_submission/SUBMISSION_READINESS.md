# Siroi Lily Digital Bioprospecting: Submission Status

## Overall status

The computational experiments are complete and suitable for manuscript
preparation.

## Primary ALOX15 result

Five-fold scaffold-disjoint cross-validation included
202 molecules and
82 scaffolds.

The strongest model was ECFP4_XGB with an out-of-fold
RMSE of 0.668
(95% scaffold-bootstrap CI
0.551–0.791).

The multi-conformer EGNN achieved an RMSE of
0.861
(95% CI
0.716–1.013).

Relative to ECFP4-XGBoost, the EGNN RMSE improvement was
-0.190
(95% CI
-0.321 to
-0.073),
where positive values would favour the EGNN.

## Defensible conclusion

Three-dimensional geometric learning was not universally superior to
molecular fingerprints. ECFP4 models generalized better on the strict
ALOX15 scaffold-disjoint benchmark. The COX-2 results indicate that
geometric utility may be endpoint-dependent.

## Candidate limitation

The screened compounds were reported in other Lilium species. They are
not confirmed constituents of Lilium mackliniae and must be described as
transferable, literature-supported candidates only.