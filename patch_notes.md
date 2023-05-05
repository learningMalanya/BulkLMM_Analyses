## Version 1.1.0:
---
#### Closed issues:
- Modified source code for grid-search algorithms: allowed the feature of regularization using Bayes on the objective function [(#55)](https://github.com/senresearch/BulkLMM.jl/issues/55) 
- Created [NEWS.md] file for detailed description for major updates [(#56)](https://github.com/senresearch/BulkLMM.jl/issues/56)

#### Merged pull requests:
- Preparation for official release of new features: simplified the interface for the feature, added tests;
- Added a small change in source code: `bulkscan_null_grid()` (using grid-search algorithm) previously does an implicit standardization to input matrices, which interferes and can cause accracy issues with the new feature (when weighted variances added in); this modification will not affect performance of the function compared to last release.
[#73](https://github.com/senresearch/BulkLMM.jl/pull/73)
---
## Version 1.0.1:
---
#### Closed issues:
No issue was closed compared to last release.

#### Merged pull requests:
- Added the feature for modeling heteroskedastic variance component unexplained by genetic variants [(#69)](https://github.com/senresearch/BulkLMM.jl/pull/69)
- Registered version 1.0.1 in Project.toml [(#71)](https://github.com/senresearch/BulkLMM.jl/pull/71).

