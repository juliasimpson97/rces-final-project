# *Investigating Ocean Acidification in the Arctic* 
## Final Project for Research Computing in Earth Science
### Julia L. Simpson, Fall 2022

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pangeo-data/pangeo-docker-images/2022.09.21?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fjuliasimpson97%252Frces-final-project%26urlpath%3Dlab%252Ftree%252Frces-final-project%252Ffinal_project.ipynb%26branch%3Dmain)


## Scientific Question: 
The goal of this project is to explore the science discussed in Krasting et al. 2022, linked [here]( https://www.nature.com/articles/s43247-022-00419-4). This paper investigated ocean acidification specifically in the Arctic, using machine learning to classify different "clusters" based on varying extents and mechanisms of acidication.
They were able to do this analysis using a relatively low number of driver variables: the classification was based only on sea surface temperature (SST), sea surface salinity (SSS), and surface pH. Interestingly, they found that the boundaries of the clusters correlate strongly with sea ice extent, with one cluster bounded by present-day sea ice extent and another bounded by mid-century sea ice extent. (Of the remaining clusters, one was not consistently identified by the machine learning algorithm and the other did not exhibit as extreme acidification as the main two clusters). This leads me to wonder about the extent of the relationship between sea ice concentration and ocean acidification in the Arctic.

## Datasets
### pCO2 
- Data Source: https://www.ncei.noaa.gov/data/oceans/ncei/ocads/data/0253659/SOCATv2022_Gridded_Dat/
- OR
https://figshare.com/collections/Large_ensemble_pCO2_testbed/4568555

### Sea Surface Temperature
- SST monthly means: https://polarwatch.noaa.gov/erddap/files/afsc_sst/sst.csv

### Sea Surface Salinity
- 

### Sea Surface pH
- 

### Sea Ice Concentration
- Sea Ice Concentration, NOAA/NSIDC Climate Data Record V3, Arctic, 25km, Science Quality, 1978-2019, Monthly DEPRECATED
https://polarwatch.noaa.gov/erddap/files/nsidcCDRiceSQnhmday/


## Intended Analysis
I'm curious regarding the extent of a potential correlation between sea ice concentration, pC02, and pH. If sea ice concentration seems to be similarly correlated with pC02 and pH changes, that would suggest that much of the increase in pCO2 in the Arctic comes from melting ice–which is typically low in pCO2 and therefore a meaningful potential sink for carbon dioxide, providing an avenue for acidification. 

The paper also posited a mechanism explaining why one of the clusters did not exhibit as extreme acidification, explaining that increased salinity in that water mass offers a buffer that delays corrosion of waters. Therefore, in addition to the potential correlations discussed above, I'll also investigate the relationships between SST/SSS and pCO2/pH.

Finally, I want to analyze the Arctic basin with sea ice concentration as a classifying lens for water masses, as opposed to using a machine learning algorithm (which was not based on sea ice but yielded results suggesting the relationship). If classifying water masses by sea ice concentration can yield similar correlations to those seen in the clusters identified by the algorithm, there may be avenues for research in this area that don't require machine learning.