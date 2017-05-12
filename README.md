# alpha_Subaru_2017
<a href="https://doi.org/10.5281/zenodo.574904"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.574904.svg" alt="DOI"></a>
<!---
<a href="https://zenodo.org/badge/latestdoi/20001/MTMurphy77/alpha_Subaru_2017"><img src="https://zenodo.org/badge/20001/MTMurphy77/alpha_Subaru_2017.svg" alt="10.5281/zenodo.XXXXX"></a>
--->

Quasar spectra and absorption profile fits associated with Murphy &amp; Cooksey (2017, MNRAS, submitted)
<!---
<a href="http://dx.doi.org/10.1093/mnras/stw1482">doi:10.5281/zenodo.51504</a>, <a href="http://arxiv.org/abs/1606.06293">arXiv:1606.06293</a>
-->

Read this README, and view/download/use the files within this repository, in conjunction with a careful read of the paper itself.

If you use any of the materials in this repository, please cite the paper. If you want to cite only the data and/or fits (for some reason), please use the DOI: <a href="https://doi.org/10.5281/zenodo.574904"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.574904.svg" alt="DOI"></a>

The paper is available at the following websites, in published or pre-print form:<br>
&ndash; arXiv.org: TBD<br>
&ndash; MNRAS (via DOI): TBD<br>
&ndash; NASA/ADS: TBD<br>

This repository contains a folder for each quasar, named using the quasar name (used in the paper), i.e. J0120+2133 and J1944+7705.

Each quasar folder contains one or more sub-folder which is the nominal redshift of the absorption system fitted in the paper (e.g. 1.3254).

Each redshift folder contains the following files:<br>
&ndash; FITS file or files containing the "master spectrum" used in the profile fits to the absorber. The FITS files were produced using UVES_popler;<br>
&ndash; fit_iso.f13: Absorption profile parameter file containing the final parameter values determined by VPFIT (as at the end of the fit_iso.f18 file). The absorption profile fit was run in VPFIT using the commented-out command in the first line of this file.<br>
&ndash; fit_iso.f18: Record of VPFIT iterations, ending with the parameters in fit_iso.f13 and including the parameter statistical uncertainties.<br>
&ndash; MM_VPFIT_2013-11-10.dat: Copy of the atomic data file used by VPFIT from the <a href="https://github.com/MTMurphy77/MMatomdat">repository</a> associated with <a href="http://adsabs.harvard.edu/abs/2014MNRAS.438..388M">Murphy & Berengut (2014, MNRAS, 438, 388, arXiv:1311.2949)</a>.<br>
&ndash; vp_setup.dat: The setup file for VPFIT used to run the fit in fit_iso.f13

The other files in the top-level directory include a table of all 27 recent, distortion-correct/resistant measurements of alpha in quasar absorbers (tab_alpha_results.tex), and all files needed to produce the plots in the paper (plus a couple that were not included) via the ipython notebook "plots_for_paper.ipynb".
