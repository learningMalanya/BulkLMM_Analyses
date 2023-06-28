## Version 1.1.0:

#### Closed issues:
- No issues were closed compared to last release [(v 1.0.1)](https://github.com/senresearch/BulkLMM.jl/releases/tag/v1.0.1).

#### Merged pull requests:
- Revised the algorithm for fast eQTL scans using grid-search for heritability estimated independently for each tested marker and trait. The new algorithm now produces more reliable results. The function `bulkscan_alt_grid()` now also reports the heritability estimates for each marker and trait, stored in a 2-dimensional array. [#75](https://github.com/senresearch/BulkLMM.jl/pull/75)
- Updated the function `scan(...; permutation_test = true)` for the feature of permutation testing: it now reports the variance components estimated under the null model, the raw output from permutation testing  (LOD scores for permuted copies), and the LOD scores for the original tested trait. [#75](https://github.com/senresearch/BulkLMM.jl/pull/75)
- Revised the implementation of the function for constructing the kinship matrix from given genotype information: used matrix multiplication to reduce the computational cost when sample size and/or marker size is large. [#77](https://github.com/senresearch/BulkLMM.jl/pull/77)
- As the package BigRiverQTLPlots.jl we developed is currently public, we updated the README.md of BulkLMM.jl by including the code to reproduce the example figures in the README.md. [#78](https://github.com/senresearch/BulkLMM.jl/pull/78)

For more details, please check [NEWS.md](https://github.com/learningMalanya/BulkLMM.jl/blob/main/NEWS.md).

---
## Version 1.0.2:

#### Closed issues:
- Modified source code for grid-search algorithms: allowed the feature of regularization using Bayes on the objective function [(#55)](https://github.com/senresearch/BulkLMM.jl/issues/55) 
- Created [NEWS.md] file for detailed description for major updates [(#56)](https://github.com/senresearch/BulkLMM.jl/issues/56)

#### Merged pull requests:
- Preparation for official release of new features: simplified the interface for the feature, added tests;
- Added a small change in source code: `bulkscan_null_grid()` (using grid-search algorithm) previously does an implicit standardization to input matrices, which interferes and can cause accuracy issues with the new feature (when weighted variances added in); this modification will not affect performance of the function compared to last release.
[#73](https://github.com/senresearch/BulkLMM.jl/pull/73)
---
## Version 1.0.1:

#### Closed issues:
No issue was closed compared to last release.

#### Merged pull requests:
- Added the feature for modeling heteroskedastic variance component unexplained by genetic variants [(#69)](https://github.com/senresearch/BulkLMM.jl/pull/69)
- Registered version 1.0.1 in Project.toml [(#71)](https://github.com/senresearch/BulkLMM.jl/pull/71).

