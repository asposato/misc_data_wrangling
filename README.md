# misc_data_wrangling
various scripts that may aid in single-cell or lineage tracing analysis

### merging allReadCounts
`merge_allReadCounts_files.Rmd` is an R Notebook that takes multiple .allReadCounts files and combines them into one file. The purpose of this script is to merge .allReadCounts files that are derived from the same animal. This would be desired if you want to generate an hmid plot for a single animal that was sequenced across multiple samples. This is likely the case for lineage barcodes retrieved from single-cell data since we often split cells from a tissue across multiple channels of 10X. For input, it takes `sample1.allReadCounts` and `sample2.allReadCounts` files and outputs a file like `sample1andsample2.allReadCounts`.

