# Galaxy Zoo star-formation rate data analysis activity

This activity uses the data for Fig. 6 and 7 of [this paper](https://arxiv.org/pdf/1703.02053). It compares two different estimates of the star-formation rate for samples of galaxies with different numbers of spiral arms (see Figure. 11 in this [other paper](https://arxiv.org/pdf/1607.01019)).

Star-formation rates (SFRs) are estimated directly from far-UV (FUV) and mid-infrared (MIR; 22 micron) photometry. Stellar mass is used to determine the specific star-formation rate (sSFR).

The provided data does not perfectly match that used in the above papers, so you will not be able to exactly reproduce their plots and results, but they should be close.

One could:
* Show that the scatter in a distribution is significantly larger than the uncertainties, i.e. there is intrinsic variation in the L_FUV, sSFR, etc. of galaxies.
* Use different sized samples to demonstrate that the error on the mean goes as 1/sqrt(N), and that it has a Gaussian distribution, even when the original quantity is non-Gaussian.
* Propagate errors for eqns. (4), (5), (6), log(sSFR) and also for log(SFR_FUV/SFR_22).
* Test for statistical differences in mean log(sSFR) and log(SFR_FUV/SFR_22) for galaxies with different numbers of spiral arms. Maybe you could first use resampled distributions of different sizes, then show that the results are the similar if you propagate the Gaussian error on the mean.
* You could then introduce bootstrap resampling and show it gives the same result.
* As a more compelling case for the bootstrap, you could consider a more complicated statistic, e.g. the median or the skew of the distribution, and see if it changes significantly with spiral arm number.

## Files

- analysis.ipynb - a (currently incomplete) example data analysis
- data.csv - the prepared data for use by analysis.ipynb and students
- data.ipynb - used for assembling the dataset from original sources
