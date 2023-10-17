

# Bootstrap analysis of significance of correlation of CSP binding vs Protection in vaccinees of the RTS,S/AS01 vaccination trial.

This analysis demonstrates a statistically significant relationship between the CSP binding fraction of a vaccinee's plasmablast repertoire and the protection against infection for that vaccinee.

## Installation.

1. Install R version `4.1.1`.
2. Install the 'renv' package.
3. Use renv::restore to recreate the R environment for this analysis.

## Analysis.

The output of this analysis is contained in the `RTS_S_CSPBinding_vs_Protection.nb.html` file.

## Re-running.

To rerun the analysis using the cached 20,000 bootstrap samples in `bootset_*.RDS` simply rerender the R markdown file:

```
	> library(rmarkdown); 
	> render("RTS_S_CSPBinding_vs_Protection.Rmd",output_file="my_rerun.html");
```

To rerun the analysis from scratch, delete the the `bootset_*.RDS` files.  If preferred, change the number of bootstrap samples to use by changing the `bootn=20000;` line in the `bootnchunk`.

```
	$ rm bootset_*.RDS
	> library(rmarkdown); 
	> render("RTS_S_CSPBinding_vs_Protection.Rmd",output_file="my_rerun.html");
```

